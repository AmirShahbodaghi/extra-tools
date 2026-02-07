# Swagger API Project

This repository contains a Swagger (OpenAPI) specification for documenting and testing REST APIs, along with a Docker Compose setup to run Swagger UI locally.

## Project Structure

```text
.
├── docker-compose.yml   # Docker Compose configuration to run Swagger UI
├── swagger.yaml         # OpenAPI (Swagger) specification file
└── README.md            # Project documentation
```

## Overview

This project is designed to:

 Define REST APIs using OpenAPI (Swagger) 
 Visualize and test APIs using Swagger UI
 Run everything locally using Docker Compose

## Prerequisites

Make sure you have the following installed on your system:

 [Docker]
 [Docker Compose]

### Start Swagger UI Using Docker Compose

```bash
docker-compose up -d
```

This will start Swagger UI in detached mode.

### 3️⃣ Access Swagger UI

Open your browser and navigate to:

```
http://localhost:8080
```

Swagger UI will automatically load the `swagger.yaml` file.

## Swagger Specification

The API definition is written in **OpenAPI YAML format** inside:

```
swagger.yaml
```

## Docker Compose Details

The `docker-compose.yml` file:

 Uses the official **swaggerapi/swagger-ui** image
 Mounts `swagger.yaml` into the container
 Exposes Swagger UI on port **8080**

## Stopping the Application

To stop and remove containers:

```bash
docker-compose down
```
