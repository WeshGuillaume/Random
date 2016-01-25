MJML Engine
===========

The `mjml-engine` is the core of the MJML renderer. It exposes the MJML parser and the MJML-to-HTML transpiler.

## How it works

(how it works image)

The engine is composed of multiple parts:
	- [`documentParser`](#) : Parse the markup MJML string and return a JSON representation
	- [`mjml2html`](#) : Turn a JSON MJML representation and returns an HTML string using react components
	- [`MJMLElementsCollection`](#) : Contains the standard MJML elements exposed to the API

## Changelog
Please refer to the [release](#) section to get more details about the diferent improvements

## Issues

Please make sure to check the closed issue and to tag your issues with the `engine`  tag
