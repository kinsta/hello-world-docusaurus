![Photo by Milad Fakurian on Unsplash](https://user-images.githubusercontent.com/2342458/197758905-c9019919-e9fa-4001-8561-089c794dfd83.png)
# Kinsta - Hello World - Docusaurus Test

An example of how to deploy a static site built with **Docusaurus** on Kinsta App Hosting services.

> Kinsta’s Application Hosting is a service to run your web apps and any databases side by side in a hassle-free environment, tailored for developer needs and ease of use. App Hosting is currently in an invite-only beta phase, sign up for a test account at [kinsta.com/application-hosting](https://kinsta.com/application-hosting/).

## Dependency Management

During the deployment process Kinsta will automatically install dependencies defined in your `package.json` file.

## Web Server Setup

### Port

Kinsta automatically sets the `PORT` environment variable. You should **not** define it yourself and you should 
**not** hard-code it into the application. The `serve` package utilizes the port set by Kinsta automatically.

### Start Command

When deploying an application Kinsta will automatically create a web process with `npm start` as the entry point. Make sure to use this command to run your server.

## Deployment Lifecycle

Whenever a deployment is initiated (through creating an application or re-deploying due to an incoming commit) the `npm build` command is run, followed by the `npm start` command.

## What is Docusaurus
[Docusaurus](https://docusaurus.io/) is a tool designed to make it easy for teams to publish documentation websites without having to worry about the infrastructure and design details. At its core, all a user has to provide are documentation files written in Markdown, customization of a provided home page written in React, and a few configuration modifications.

More info on the [Docusaurus](https://docusaurus.io/) website.
