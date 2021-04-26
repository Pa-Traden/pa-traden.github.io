# På tråden

This is the På Tråden podcast site. It includes a source code repository as well
as a github-pages repository.

The final website is generated using jekyll.

## Installation

Clone this repository as well as its sub-repo

```
git@github.com:Pa-Traden/pa-traden-source-code.git patradenpod
cd patradenpod
git submodule update --init --recursive
cd _site
git checkout main
```

Install a recent version of ruby (3.0.0 at the time of writing) and execute

```
bundle install
```

Followed by the following command to start a development server on
`http://localhost:4000`

```
bundle exec jekyll serve
```

Make sure not to commit anything straight after running the development server
as all global links will be replaced with "localhost"

To create a Github-build execute

```
bundle exec jekyll build
```

And commit the changes of the `_site` folder.
