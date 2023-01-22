![logo-graphqlana-narrow](https://user-images.githubusercontent.com/38172/213896525-2e0ebc4c-5e19-48a8-800d-03340eea8f34.png)

## Solana's blockchain data for humans

Solana data can be very hard to access and even harder to properly understand.

This has been the main drive behind the recent surge of services that are trying to democratise the access to that data through their APIs.

**GraphQLana** builds on top of those services and uses the power of GraphQL to create a human-friendly interface for on-chain data that can be used by technical and (more importantly) non-technical people.

## Features

### Seamlessly combine multiple sources of data

Stop worrying about fetching data from multiple endpoints and stitching that all back together. With **GraphQLana** you get access to the top sources of data from Solana's blockchain without even knowing it.

Focus on the data that you want, and let us do all the work behind the scenes.

### Get exactly the data that you need and nothing else

Why have to parse all the data if you just need a small sample? And what about having to fetch that additional data that didn't come in the first request?

With **GraphQLana** there's no extra data or missing fields, you get **exactly** what you want. We wish we could take the credits for that but it's just one of the benefits of using GraphQL.

### Quickly iterate in the online explorer

You don't need to setup a project or download an app to get started. Just hop into our online playground and start exploring the data!

Start with a small query and build on top of that. When you're happy with the data, use that query in your application and create something amazing with it!

### Discover the unknown with the integrated documentation

Looking for the documentation? Well with GraphQL everything is self-documented! We take advantage of GraphQL's declarative nature and

No more wasted time going through the docs to see how to use a given API, using **GraphQLana** will feel natural to you.

## Getting started

TBA

## Supported data sources

We're constantly improving the access to on-chain data through our supported services and currently support these sources:

-   [Helius](https://helius.xyz/)
-   [Shyft](https://shyft.to/)
-   [Hyperspace](https://hyperspace.xyz/)
-   [Jupiter](https://jup.ag/)

**GraphQLana** doesn't expose all of these API's endpoints in our schema, the intention isn't to create a simple 1-to-1 match with each API but to curate a more human-readable schema that makes it easier to navigate through the data.

## Schema

**GraphQLana** is mainly focused on user-centered data so we define most of our queries based on a given wallet or set of wallets.

For that reason, the main query is the `account` query, although it also exposes a bunch of other queries to access a particular subset of the data.

From the account query it's possible to find information about a token balances, associated .sol domains, transactions and existing NFTs. There are many layers of data to explore for each of these fields and we're regularly improving the existing queries so the best option is to use our online playground and see the data that we can fetch.

## Technologies

### [StepZen](https://stepzen.com/) GraphQL framework

GraphQLana use StepZen as its core GraphQL framework, using a low-code approach with the benefits of the declarative nature of GraphQL.

This makes it very easy to extend and very accessible to new contributors, which is one of the main reason why StepZen was chosen.

One of the core objective of this project is to make data more accessible and we want to extend that to our codebase as well.

### [Stellate](https://stellate.co/) GraphQL CDN

Even though StepZen already provides a bunch of optimizations out of the box, we use Stellate for our public-facing GraphQL endpoint so we get advanced caching optimizations and usage metrics.

This is an amazing service that makes queries to GraphQLana as fast as possible and improves the developer experience of those using our endpoint.
