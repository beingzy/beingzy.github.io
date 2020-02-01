```
docker run --rm -it --volume="$PWD:/srv/jekyll" \
    --volume="$PWD/vendor/bundle:/usr/local/bundle" \
    --env JEKYLL_ENV=production jekyll/jekyll:4.0 jekyll build
```
* `--rm`: auotmatically removes the container when it exits
* `--volumne="$PWD:/srv/jekyll"` taks the current diectory indicated by `$PWD` and map it to the directory at `/srv/jekyll` within the container so taht it could build it
* `--volumne="$PWD/vender/bundle:/usr/local/bundle" this option maps the contents of the current directory's `/vendor/bundle` and maps it to `/usr/local/bundle`. The reason for this option is so that gems could be cached and resued in future builds.
* `--env JEKYLL_ENV=production` in various parts of the project, this tag tells to render contents only if for production* `jekyll/jekyll:4.0` this tells it to use `jekyll:4.0` as base image.
* `jekyll build` runs the build command for jekyll
