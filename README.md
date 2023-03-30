![Photo by Milad Fakurian on Unsplash](https://user-images.githubusercontent.com/2342458/197758905-c9019919-e9fa-4001-8561-089c794dfd83.png)
# Kinsta - Hello World - Docusaurus 

An example of how to deploy a static site built with **Docusaurus** on Kinsta App Hosting services.

---
Kinsta is a developer-centric cloud host / PaaS. We’re striving to make it easier for you to share your web projects with your users. Focus on coding and building, and we’ll take care of deployment and provide fast, scalable hosting. + 24/7 expert-only support.

- [Start your free trial](https://kinsta.com/signup/?product_type=app-db)
- [Application Hosting](https://kinsta.com/application-hosting)
- [Database Hosting](https://kinsta.com/database-hosting)

## Dependency Management

Kinsta automatically installs dependencies defined in your `package.json` file during the deployment process.

## Web Server Setup

### Port

Kinsta automatically sets the `PORT` environment variable. You should **not** define it yourself and you should 
**not** hard-code it into the application. The `serve` package utilizes the port set by Kinsta automatically.

### Start Command

When deploying an application, Kinsta automatically creates a web process with `npm start` as the entry point. Make sure to use this command to run your server.

## Deployment Lifecycle

Whenever a deployment is initiated (through creating an application or re-deploying due to an incoming commit) the `npm build` command is run, followed by the `npm start` command.

## What is Docusaurus
[Docusaurus](https://docusaurus.io/) is a static-site generator specializing in producing documentation websites that are simple to build with minimal coding experience required so you can use it out of the box. More information is available on the [Docusaurus](https://docusaurus.io/) website.
