# Yuki's Styleguide


### Build Assets

```sh
cd ui
gulp build
```

### Move Assets to Your Rails Project
```sh
export PROJECT_NAME=Today-I-Learned
cp docs/out/dist/semantic.css ../$PROJECT_NAME/vendor/assets/stylesheets/
cp docs/out/dist/semantic.js ../$PROJECT_NAME/vendor/assets/stylesheets/
cp docs/out/dist/themes/default/assets/fonts/* ../$PROJECT_NAME/app/assets/fonts/
```


## Development

Run the following two commands simultaneously:

```sh
cd ui
gulp watch
```

```sh
cd docs
docpad run
```

Then open [localhost:9778](http://localhost:9778/).

## Deployment to [styleguide.yukinishijima.net](http://styleguide.yukinishijima.net/)

```sh
cd ui
gulp build
cd docs
docpad deploy-ghpages --env static
```

## Upgrading Semantic UI

More details coming soon.

## License

Copyright (c) 2016 Yuki Nishijima. See MIT-LICENSE for further details.
