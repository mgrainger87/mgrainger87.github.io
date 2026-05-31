# mgrainger87.github.io

Minimal Jekyll + Minimal Mistakes academic website for GitHub Pages.

## Local setup

1. Install and activate a modern Ruby with Homebrew:
   - `brew install chruby ruby-install`
   - `ruby-install ruby 3.3.4`
   - Add to `~/.zshrc`:
     - `source $(brew --prefix)/opt/chruby/share/chruby/chruby.sh`
     - `source $(brew --prefix)/opt/chruby/share/chruby/auto.sh`
     - `chruby ruby-3.3.4`
2. Restart your shell.
3. Install gems: `bundle install`
4. Run the site: `bundle exec jekyll serve`
5. Open: `http://127.0.0.1:4000`

## Content to customize

- `_config.yml`: name, bio, links, email, location, domain
- `index.md`: short academic profile and research overview
- `_pages/publications.md`: publication list
- `_pages/contact.md`: contact details
- `assets/files/cv.pdf`: your CV PDF

## GitHub Pages

- Repository name must be `mgrainger87.github.io`
- Pages should publish from **GitHub Actions**
- After the first successful deploy, the site will appear at `https://mgrainger87.github.io`

## Custom domain

1. Verify your domain in GitHub.
2. Update `_config.yml` so `url` matches your apex domain.
3. In repository settings, set the custom domain to your apex domain.
4. Point the apex domain via `A`/`ALIAS`/`ANAME` records per your DNS provider.
5. Point `www` to `mgrainger87.github.io` with a `CNAME`.
6. Enable HTTPS in GitHub Pages after DNS propagation completes.
