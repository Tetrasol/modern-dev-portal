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
$ cd coqui-dev-portal
$ git clone https://bitbucket client
$ cd default
$ git pull https://bitbucket production
```

{ "keys": ["alt+m"], "command": "markdown_preview", "args": {"target": "browser", "parser":"markdown"} }