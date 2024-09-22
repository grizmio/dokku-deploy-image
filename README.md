# dokku-deploy-image

Pull the image with docker and run ps:rebuild

## Example

Imagine this, you use docker images for build and deploy, you just have all running with from-image but you need to update to a new image, but you only have dokku commands for deployment. With this, you can make dokcker pull a newer image from a docker registry and run dokku ps:rebuild <app>

## Installation

```
sudo dokku plugin:install https://github.com/grizmio/dokku-docker-deploy-image.git
```

## Commands

```
deploy-image:pull    <image> <app>  Image to pull into <app>
```

## Usage


Dokku will run docker pull <image>
```
dokku deploy-image:pull <image> <app>
```

## Behind the scenes

This command just runs docker commands
