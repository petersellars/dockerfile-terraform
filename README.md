# cato1971/terraform [![Circle CI](https://circleci.com/gh/petersellars/dockerfile-terraform.svg?style=svg)](https://circleci.com/gh/petersellars/dockerfile-terraform)

## What is terraform

Terraform provides a common configuration to launch infrastructure — from physical and virtual servers to email and DNS providers. Once launched, Terraform safely and efficiently changes infrastructure as the configuration is evolved.

Simple file based configuration gives you a single view of your entire infrastructure.

[https://www.terraform.io/](https://www.terraform.io/)

## Dockerfile

[**Trusted Build**](https://hub.docker.com/r/cato1971/terraform/)

This Docker image is based on the official [alpine:3.3](https://hub.docker.com/_/alpine/) base image.

## How to use this image

```
docker run cato1971/terraform [--version] [--help] <command> [<args>]

```

## Using

**Please note: Create by your Terraform configuration files (.tf) is `/data` directory**

### terraform apply

```
docker run --rm -v /data:/data cato1971/terraform apply [options]
```

### terraform destroy

```
docker run --rm -v /data:/data cato1971/terraform destroy [options] [DIR]
```

### terraform get

```
docker run --rm -v /data:/data cato1971/terraform get [options] PATH
```

### terraform graph

```
docker run --rm -v /data:/data cato1971/terraform graph [options]
```

### terraform init

```
docker run --rm -v /data:/data cato1971/terraform init [options] SOURCE [PATH]
```

### terraform output

```
docker run --rm -v /data:/data cato1971/terraform output [options] NAME
```

### terraform plan

```
docker run --rm -v /data:/data cato1971/terraform plan [options]
```

### terraform push

```
docker run --rm -v /data:/data cato1971/terraform push [options]
```

### terraform refresh

```
docker run --rm -v /data:/data cato1971/terraform refresh [options]
```

### terraform remote

```
docker run --rm -v /data:/data cato1971/terraform remote [options]
```

### terraform show

```
docker run --rm -v /data:/data cato1971/terraform show terraform.tfstate [options]
```

### terraform taint

```
docker run --rm -v /data:/data cato1971/terraform taint [options] name
```

### terraform version

```
docker run --rm cato1971/terraform version
```
