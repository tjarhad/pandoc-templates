
# Pandoc markdown template

### Contributing

1. Create or Edit *.md file in `chapters` folder using [Markdown](https://en.wikipedia.org/wiki/Markdown) syntax
2. `img` folders contains images


#### Compiling document 

Prerequisite: Install docker on system. We will be using `pandoc/latex:latest` docker image to build pdf from markdown.

1. Pull Docker image
```bash
make pull-docker-image
```

2. Generate PDF
```bash
make docker-build-pdf
```

### Pandoc 

* `metadata.yml` file contains pandoc variables. This includes report title, subtitle, etc.
* `page.tex` is custom made latex template for cover page. You can refer [default latex](https://github.com/jgm/pandoc-templates/blob/master/default.latex) template. 
