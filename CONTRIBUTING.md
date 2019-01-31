# Contributing to the Developer portal

We – the maintainers of this project – value your input, enjoy feedback and welcome improvements.

We love issues and pull requests from everyone.

## Problems, suggestions and questions

You don't need to change any of our code or documentation to be a contributor. Many contributors add to our software by reporting problems, suggesting changes and asking simple and difficult questions. To do this, you can create a [GitHub Issue](https://help.github.com/articles/creating-an-issue/) for this project.

## Content, APIs, documentation and code

If you want to add to the content, documentation or code of one of our projects you should make a Pull Request. If you never used GitHub, get up to speed with [Understanding the GitHub Flow](https://guides.github.com/introduction/flow/). If you would like to learn more about using GitHub Pages, the content management system for this site, please check out the interactive courses in the [GitHub lab](https://lab.github.com).

### 1. Make your changes

Add your changes in commits [with a message that explains them](https://github.com/alphagov/styleguides/blob/master/git.md#commit-messages). Document choices or decisions you make in the commit message, this will enable everyone to be informed of your choices in the future.

#### Adding an Organisation

1. Add a folder with the lowercase and hyphens (`kebab-case`) name of the governmental organsiation, for example `gemeente-amsterdam` or `kadaster`.
2. Add a MarkDown file named `index.md` to the folder that starts with the following ['Front Matter'](https://jekyllrb.com/docs/front-matter/):

```markdown
---
title: Gemeente Amsterdam # Official name of the organisation
websiteUrl: http://amsterdam.nl # Homepage of the organsation
---
```

Feel free to describe a bit more about this organisation and it's take on developers.

#### Adding an API

1. In the folder of the organsiation (`organisations/organisation-name`) add a new MarkDown file with the name of the resource or endpoint in lowercase and hyphens (`kebab-case`). For instance `trash-bin-locations.md`.
2. Add a MarkDown file named `index.md` to the folder that starts with the following ['Front Matter'](https://jekyllrb.com/docs/front-matter/):

```markdown
---
name: Garbage bin location API # The name of the API
openAPIUrl: https://api.data.amsterdam.nl/afval/swagger/ # OpenAPI Url (if available)
url: https://api.data.amsterdam.nl/afval/ # URL of the resource
licenceSpdx: CC0-1.0 # SPDX Licence code
---
```

And this file can have a more in depth description of the API and per haps some examples in the body of the MarkDown document.

### 2. Pull Request

When submitting the pull request, please accompany it with a description of the problem you are trying to address and the issue numbers that this Pull Request fixes/addresses.

### 3. Improve

It could be that your contribution can be merged immediately by a maintainer. However, usually, a new Pull Request needs some improvements before it can be merged. Other contributors (or helper robots) might have feedback. If this is the case the reviewing maintainer will help you improve your documentation and code.

If your documentation and code have passed human review and have passed the automated tests, it is merged.

### 4. Celebrate

Your ideas, documentation and code have become an integral part of this project. You are the Open Source hero we need.

---

For more information on how to use and contribute to this project, please read the [`README`](README.md).
