This website repository is published at https://floability.github.io.

To test changes locally:

```
conda create -n website-dev -c conda-forge
conda active website-dev
conda install -c conda-forge rb-jekyll

# kramdown is somehow missing or incorrect in the conda package: 
gem install kramdown

# run jekyll to generate the site and a local preview:
jekyll serve

# in a separate window, open a web browser e.g.
firefox http://localhost:8888
```

