# Laravel & Vue Docker template

Basic template for Laravel project with Vue in Docker container

## Prerequisites

- [Docker](https://www.docker.com/get-started/)

## Installation

### 1. Create .env file and fill env variables

- Copy the `.env.example` file and rename it to `.env`.

  ```shell
  cp .env.example .env
  ```

### 2. Build the images run containers

- Open terminal in the project root folder and run:

  ```shell
  docker compose up --build
  ```

  The `--build` option forces docker to rebuild the images in case they were already built and are cached.

### 3. Run database migrations

  ```shell
  docker compose run app php artisan migrate
  ```
  
## Development

### 1. Run containers

- Open terminal in the project root folder and run:

  ```shell
  docker compose up
  ```
