This website repository is published at https://floability.github.io.

To test changes locally:

```bash
conda create -y -n floability-site -c conda-forge \
  ruby=3.3 \
  c-compiler \
  cxx-compiler \
  make
conda activate floability-site

# Use Conda's RubyGems executable explicitly. On macOS, plain `gem` may resolve
# to the system Ruby instead of the Ruby installed in this environment.
"$CONDA_PREFIX/bin/gem" install --no-document --force \
  jekyll \
  jekyll-theme-modernist \
  jekyll-seo-tag \
  webrick

jekyll build
jekyll serve --livereload --host 127.0.0.1 --port 4000
```

Open the tutorial landing page at:

```text
http://127.0.0.1:4000/tutorial/
```
