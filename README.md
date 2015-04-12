Modern Development Org
======================
projectID: coqui-dev-portal

## Backlog
* [KanbanFlow](https://kanbanflow.com)

## Environment Installation and Set up
You will need various tools to get started with development. Below are the links to the tools to be installed in sequence.

* [Git](http://git-scm.com/)
* [Python](https://www.python.org/) - use version 2.7.x (2.7.8 preferred)
* [Google Cloud SDK](https://cloud.google.com/sdk/)
    - `$ gcloud auth login`
    - `$ gcloud config set project coqui-dev-portal`
    - Install components with `$ gcloud components update`
        + pkg-python
        + gae-python
        + app-engine-python
        + alpha, beta, app, preview (optional)
* [Node.js](https://nodejs.org/)
    - https://www.digitalocean.com/community/tutorials/how-to-install-node-js-on-an-ubuntu-14-04-server
    - `$ curl -sL https://deb.nodesource.com/setup | sudo bash -`
    - `$ sudo apt-get install nodejs`
    - `sudo apt-get install npm`
    - `sudo apt-get install build-essential libssl-dev`
    - [Bower](http://bower.io/) `$ npm install -g bower`
        + [AngularJS](https://angularjs.org/)
        + [Angular Material](https://material.angularjs.org/)
        + []()
    - [Gulp](http://gulpjs.com/) `$ npm install -g gulp`
    - [Yeoman](http://yeoman.io/) `$ npm install -g yo`
    - [Ng-Poly Generator](https://github.com/dustinspecker/generator-ng-poly) `npm install -g generator-ng-poly`

## Installing Dependencies and Libraries
From within your project directory run the commands below to get started.
(assuming $HOME/ModernDev/ is the active workspace) 

``` 
# Clone the repositories
$ gcloud init coqui-dev-portal

## these steps might not be needed - need to confirm
$ cd coqui-dev-portal
$ git clone https://bitbucket client
$ cd default
$ git pull https://g0r1v3r4@bitbucket.org/moderndev/portal.git
```

{ "keys": ["alt+m"], "command": "markdown_preview", "args": {"target": "browser", "parser":"markdown"} }

## Working with the repository
* Make a new branch every time using `$ git checkout -b <nameofbranch>`
* When finished working with the branch push the code to Bitbucket
* Creat pull request to `master` when ready to push changes to production

## Working with the development Server for app engine and deploy
+ `$ gcloud preview app run <nameofdirectory>` will run the dev server for `localhost` testing
+ `$ gcloud preview app deploy <nameofdirectory` will deploy the branch to app engine instance