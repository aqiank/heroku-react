# Heroku React
This is a template for creating and deploying static React website on Heroku.

## Development
1. Run `npm install`
2. Run `./babel.sh` and `./webpack.sh`

## Deploying to Heroku
Here are some steps to deploy your static site to Heroku:
1. Create your Heroku app.
`heroku create --remote staging`

2. Add NodeJS buildpack.
`heroku buildpacks:set heroku/nodejs`

3. Push to Heroku. Make sure you've already commited the code you want in Git.
`git push staging master`

3a. Use the following command if you have different local branch name (e.g. `jane` not `master`).
`git push staging jane:master`
