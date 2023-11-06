# shinyverse

[![Docker Build & Push](https://github.com/rmgpanw/shinyverse/actions/workflows/docker-build-push.yml/badge.svg)](https://github.com/rmgpanw/shinyverse/actions/workflows/docker-build-push.yml)

This repository uses GitHub Actions to build a docker image that includes both RStudio Server and RShiny Server. Launch RStudio server as you would for the base rocker image (see [Rocker Project documentation](https://rocker-project.org/images/versioned/rstudio.html#overview)) and Shiny Server will also be running at port `3838`. For example:

```
docker run -ti --rm -p 8787:8787 -p 3838:3838 --name rstudio_shiny_server rmgpanw/shinyverse
```