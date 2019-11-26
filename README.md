I'm migrating my blog to GitHub Pages. The page is [live](https://exo.pm), but it is still a work in progress.

## Tasks
- [x] Migrate posts and sites
- [x] Check posts and sites
- [x] Check redirects
- [x] Migrate theme!
- [x] Add custom domain with https

## Notes

### Images
To include images, put them into `_site/images/` and include them in a post like this:
```
{% include image.html src="sample-image.jpg" src-full="sample-image-full.jpg"  width="300px" title="Sample Title" %}
```

Only `src` is required. `src-full` defaults to the value of `src`, and `width` defaults to `100%`.

To include floating left images, use the following instead:
```
{% include image-left.html src="sample-image.jpg" width="100px" title="Sample Title" %}
```

At the moment, these can't be linked (only manually). Default `width` is 200 pixels.

### Footnotes
```
Some text[^1].

Some other text[^2].

The identifier in the square brackets does not have to be numeric[^my_footnote].

[^1]: Some footnote.
[^2]: Other footnote.
[^my_footnote]: This also works fine.
```

### Local Testing
For local testing, you need:
- Ruby (>=2.4)
- bundler (gem install bundler)
- dependencies (bundle install)

Then run `bundle exec jekyll serve` ([see also](https://help.github.com/en/articles/testing-your-github-pages-site-locally-with-jekyll)).
