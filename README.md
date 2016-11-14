# Nebulis Website [![Standard - JavaScript Style Guide](https://img.shields.io/badge/code%20style-standard-brightgreen.svg)](http://standardjs.com/)


> **GENERAL NOTE**
>
> * Production server is running Dokku for deployment
> * Keep `nodemon.example.json` in sync with `nodemon.json`
> * To add team member's information, just edit [team.json](./team.json) file
> * Do run `npm test` before sending PR or merging your commits


## Contributing

Do not push directly to master. Instead fork the repo, commit any changes and send a pull request.

## Setup

    git pull git@github.com:nebulis-io/website.git
    cd website
    npm run setup


## Configuration

    cp nodemon.example.json nodemon.json

Edit `nodemon.json` file and add `MONGO_URL` and `YAR_PASSWORD`.


## Run it locally

    npm run dev

Visit http://localhost:8000

## Deploying

The Nebulis site uses Dokku for automatic deployment. If you have write access to nebulis-io/master, add the dokku deployer locally via:

	git remote add dokku dokku@nebulis.io:nebulis-website

Then push it with the following command:

	git push dokku master

This will automatically update the website on the server.
