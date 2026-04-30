---
layout: post
title: "How We Built a Self-Operating Team of AI Agents"
date: 2026-04-30
category: Blog
---

We did not set out to build a team of AI agents. We set out to solve a very human problem: how do you run a fast-moving company when every task requires context-switching, coordination, and follow-through?

The answer, it turns out, is that you do not. You let the agents do it.

## What Is Multi-Agent Orchestration?

Multi-agent orchestration is the practice of deploying multiple AI agents — each with a defined role, tools, and scope of authority — and letting them coordinate through a shared task management system. Instead of a single AI assistant answering questions, you have a team of specialists that assign work to each other, track progress, and escalate when blocked.

Think of it as building an org chart for AI, then watching it run.

At Algoway, we built exactly that. Our system runs seven agents, each with a distinct role, communicating through a platform called Paperclip. Here is what we learned.

## Our Agent Ecosystem

Our team is modeled on a real company structure:

- **CEO** — The orchestrator. Routes tasks, makes architectural decisions, keeps the captain (human owner) informed. Everything flows through CEO.
- **Alex** — Senior Engineer. Handles all coding, infrastructure automation, and technical builds.
- **Meutia** — COO. Manages consulting deliverables, content production, business operations, and financial reporting through Johnny.
- **Jancuk** — Knowledge and Research. Runs deep research tasks, social media automation across four platforms, and market analysis.
- **cuk_infra** — Infrastructure bot. Monitors servers, applies updates, restarts services, and responds to daily health checks.
- **Hermes** — Communications. Handles Telegram relay, external messages, and notification routing.
- **Meridian** — Trading bot. Executes autonomous trading decisions with community-intelligence inputs.

Each agent has a defined set of tools, a reporting chain, and a budget cap. They do not talk to each other directly — they communicate through issues.

## How Agents Communicate Through Paperclip

Paperclip is our issue-based orchestration layer. Every task — whether it is writing a blog post, restarting a service, or executing a trade — is an issue in Paperclip. Agents wake up in heartbeats, check their inbox, check out the highest-priority task, do the work, and post a comment with their progress.

This sounds simple. The power is in the constraints.

Because every action is logged as a comment on an issue, there is a full audit trail of every decision an agent makes. Because agents must check out tasks before working on them, there are no race conditions. Because status transitions are explicit (todo to in_progress to done, or blocked with a named unblocking owner), nothing falls into a void.

When CEO routes a task to Alex, Alex's next heartbeat picks it up. When Alex delegates to cuk_infra, the infrastructure agent runs the command and reports back. The whole system is asynchronous but traceable.

## Real-World Results

**Meridian** has completed 46 autonomous trades with a 76% win rate. The agent pulls community intelligence from curated channels, applies Darwinian learning — strategies that work get reinforced; those that do not get blacklisted — and executes without human input. Auto-blacklisting prevents repeated mistakes from compounding.

**Jancuk** manages social media presence across four platforms from a single command. When Meutia needs a post published, she creates a task. Jancuk drafts, formats for each platform, and publishes — usually in one heartbeat.

**cuk_infra** runs daily infrastructure health checks. When disk usage crosses a threshold, it cleans up. When a systemd unit fails, it restarts it and posts a report. Tier 2 updates (kernel, bootloader, network stack) get flagged for human approval before anything touches them.

## The Shim Pattern

One of the more interesting engineering decisions was how we handle different AI backends. Our agents do not all run the same model. CEO and Alex use Claude Code. Meridian uses a specialized trading model. Some agents run via DeepSeek.

To make these interoperable, we use a shim pattern. Each agent has an adapter configuration that specifies its backend, its working directory, its instruction file path, and its tool permissions. Paperclip routes heartbeats to the right adapter without the agents needing to know anything about each other's underlying infrastructure.

This means we can swap out a model for any agent without changing a single line of agent logic. The interface is the issue.

## Lessons Learned

**Explicit status matters.** Early on, agents would mark tasks done when they were only partially complete. Now every status transition requires a comment explaining what was done and what remains. This single change cut our hallucinated-completion rate dramatically.

**Budget caps prevent runaway loops.** Each agent has a budget ceiling. When an agent hits 80%, it focuses only on critical tasks. At 100%, it pauses. This has prevented several situations where an agent got into a retry loop on a failing task.

**Blocked does not mean silent.** When a task is blocked, the agent must name the blocker and who needs to unblock it before going dormant. No blocked task is ever invisible.

**Self-hosting gives you control.** Our primary stack runs on a Mac Mini on-premise, with Railway as a cloud fallback. We own our data, our uptime, and our costs. When something breaks, we debug it — we do not wait for a vendor.

## What Comes Next

We are building toward a system where agents do not just execute tasks — they propose them. Jancuk already surfaces research that CEO routes into new initiatives. Meridian is developing strategy templates based on historical performance.

The goal is not to remove humans from the loop. It is to move humans up the loop — from execution to decision-making, from task management to goal-setting.

A self-operating team of AI agents is not science fiction. It is a Tuesday at Algoway.
