# hackernews-graphql-js

This repository contains the final project for the [**GraphQL.js tutorial**](https://www.howtographql.com/graphql-js/0-introduction/) on [How to GraphQL](https://www.howtographql.com/). Note that it also serves as foundation for all frontend tutorials on the site.

For the backend in this tutorial we’ll simply use the final project from the [Node tutorial] (https://www.howtographql.com/graphql-js/0-introduction).
Run this code to generate Server: `curl https://codeload.github.com/howtographql/react-apollo/tar.gz/starter | tar -xz --strip=1 react-apollo-starter/server`
The command above will generate `server` directory with the code needed for our backend.

- prisma: This directory holds all the files that relate to our Prisma setup. Prisma Client is used to access the database in our GraphQL resolvers (similar to an ORM).

  - schema.prisma defines our data model for the project. It uses the Prisma Schema Language to define the shape of our databases tables and the relations between them.
  - dev.db is a SQLite database that will be used to store and retrieve data for this tutorial

- src: This directory holds the source files for our GraphQL server.

  - schema.graphql contains our application schema. The application schema defines the GraphQL operations we can send from the frontend. We’ll take a closer look at this file in just a bit.
  - resolvers contains the resolver functions for the operations defined in the application schema.
  - index.js is the entry point for our GraphQL server.
