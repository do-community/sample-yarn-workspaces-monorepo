# Yarn workspaces monorepo example

This is an example monorepo that uses Yarn workspaces. There are two workspaces in the repo: `workspace-a`, and `workspace-b`. Both workspaces start HTTP servers using `yarn serve`, each returning different responses.

## Local Testing

1. Start at the repo root
1. Run `yarn install` to install all dependencies
1. Change into either workspace directory:
    * `cd workspace-a`; or
    * `cd workspace-b`
1. Start the server: `yarn serve`

## Deploying to App Platform

1. Select your git repo
1. Keep the source directory set to the default, `/`
1. If you have a build script in `package.json`, set the build command to:
    ```
    cd workspace-b
    yarn build
    ```
1. Set the run command to:
    ```
    cd workspace-b
    yarn serve
    ```
