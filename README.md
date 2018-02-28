# Dockerfiles for developing with the serverless framework, AWS lambda and node.js or python

The resulting docker images provide

- nodejs
- python
- npm
- aws cli
- serverless

## Configure AWS CLI

To deploy your app you need to have AWS CLI configured. The configuration and the credentials are stored at `/root/.aws` inside the container, so you might want to define a volume for that path.

If you don't have configuration and credentials already on your host machine that you want to make accessible from inside the container, run (inside the container)
```sh
$ aws configure
```
to create it.
