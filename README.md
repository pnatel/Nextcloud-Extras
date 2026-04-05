# Nextcloud-Extras

Nextcloud image with extra packages

* This image is a multiplatform (ARM and x86) implementation of the Nextcloud Image with extra packages like imagemagick and ffmpeg.
* The image is kept in DockerHub for convenience and can be pulled directly via `docker pull pnatel/nextcloud-imagemagick-ffmpeg:<TAG>`

* Dockerfile available in the [GitHub repo](https://github.com/pnatel/Nextcloud-Extras) for reference.

## Notes

* Added packages for the [Extract app](https://apps.nextcloud.com/apps/extract)
  This app is unsupported at the moment and it is included for testing only.
* The repo does not need to have a recent commit to be "up to date" check for [Github actions date](https://github.com/pnatel/Nextcloud-Extras/actions/workflows/nc-dockerimage.yml) for latest available content.

## The available tags represent

Check latest Github Actions date for image tag age [![Build Nextcloud image with extra packages](https://github.com/pnatel/Nextcloud-Extras/actions/workflows/nc-dockerimage.yml/badge.svg)](https://github.com/pnatel/Nextcloud-Extras/actions/workflows/nc-dockerimage.yml)

- nc-33-apache/dev/current - Nextcloud 33 release as per latest [Github action date](https://github.com/pnatel/Nextcloud-Extras/actions/workflows/nc-dockerimage.yml)
- nc-32-apache/prod/old - Nextcloud 32 release as per latest [Github action date](https://github.com/pnatel/Nextcloud-Extras/actions/workflows/nc-dockerimage.yml)
- nc-31-apache - outdated (Nextcloud Hub 10 31.0.14 (Mar/2026)
- nc-30-apache - outdated (Nextcloud Hub 9 (30.0.17) on Dec/25)
- nc-29-apache - outdated (v.29.0.11 on 29/01/2025)
- nc-28-apache - outdated (v.28.0.12 on 01/12/2024)
- nc-27-apache - outdated (v.27 on 27/04/2024)
Refer to [Nextcloud Maintenance and Release Schedule](https://github.com/nextcloud/server/wiki/Maintenance-and-Release-Schedule) for lifecycle details. 


Hit me up on Discord (@pnatel) if you have questions.
