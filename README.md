This is my blog running on [jan-berndt.de](https://jan-berndt.de).

To run locally:

```
hugo version # should be v0.139.4
hugo server -D
```

To change theme:

```
cd themes/hugo-theme-stack
git commit -am 'updates'
git push
cd ...
git commit -am 'updates'
git push
```

To combine all posts into one big file:

`find content/posts -type f -name "*.md" -exec cat {} + > combined.tmp`
