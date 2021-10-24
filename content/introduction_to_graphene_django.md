title: What is Graphene?
date: 2021-10-23 22:00
slug: how-to-become-senior-software-developer
summary: Graphene is a library that provides tools to implement a GraphQL API in Python using a code-first approach.

### Introduction
## What is GraphQL?
- GraphQL is a query language for your API.

- **It provides a standard way to:

describe data provided by a server in a statically typed Schema
request data in a Query which exactly describes your data requirements and
receive data in a Response containing only the data you requested.
For an introduction to GraphQL and an overview of its concepts, please refer to the official GraphQL documentation.

## What is Graphene?
Graphene is a library that provides tools to implement a GraphQL API in Python using a code-first approach.

Compare Graphene’s code-first approach to building a GraphQL API with schema-first approaches like Apollo Server (JavaScript) or Ariadne (Python). Instead of writing GraphQL Schema Definition Language (SDL), we write Python code to describe the data provided by your server.

Graphene is fully featured with integrations for the most popular web frameworks and ORMs. Graphene produces schemas that are fully compliant with the GraphQL spec and provides tools and patterns for building a Relay-Compliant API as well.

## An example in Graphene
Let’s build a basic GraphQL schema to say “hello” and “goodbye” in Graphene.

When we send a Query requesting only one Field, hello, and specify a value for the name Argument...

{
  hello(name: "friend")
}


...we would expect the following Response containing only the data requested (the goodbye field is not resolved).

{
  "data": {
    "hello": "Hello friend!"
  }
}

<div><a href="https://docs.graphene-python.org/projects/django/en/latest/" rel="lightbox" title="django">for more..</div>
