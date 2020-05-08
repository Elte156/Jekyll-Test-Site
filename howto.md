---
layout: page
title: How To
permalink: /how-to/
---

Use these commands to build a Jekyll Site.

```bash
# Create a brand new site
docker run --rm --volume="$PWD:/srv/jekyll" -it jekyll/builder:3.8 jekyll new .
# Build the site
docker run --rm --volume="$PWD:/srv/jekyll" -it jekyll/builder:3.8 jekyll build
# Serve the site via HTTP and watch for changes
docker run --rm --volume="$PWD:/srv/jekyll" -p 4000:4000 -it jekyll/builder:3.8 jekyll serve --watch --drafts
```

Visit the site: <http://localhost:4000/>
