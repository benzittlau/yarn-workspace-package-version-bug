# Reproduction steps

Install yarn 1.22.22  
Run `yarn install` in the root directory  
Run `yarn run eslint --version` in `src/apps/workspace-a`

Expected:  
$ .../yarn-run-version-debugging/src/apps/workspace-a/node_modules/.bin/eslint --version
v8.57.0 // The version installed in workspace-a

Actual:  
$ .../yarn-run-version-debugging/node_modules/.bin/eslint --version
v7.32.0 // The version in the root node_modules
