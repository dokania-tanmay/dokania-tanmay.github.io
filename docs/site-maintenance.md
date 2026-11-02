# Security and search follow-up

The site no longer references the compromised polyfill.io service. MathJax
remains enabled. Theme sample posts, announcements, placeholder projects,
people/submenu pages, the empty blog/news landing pages, and standalone demo
HTML/notebook files have been removed. The theme author's Medium feed import
and blog archive generation are disabled. Personal publications and projects
remain published.

## Build and deploy

With Ruby and the Gemfile dependencies installed, run:

```sh
JEKYLL_ENV=production bundle exec jekyll build --lsi
```

Push the reviewed changes to the existing `main` or `master` branch to run the
repository's GitHub Actions deployment. That workflow builds `_site` and
publishes it to GitHub Pages. Check that the workflow succeeds before requesting
security or indexing reviews.

After deployment, verify:

- View the homepage's source and confirm it has no polyfill.io script.
- Check mathematical notation on a project page still renders.
- Open `/sitemap.xml`: it should include the homepage and personal pages but no
  sample blog posts, announcements, placeholder projects, or people page.
- Open a removed URL such as `/blog/2023/tikzjax/`: it should return HTTP 404,
  without an automatic redirect. Do not block these old URLs in robots.txt;
  crawlers need to see that they have been removed.

## Search engines

1. Add `https://dokania-tanmay.github.io/` as a URL-prefix property in Google
   Search Console. For HTML-tag verification, put the supplied token in
   `google_site_verification` in `_config.yml` and set
   `enable_google_verification: true`, then deploy and complete verification.
   Never use an invented verification token.
2. Inspect the homepage with URL Inspection. Check the reported indexing reason
   and selected canonical URL, and review Security issues and Manual actions.
3. Submit `https://dokania-tanmay.github.io/sitemap.xml`. Once any reported
   issues are resolved, request homepage indexing or a security review as
   appropriate. Indexing and ranking are controlled by the search engine.
4. Bing Webmaster Tools can similarly use `bing_site_verification` with
   `enable_bing_verification: true`.

## Security classification

Request a review from each service that still flags the deployed site. For
Georgia Tech, use the Security Operations Center contact in the block page and
include the complete block details, affected URL, timestamp, and the removal
of the polyfill.io dependency. The screenshot alone does not identify the
vendor or classification that triggered the block. Removing the script does
not automatically clear existing reputation records.
