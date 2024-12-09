# Nextcloud-Extras

Nextcloud image with extra packages

* This image is a multiplatform (ARM and x86) implementation of the Nextcloud Image with extra packages like imagemagick and ffmpeg.
* The image is kept in DockerHub for convenience and can be pulled directly via `docker pull pnatel/nextcloud-imagemagick-ffmpeg:<TAG>`

* Dockerfile available in the [GitHub repo](https://github.com/pnatel/Nextcloud-Extras) for reference.

## Notes

* Added packages for the [Extract app](https://apps.nextcloud.com/apps/extract)
  This app is unsupported at the moment and it is included for testing only.

## The available tags represent

Check latest Github Actions date for image tag age [![Build Nextcloud image with extra packages](https://github.com/pnatel/Nextcloud-Extras/actions/workflows/nc-dockerimage.yml/badge.svg)](https://github.com/pnatel/Nextcloud-Extras/actions/workflows/nc-dockerimage.yml)

- nc-30-apache/dev/current - Current Nextcloud 30 release as per latest Github action date 
- nc-29-apache/prod/old - Current Nextcloud 29 release as per latest Github action date 
- nc-28-apache - outdated (v.28.0.12 on 01/12/2024)
- nc-27-apache - outdated (v.27 on 27/04/2024)

Hit me up on Discord (@pnatel) if you have questions.
