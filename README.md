# Apigee-ApiHub-Simple-Github-Pipeline

**This is not an official Google product.**<BR>This implementation is not an official Google product, nor is it part of an official Google product. Support is available on a best-effort basis via GitHub.

***

## Goal

Simple implementation of a CI/CD pipeline for Apigee using GitHub repository, 
[CI/CD with GitHub](https://docs.GitHub.com/ee/ci/introduction/) and Apigee Maven Plugins.

![GitHub CICD Pipeline overview](./images/project.jpg)<BR>

### The CICD pipeline includes:

- An Apigee proxy to be deployed in Apigee X/hybrid (Edge/OPSK not supported)
    - Integration testing of the deployed proxy using
    [apickli](https://github.com/apickli/apickli)
    - Packaging and deployment of an Apigee configuration using
    [Apigee Config Maven Plugin](https://github.com/apigee/apigee-config-maven-plugin)
    - Packaging and deployment of the API proxy bundle using
    [Apigee Deploy Maven Plugin](https://github.com/apigee/apigee-deploy-maven-plugin)

- A corresponding API specification file (OAS, Open Api Specification) to be deployed in Apigee APi Hub
    - Publication of the API into Apigee Api Hub using
    [Apigee Registry Maven Plugin](https://github.com/apigee/apigee-registry-maven-plugin)


## Work in Progress...

Demo scenario

  - Step 1   (main branch): deploy API Proxy and create API v1 into Apigee API Hub
  - Step 1.1 (main branch): deploy new API Proxy release with no change on API Specification
  - Step 2   (main branch): deploy new API Proxy release and publish API v1.1 into Apigee API Hub
  - Step 3   (main branch): publish API v2 into Apigee API Hub, in "Design" Status
