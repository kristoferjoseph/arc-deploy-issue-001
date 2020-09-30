Steps to reproduce issue deploying a project with a configured static folder.

1. open app.arc
2. notice the `@static` pragma with a folder set to build
3. leave the app.arc file open
4. on the command line run `npm run deploy`
5. notice the `@static` pragma has been removed during the deploy
6. This causes the deployed app to fail because it is looking in the wrong folder for the needed generated static assets.
