# Yarn workspaces monorepo example

This is an example monorepo that uses Yarn workspaces. There are two workspaces in the repo: `workspace-a`, and `workspace-b`. Both workspaces start HTTP servers using `yarn serve`, each returning different responses.

1. Start at the repo root
1. Run `yarn install` to install all dependencies
1. Change into either workspace directory:
    * `cd workspace-a`; or
    * `cd workspace-b`
1. Start the server: `yarn serve`