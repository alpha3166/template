# Usage

## Setup

Replace UID (`1000`) and GID (`1000`) in `Dockerfile` with yours.

## With Docker

To build image:

    docker build -t template-dev .

To start shell:

    docker run -it --rm -v $PWD/../..:/template -w /template template-dev

## With Docker Compose

To start shell:

    docker compose run --rm ws
