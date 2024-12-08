# Simple GraphQL API with Apollo Server in Docker

A simple GraphQL API using Apollo Server, dockerized for easy execution in any environment.

## Description

This is a basic Node.js program using Apollo Server. The application exposes a GraphQL API with a single query (hello) that responds with a greeting message when accessed via a GET or POST request.

## Technologies Used

- Node.js
- Apollo Server
- GraphQL
- Docker

## Prerequisites

To run this project, you need to have Docker installed on your machine. If you don't have it, you can download it from [here](https://www.docker.com/products/docker-desktop).

## Instructions to Run the Project

1. **Clone this repository:**

   If you haven't cloned the repository yet, you can do so with the following command:

   ```bash
   git clone git clone https://github.com/your_username/graphql-api.git

2. **Build the Docker image:**

   Before running the container, build the Docker image using the following command:

   ```bash
   docker build -t ksrobalino/graphql-api:v1 .

3. **Push the image to Docker Hub (if needed):**

   If you'd like to upload the image to Docker Hub for others to use, you can do so with:

   ```bash
   docker push ksrobalino/graphql-api:v1

4. **Run the Docker container:**

   After building the image, run the container with the following command:

   ```bash
   docker run -d -p 4000:4000 --name graphql_container ksrobalino/graphql-api:v1

5. **Access the application:**

   Once the container is running, you can access the API in your browser or with tools like Postman, at the following URL:
   ```bash
   http://localhost:4000
   
   You can use a GraphQL client like [GraphiQL](https://www.electronjs.org/apps/graphiql) or [Postman](https://www.postman.com/) to interact with the API.

### Query example:

```graphql
{
  hello
}
