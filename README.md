# Potrace as a service

A simple web service that traces the given bitmap image into an SVG file. 

Run with `docker run -p 8080:8080 gcr.io/as-a-service-dev/trace`

[![Run on Google Cloud](https://storage.googleapis.com/cloudrun/button.png)](https://console.cloud.google.com/cloudshell/editor?shellonly=true&cloudshell_image=gcr.io/cloudrun/button&cloudshell_git_repo=https://github.com/as-a-service/trace.git)

### URL parameters:

* `input`: URL of the image to trace.

## Running the server locally

* Build with `docker build . -t trace`
* Start with `docker run -p 8080:8080 trace`
* Open in your browser at `http://localhost:8080/?url=https://www.wikipedia.org/portal/wikipedia.org/assets/img/Wikipedia-logo-v2.png`

## Deploy to your server

The following container image always reflects the latest version of the `master` branch of this repo: `gcr.io/as-a-service-dev/trace`

## TODO

* also accept images via POST requests.
