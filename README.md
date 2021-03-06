[![Build status](https://dev.azure.com/patros/OpenSource/_apis/build/status/docker-geoserver-azure-web-app)](https://dev.azure.com/patros/OpenSource/_build/latest?definitionId=20)
![Docker Pulls](https://img.shields.io/docker/pulls/coderpatros/geoserver-azure-web-app.svg)

# GeoServer Azure Web App Docker Container

Available from Docker Hub as `patroscoder/geoserver-azure-web-app`

`/home/geoserver-data` is used as the GeoServer data directory.

To enable persistent storage make sure you set the appsetting `WEBSITES_ENABLE_APP_SERVICE_STORAGE` to `true`.

# Currently Maintained Versions

I currently maintain images for the current stable and maintenance releases of
GeoServer. Although there can be a slight delay between GeoServer releases and
new point releases of this image.

# Base Image & Tags

This image is based on my other image `patroscoder/geoserver-base`. Which in
turn uses `openjdk:8-jre-alpine` as a base image to minimise image size and
risk of vulnerable packages.

I create latest tags for each minor version. i.e. `2.15-latest`.

I rebuild the images regularly to ensure I pull in any updates to the base
image. So I recommend you use one of these tags to ensure you get the latest
security updates.

But keep in mind, I drop support for minor versions when GeoServer does.

# Microsoft Core Fonts

Please note that this docker image contains the Microsoft Core Fonts.

[Microsoft Core Fonts EULA](http://corefonts.sourceforge.net/eula.htm)