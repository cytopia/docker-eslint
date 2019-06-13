# Docker image for `eslint`

[![Build Status](https://travis-ci.com/cytopia/docker-eslint.svg?branch=master)](https://travis-ci.com/cytopia/docker-eslint)
[![Tag](https://img.shields.io/github/tag/cytopia/docker-eslint.svg)](https://github.com/cytopia/docker-eslint/releases)
[![](https://images.microbadger.com/badges/version/cytopia/eslint:latest.svg)](https://microbadger.com/images/cytopia/eslint:latest "eslint")
[![](https://images.microbadger.com/badges/image/cytopia/eslint:latest.svg)](https://microbadger.com/images/cytopia/eslint:latest "eslint")
[![](https://img.shields.io/badge/github-cytopia%2Fdocker--eslint-red.svg)](https://github.com/cytopia/docker-eslint "github.com/cytopia/docker-eslint")
[![License](https://img.shields.io/badge/license-MIT-%233DA639.svg)](https://opensource.org/licenses/MIT)

> #### All awesome CI images
>
> [ansible](https://github.com/cytopia/docker-ansible) |
> [ansible-lint](https://github.com/cytopia/docker-ansible-lint) |
> [awesome-ci](https://github.com/cytopia/awesome-ci) |
> [eslint](https://github.com/cytopia/docker-eslint) |
> [jsonlint](https://github.com/cytopia/docker-jsonlint) |
> [terraform-docs](https://github.com/cytopia/docker-terraform-docs) |
> [yamllint](https://github.com/cytopia/docker-yamllint)


View **[Dockerfile](https://github.com/cytopia/docker-eslint/blob/master/Dockerfile)** on GitHub.

[![Docker hub](http://dockeri.co/image/cytopia/eslint)](https://hub.docker.com/r/cytopia/eslint)

Tiny Alpine-based multistage-build dockerized version of [eslint](https://github.com/eslint/eslint)<sup>[1]</sup>.
The image is built nightly against multiple stable versions and pushed to Dockerhub.

<sup>[1] Official project: https://github.com/eslint/eslint</sup>


## Available Docker image versions

| Docker tag | Build from |
|------------|------------|
| `latest`   | [Branch: master](https://github.com/eslint/eslint) |
<!--
| `1.6.0`    | [Tag: v1.6.0](https://github.com/zaach/eslint/tree/v1.6.0) |
| `1.5.0`    | [Tag: v1.5.0](https://github.com/zaach/eslint/tree/v1.5.0) |
| `1.4.1`    | [Tag: v1.4.1](https://github.com/zaach/eslint/tree/v1.4.1) |
| `1.4.0`    | [Tag: v1.4.0](https://github.com/zaach/eslint/tree/v1.4.0) |
| `1.3.2`    | [Tag: v1.3.2](https://github.com/zaach/eslint/tree/v1.3.2) |
| `1.2.0`    | [Tag: v1.2.0](https://github.com/zaach/eslint/tree/v1.2.0) |
| `1.1.1`    | [Tag: v1.1.1](https://github.com/zaach/eslint/tree/v1.1.1) |
| `1.1.0`    | [Tag: v1.1.0](https://github.com/zaach/eslint/tree/v1.1.0) |
| `1.0.1`    | [Tag: v1.0.1](https://github.com/zaach/eslint/tree/v1.0.1) |
-->


## Docker mounts

The working directory inside the Docker container is **`/data/`** and should be mounted locally to
where your `.eslint` config file is located.


## Usage

#### Lint JS files
```bash
$ docker run -it --rm -v $(pwd):/data cytopia/eslint .

/data/index.js
  3:1  error  Parsing error: The keyword 'const' is reserved

✖ 1 problem (1 error, 0 warnings)
```

## License

**[MIT License](LICENSE)**

Copyright (c) 2019 [cytopia](https://github.com/cytopia)
