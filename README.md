# Dutch Government API portal

> 👩‍🔬 This project is an early stage **Proof of Concept**, which means functionality and documentation might be broken, missing or flat out wrong.

A website to advertise the APIs provided by governments and public administrations in the Netherlands.

---

## Adding content

### Adding an organisation

Add a file with the following file pattern: `/apis/{organisationName}/index.md`, and make sure the title of the file is the name of the organisation.

### Adding an API

Add a file with the following file pattern: `/apis/{organisation-name}/{api-name}.md`. The following front-matter variables are available to be set:

```yaml
---
OpenAPI: https://api.data.amsterdam.nl/afval/swagger/
licence: cc0
url: https://api.data.amsterdam.nl/afval/
---
```

Make sure to add the API to the organisations' index, since there is no automatic inclusion.

---

## Installing, running and building

This site and it's contents are served over [GitHub pages](http://pages.github.com) and redered in it's native static site genrator [Jekyll](http://jekyllrb.com).

More on [Jekyll as a static site generator with GitHub](https://help.github.com/articles/using-jekyll-as-a-static-site-generator-with-github-pages/).

### Installing locally

[Install Ruby and it's package manager Bundler](https://help.github.com/articles/setting-up-your-github-pages-site-locally-with-jekyll/) with 

```bash
gem install bundler
```

Install the dependencies and Jekyll using 

```bash
bundle install
```

### Running and serving locally

Run Jekyll, generate the site, watch for changes and serve over a local webserver with 

```bash
jekyll serve
```
