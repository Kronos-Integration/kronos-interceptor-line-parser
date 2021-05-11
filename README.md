[![npm](https://img.shields.io/npm/v/@kronos-integration/interceptor-line-parser.svg)](https://www.npmjs.com/package/@kronos-integration/interceptor-line-parser)
[![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
[![minified size](https://badgen.net/bundlephobia/min/@kronos-integration/interceptor-line-parser)](https://bundlephobia.com/result?p=@kronos-integration/interceptor-line-parser)
[![downloads](http://img.shields.io/npm/dm/@kronos-integration/interceptor-line-parser.svg?style=flat-square)](https://npmjs.org/package/@kronos-integration/interceptor-line-parser)
[![GitHub Issues](https://img.shields.io/github/issues/Kronos-Integration/interceptor-line-parser.svg?style=flat-square)](https://github.com/Kronos-Integration/interceptor-line-parser/issues)
[![Build Status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2FKronos-Integration%2Finterceptor-line-parser%2Fbadge&style=flat)](https://actions-badge.atrox.dev/Kronos-Integration/interceptor-line-parser/goto)
[![Styled with prettier](https://img.shields.io/badge/styled_with-prettier-ff69b4.svg)](https://github.com/prettier/prettier)
[![Commitizen friendly](https://img.shields.io/badge/commitizen-friendly-brightgreen.svg)](http://commitizen.github.io/cz-cli/)
[![Known Vulnerabilities](https://snyk.io/test/github/Kronos-Integration/interceptor-line-parser/badge.svg)](https://snyk.io/test/github/Kronos-Integration/interceptor-line-parser)
[![Coverage Status](https://coveralls.io/repos/Kronos-Integration/interceptor-line-parser/badge.svg)](https://coveralls.io/github/Kronos-Integration/interceptor-line-parser)

# API

<!-- Generated by documentation.js. Update this documentation by updating the source code. -->

### Table of Contents

*   [LineParserInterceptor](#lineparserinterceptor)
*   [Transform](#transform)
*   [constructor](#constructor)
    *   [Parameters](#parameters)
*   [\_transform](#\_transform)
    *   [Parameters](#parameters-1)
*   [\_flush](#\_flush)
    *   [Parameters](#parameters-2)
*   [\_pushLine](#\_pushline)
    *   [Parameters](#parameters-3)

## LineParserInterceptor

**Extends StreamTransformInterceptor**

This interceptor cares about the handling of the messages.
It will add the hops and copies the messages

## Transform

This module reads a stream and split it into lines.
The out put stream will be an object stream

## constructor

Creates the line parser and sets the options.
The following options are supported:
{
"allow_new_line_in_cell" : true,
"line_separator" : "\n",
"quote_char" : '"'
"skip_empty_lines" : true
}

### Parameters

*   `opts`   (optional, default `{}`)

## \_transform

Reads the stream data and split it into lines.

### Parameters

*   `data`  
*   `enc`  
*   `cb`  

## \_flush

Returns the rest as line

### Parameters

*   `cb`  

## \_pushLine

Pushes a line object onto the stream

### Parameters

*   `data`  
