# PT Algoway System Solution

Jekyll source for [www.algowayss.com](https://www.algowayss.com/).

## Local development

Use the Ruby version in `.ruby-version`. Run `bundle install`, then
`bundle exec jekyll serve` and open <http://localhost:4000>.
To reproduce the production build, run
`JEKYLL_ENV=production bundle exec jekyll build --strict_front_matter`.

The homepage is in `index.html`, articles are in `_posts/`, and the
Formspree form ID and canonical domain are in `_config.yml`.

## Contact form

Create a form in the [Formspree dashboard](https://formspree.io/forms) and
select the inbox that should receive enquiries. In the form’s Integration tab,
copy the ID at the end of the endpoint URL into `formspree_form_id` in
`_config.yml`. Rebuild the site after setting the ID.

The form sends the visitor’s name, email, phone and message directly to
Formspree using an HTML POST. Formspree displays the submission result and
manages notification delivery. The draft disables submission while the ID is
empty. The recipient address belongs in Formspree’s settings.

## GitHub Pages

For the first release, select **Settings → Pages → Build and deployment →
Source → GitHub Actions**. The workflow builds pull requests with the locked
Jekyll dependencies. A push to `master` builds and publishes `_site/`.
The workflow can also be run manually from `master`.
The custom domain is `www.algowayss.com`.
