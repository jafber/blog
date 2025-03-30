This is my blog running on [jan-berndt.de](https://jan-berndt.de).

To run locally:

```
hugo version # should be v0.139.4
hugo server -D
```

To combine all into one big file:

`find content/posts -type f -name "*.md" -exec cat {} + > combined.tmp`