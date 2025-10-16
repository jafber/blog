This is the repository for my personal blog running on [jan-berndt.de](https://jan-berndt.de).

## Run Locally

```
git submodule update --init --recursive # pull in theme repository
hugo version # should be v0.139.4
hugo server -D
```

## Cimeyclust Deployment

- workflow `.github/hugo.yml` runs on every push to main
- uses `web111_blog` FTP credentials from [Cimeyclust webspace](https://liveconfig.cimeyclust.org/liveconfig/hosting/webspace)

## Development Notes

### Emoji

See [hugo emoji reference](https://gohugo.io/quick-reference/emojis/).

### Make Theme Adjustments

```
cd themes/hugo-theme-stack
git commit -am 'updates'
git push
cd ...
git commit -am 'updates'
git push
```

### Combine All Posts Into One File

To feed LLMs.

```
find content/posts -type f -name "*.md" -exec cat {} + > combined.tmp
```
