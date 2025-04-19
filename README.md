# Fluent Bit playground

A simple playground setup to explore Fluent Bit with Elasticsearch.

## Prerequisites

Make sure you have **Docker Compose** installed before starting.

## Setup

Clone the repository:
```shell
git clone git@github.com:g-svitelskyi/fluent-bit-playground.git
cd fluent-bit-playground
```

Start the application:
```shell
docker compose up -d
```

## Accessing Kibana

Once the containers are up, open your browser and navigate to: http://localhost:5601

Log in using the default credentials:
- Username: `elastic`
- Password: `elastic`

## Running Elasticsearch queries

After logging into Kibana, go to the Dev Tools section and open the Console.

Search for all documents:
```
GET /_search
```

## Cleanup

To stop the containers and remove associated volumes, run:

```shell
docker compose down -v
```
