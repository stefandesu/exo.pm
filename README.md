# exo.pm

My personal blog, hosted at https://exo.pm.

## Tasks

- [ ] Do not regenerate all images on each build (requires cloning `gh-pages` branch into folder `_site` before building)
- [ ] Make [PageSpeed Insights](https://pagespeed.web.dev) happy (still complains about "Properly size images" and some other things)
- [ ] With the update to Jekyll 4 and deployment via GitHub Actions, part of the footer got lost; need to investigate
- [ ] Add image captions
- [ ] In the future: Technically rebuild the whole site (e.g. with Astro)

## Notes

### Images
To include images, put them into `_images` and include them in a post like this:
```
{% picture test.jpg %}
```

See https://rbuchberger.github.io/jekyll_picture_tag/ for more details.

Before committing any images to the repository, remove dates and GPS metadata from the EXIF:

```sh
exiftool -alldates= -gps:all= -DateCreated= _images/**/*
```

TODO: Automate this (pre-commit hook?)

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
- Ruby (>=3)
- bundler (gem install bundler)
- dependencies (bundle install)

Then run `bundle exec jekyll serve`.
