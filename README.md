<p align="center">
  <a href="www.blaugame.com">
    <img alt="Screenshot" src="docs/images/screenshot.png" width="500px">
  </a>
</p>

<p align="center">
  Blau Game official website.
</p>

<p align="center">

  <a href=""><img alt="Build Status" src=""></a>

  <a href="https://travis-ci.org/xablauger-studios/blau-site"><img alt="Build Status" src="https://travis-ci.org/xablauger-studios/blau-site.svg?branch=master"></a>

  <a href="https://codeclimate.com/github/mabrasil/flat-palettes"><img alt="Code Climate" src="https://codeclimate.com/github/xablauger-studios/blau-site/badges/gpa.svg"/></a>

  <a href="https://david-dm.org/xablauger-studios/blau-site" title="Dependency status"><img src="https://david-dm.org/xablauger-studios/blau-site.svg"/></a>

  <a href="https://david-dm.org/xablauger-studios/blau-site#info=devDependencies" title="devDependency status"><img src="https://david-dm.org/xablauger-studios/blau-site/dev-status.svg"/></a>

</p>

## Table of Contents

- [The Game](#the-game)
- [Usage](#usage)
- [How it works?](#how-it-works)
- [Contributing](#contributing)
- [License](#license)
- [Credits](#credits)

## The Game

<p align="center">
  <a href="https://itunes.apple.com/br/app/blau/id1150066458">
    <img alt="Logo" src="docs/images/logo.png" width="350px">
  </a>
</p>

**blau** is game where your goal is the simplest possible one: get to the end 
of each level. How? By guiding blau - actually, an abstract black circle - 
through many simple - yet elegant - puzzles, avoiding physics-based traps and collecting shapes; to every level, there are many solutions, which go from beautifully simple to deep and complex ones - **it all starts with a gesture, 
then evolves with physics, but the end is up to you**.

[Download it now here](https://itunes.apple.com/br/app/blau/id1150066458)
[Official game teaser](https://www.youtube.com/watch?v=kNVg4-tiJzA)

## Usage

### Getting Started

Make sure you have the main dependencies:

- [Git](http://git-scm.com/downloads)
- [NodeJS](http://nodejs.org/)

Clone this repository:

```sh
$ git clone https://github.com/xablauger-studios/blau-site.git
```

Install all dependencies:

```sh
$ cd blau-site
$ npm install
```

### Structure

If everything from the [Getting Started](#getting-started) section goes well, you should have this:

```
|-- docs/
|-- src/
|   |-- images/
|   |-- scripts/
|   |-- styles/
|   |-- templates/
|   |-- vendor/
|   |-- videos/
|   |-- config.json
|   |-- manifest.json
|-- tasks/
|   |-- deploy/
|       |-- gh-pages.js
|   |-- templates/
|       |-- compiler.js
|-- .babelrc
|-- .bowerrc
|-- .editorconfig
|-- .eslint
|-- .gitignore
|-- .styluslintrc
|-- .travis.yml
|-- bower.json
|-- package.json
|-- [...]
```

### Customization

For most of the updates/changes in our page, just go to the 
[`config.json`](/src/config.json) file and change the value of variables.

#### Basic Information About The Game

Here goes the app basic data - which is used, for example, to feed the page
metadata.

```json
"about":{
  "title":"Blau Game",
  "description":"It all starts with a gesture, then evolves with physics, but the end is up to you.",
  "author":"Xablauger Software",
  "canonical":"https://blaugame.com",
  "image":"",
  "appleItunesAppID":"1150066458",
  "mobile":{
    "themeColor":"#ffffff"
  },
  "googleAnalytics":{
    "ID":"UA-58120604-9"
  },
  "socialNetworks":[
    {
      "name":"Facebook",
      "ID":"blaugame"
    },
    {
      "name":"Twitter",
      "ID":"blaugame"
    },
    {
      "name":"Instagram",
      "ID":"blaugame"
    },
    {
      "name":"YouTube",
      "ID":"UCT5wWP3UeA7og9CVVz2USgA"
    }
  ]
}
```

#### Players Testimonials

Here goes all the opinions about the game which come from specialist sites/
other players.

```json
{
  "name":"testimonials",
  "shortLabel":"What others say It is",
  "longLabel":"what do other people say blau is?",
  "teamTestimonials":[
    {
      "author":{
        "name":"Matheus Martins",
        "role":"Lead Game Programmer",
        "company":"Blau Game"
      },
      "opinion":"The best game I've ever palyed.",
      "link":"https://blaugame.com"
    }
  ],
  "playersTestimonials":[
    {
      "author":{
        "name":"Press Coordination Office",
        "role":"",
        "company":"IFCE"
      },
      "opinion":"[...]It's a super exciting game[...]",
      "link":"https://www.facebook.com/ifce.campusfortaleza/photos/pb.696732933672509.-2207520000.1476304727./1366599953352467/?type=3&theater"
    }
  ]
}
```