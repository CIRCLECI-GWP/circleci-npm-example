# circleci-npm-example

Example npm package for the CircleCI tutorial
[Publishing npm packages with CircleCI](https://circleci.com/blog/publishing-npm-packages-using-circleci-2-0/).

CircleCI tests every commit. When you push a version tag such as `v0.1.1`, it
publishes the package to npm with
[npm trusted publishing](https://docs.npmjs.com/trusted-publishers) (OIDC), so
no npm token is stored in CircleCI.

## Run the tests

    npm ci
    npm test

## Use it for your own package

1. Fork this repository and set the fork up as a project in CircleCI.
2. In `package.json`, change `name` to a name you own, for example
   `@your-npm-username/circleci-npm-example`, and change `repository.url` to
   your fork.
3. Follow the tutorial to publish the first version and set up trusted
   publishing.
