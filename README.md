<br>
<p align="center"><a href="#" target="_blank"><img width="250"src="https://bitbucket.mailjet.com/projects/DEVREL/repos/mjml/browse/assets/Logo.png?at=c81cd1a829fa5ca36d0eb033735d3eaf9a7afa6f&raw"></a></p>

<p align="center">
  <a href="https://travis-ci.org/mailjet/mailjet-apiv3-python"><img src="https://travis-ci.org/mailjet/mailjet-apiv3-python.svg?branch=master" alt="travis"></a>
</p>

<p align="center">
<br>
|
<b><a href="#introduction">Introduction</a></b>|
<b><a href="#installation">Installation</a></b>|
<b><a href="#usage">Usage</a></b>|
<b><a href="#tryitlive">Plugins</a></b>|
<b><a href="#contribute">Contribute</a></b>|

</p>
<br>

---

# Introduction

MJML is a markup language designed to reduce the pain of coding a responsive email. Its semantic syntax makes it easy and straightforward while its rich standard components library fastens your development time and lightens your email codebase. MJML’s open-source engine takes care of translating the MJML you wrote into responsive HTML.


<br>
# Installation (not available yet)

``` bash
# via NPM
npm install -g mjml

# via Bower
bower install mjml

# via Homebrew
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
