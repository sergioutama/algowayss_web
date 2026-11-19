# PT Algoway System Solution

Jekyll source for [www.algowayss.com](https://www.algowayss.com/).

## Local development

Use the Ruby version in `.ruby-version`. Run `bundle install`, then
`bundle exec jekyll serve` and open <http://localhost:4000>.
To reproduce the production build, run
`JEKYLL_ENV=production bundle exec jekyll build --strict_front_matter`.

The homepage is in `index.html`, articles are in `_posts/`, and the
contact form endpoint and canonical domain are in `_config.yml`.

## Contact form

Set `contact_endpoint` in `_config.yml` to the public HTTPS URL that accepts
enquiries. The form posts `name`, `email`, `phone` and `message` as standard
HTML form data. The endpoint handles delivery and displays the result to the
visitor. Configure the recipient privately with the backend. The preview
disables submission while the endpoint is blank.

## GitHub Pages

For the first release, select **Settings → Pages → Build and deployment →
Source → GitHub Actions**. The workflow builds pull requests with the locked
Jekyll dependencies. A push to `master` builds and publishes `_site/`.
The workflow can also be run manually from `master`.
The custom domain is `www.algowayss.com`.
