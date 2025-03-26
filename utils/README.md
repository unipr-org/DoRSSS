# Guide to the utils folder

This directory contains tools/scripts that will could be useful during the course.

```bash
.
├── README.md
└── utils
    ├── docker
    │   ├── docker-compose.yml
    │   ├── Dockerfile
    │   └── pip-requirements.txt
    └── README.md
```

## Docker

The docker folder contains a `Dockerfile`, `pip-requirements.txt` and `docker-compose.yml` files.
This files will allow you to create a container with all the dependencies needed to compile and run the project
created in this course.

### Setup

Supposing that your project is called `Isolette` and is located in a folder called `project` you have to copy the files from the `docker` folder to the `project` folder. At the end you must have the following structure:

```bash
project/
├── Dockerfile
├── docker-compose.yml
├── pip-requirements.txt
└── Isolette/
```

### Build

```bash
docker compose build --no-cache
```

### Run

```bash
docker compose run --rm isolette bash
```
