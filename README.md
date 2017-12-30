# Source for http://arvidl.github.io
This repository contains the source for my Computational Medicine blog http://arvidl.github.io/.
Based on: git clone https://github.com/jakevdp/jakevdp.github.io-source.git

## Building the Blog

Clone the repository & make sure submodules are included

```
$ git clone https://github.com/arvidl/arvidl.github.io-source.git
$ git submodule update --init --recursive
```

Install the required packages:

```
$ conda create -n pelican-blog python=3.5 jupyter notebook
$ source activate pelican-blog
$ pip install pelican Markdown ghp-import
```

Build the html and serve locally:

```
$ make html
$ make serve
$ open http://localhost:8000
```

Deploy to github pages

```
$ make publish-to-github
```
