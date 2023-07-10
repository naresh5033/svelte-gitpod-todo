# Full Stack Web Development in the Cloud

This repository contains the source code for the Full Stack Web Development in the Cloud.


## Architecture

The diagram below outlines the high-level architecture and the hosting providers for the web application, API and database.

![image](https://user-images.githubusercontent.com/788827/145879564-e7dc42d6-3055-492b-95d7-902e9a5fad96.png)

## Ephemeral developer environments (GitPod)

- with gitpod we can spin up fresh, automated our dev environments, for each task in the cloud, in seconds.

The entire course is developed using [Gitpod](https://www.gitpod.io/). For each task, we use an ephemeral developer environment that we dispose of as soon as the task is completed. Environments are fully automated and we never run `npm install` or `npm run dev` manually. We also don't have any code, dependencies, etc installed locally.

## Technology stack

The course leverages the following technologies.

**Web application**

[Svelte](https://svelte.dev/) is a compiler to develop highly performant web applications with great developer experience. The application is styled with plain CSS.

**API**

[SvelteKit](https://kit.svelte.dev/) is the library & application framework powered by Svelte. It provides routing, server-side rendering and also enables us to develop a web application that works if Javascript is disabled.

[Prisma](https://www.prisma.io/) is the object-relational mapping (ORM) library that let's us interact with the database. Based on models we define, Prisma generates the database schema and keeps the databsae in sync with our model(s). In addition, it generates a Typescript client we import into our code so that we have type safety when we work with database objects.

**Database**

[Postgres](https://www.postgresql.org/) is our database of choice for the course. However, thanks to Prisma's support for various other databases, it is a matter of changing configuration values to leverage a different database.

**Deployment**

The web application and API are hosted on [Vercel](https://vercel.com/) whereas the database lives on [Railway](https://railway.app/).

