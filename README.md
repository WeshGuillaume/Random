<br>
<p align="center"><a href="#" target="_blank"><img width="250"src="https://raw.githubusercontent.com/GuillaumeBadi/Random/master/Logo.png?token=AGQURskZ1M9E4ghdsXYOEpQSIOVMiCfMks5Wl7MawA%3D%3D"></a></p>

<p align="center">
  <a href="https://travis-ci.org/mailjet/mailjet-apiv3-python"><img src="https://travis-ci.org/mailjet/mailjet-apiv3-python.svg?branch=master" alt="travis"></a>
</p>

<p align="center">
<br>
|
<b><a href="#introduction"> Introduction </a></b>|
<b><a href="#installation"> Installation </a></b>|
<b><a href="#usage"> Usage </a></b>|
<b><a href="#tryitlive"> Plugins </a></b>|
<b><a href="#contribute"> Contribute </a></b>|

</p>
<br>

---

# Introduction

MJML is a markup language designed to reduce the pain of coding a responsive email. Its semantic syntax makes it easy and straightforward while its rich standard components library fastens your development time and lightens your email codebase. MJML’s open-source engine takes care of translating the MJML you wrote into responsive HTML.

<br>
<p align="center"><a href="#" target="_blank"><img width="75%"src="https://raw.githubusercontent.com/GuillaumeBadi/Random/master/Editor%20with%20shadow.png?token=AGQURlK4wYL5kH7LwhgOXvel61r6CIj9ks5Wl7OZwA%3D%3D"></a></p>

<br>
# Installation (not available yet)

> via NPM

<p align="right"><a href="#" target="_blank"><img width="30"src="https://www.npmjs.com/static/images/npm-logo.svg"></a></p>

``` bash

npm install -g mjml

```

> via Homebrew

<p align="right"><a href="#" target="_blank"><img width="30"src="https://upload.wikimedia.org/wikipedia/commons/thumb/1/1f/Emoji_u1f37a.svg/2000px-Emoji_u1f37a.svg.png"></a></p>

``` bash

brew install mjml

```
<br>
# Usage

### Command line

> Compile the file and output the result in `a.html`

``` bash

$> mjml input.mjml

```

> Redirect the result to a file

``` bash

$> mjml input.mjml -o output.html

```

> Watch a file and compile every time the file changes

``` bash

$> mjml -w input.mjml -o output.html

```

<br>
### Inside NodeJs

``` javascript

import mjml, { watch, compile } from 'mjml'

/*
  Takes a file and compile it using the provided options
*/
compile('input.html', {output: 'output.html', minify: true})

/*
  Takes a file and call compile on each change
*/
watch('input.mjml', {output: 'output.html'})

/*
  Compile an mjml string
*/
const outputString = mjml('mjml code')

```

<br>
# Try it live

<br>

# Contribute

 - [ ] Fork the repository
 - [ ] Code an awesome feature
 - [ ] Make your pull request
 - [ ] Add your github profile here
