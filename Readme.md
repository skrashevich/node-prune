<img src="http://tjholowaychuk.com:6000/svg/title/NODE/PRUNE">

## What?

node-prune is a small tool to prune unnecessary files from ./node_modules, such as markdown, typescript source files, and so on. Primarily built for [Up](https://github.com/apex/up) which lets you deploy serverless web applications in seconds.

## Installation

From [gobinaries.com](https://gobinaries.com):

```sh
$ curl -sf https://gobinaries.com/skrashevich/node-prune | sh
```

From source:

```
$ go install github.com/skrashevich/node-prune@latest
```

## Usage

In your app directory:

```
$ node-prune

files total 27,330
files removed 3,990
size removed 13 MB
   duration 200ms
```

Somewhere else:

```
$ node-prune path/to/node_modules

files total 27,330
files removed 3,990
size removed 13 MB
   duration 200ms
```

Or add to the ``package.json`` scripts field

```
  "scripts": {
    "postinstall": "node-prune"
  }
```

## Why?

![huge](https://pbs.twimg.com/media/DEIV_1XWsAAlY29.jpg)

---

[![GoDoc](https://godoc.org/github.com/skrashevich/node-prune?status.svg)](https://godoc.org/github.com/skrashevich/node-prune)
![](https://img.shields.io/badge/license-MIT-blue.svg)
![](https://img.shields.io/badge/status-stable-green.svg)

<a href="https://apex.sh"><img src="http://tjholowaychuk.com:6000/svg/sponsor"></a>
