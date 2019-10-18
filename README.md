I'm migrating my blog to GitHub Pages. The page is [live](https://exo.pm), but it is still a work in progress.

## Tasks
- [x] Migrate posts and sites
- [ ] Check posts and sites
- [ ] Check redirects
- [x] Migrate theme!
- [x] Add custom domain with https

## Notes

To include images, put them into `_site/images/` and include them in a post like this:

```
{% include image.html src="sample-image.jpg" src-full="sample-image-full.jpg"  width="300px" title="Sample Title" %}
```

Only `src` is required. `src-full` defaults to the value of `src`, and `width` defaults to `100%`.
