# ThreeThirds Collaboration Documentation Site (docs.collab.cloud)

This site is hosted on github pages and is generated by [mkdocs](https://www.mkdocs.org) and [mkdocs-material](https://hub.docker.com/r/squidfunk/mkdocs-material/)

The static files for the website are served out from the `gh-pages` branch.

## Making changes, adding pages, etc

1. Clone this repo or issue `git pull` to get the latest
2. Install mkdocs & mkdocs-material as per [these instructions](https://squidfunk.github.io/mkdocs-material/getting-started/#installation) (Please make sure use pip3 to install both of mkdocs & mkdocs-material instead of pip)
3. Install [mkdocs-redirects](https://pypi.org/project/mkdocs-redirects/)

    ```sh
    pip install mkdocs-redirects
    ```

    or

    ```sh
    pip3 install mkdocs-redirects
    ```

4. Directly commit any changes to the master branch to publish a new version of the website. This includes editing md files or config in `mkdocs.yml` and adding new pages and assets.

5. Then the site must be generated and committed by issuing:

    ```sh
    mkdocs gh-deploy
    ```

## Previewing changes locally before commit

1. Run this command in project dir

    ```sh
    mkdocs serve
    ```

2. Browse to [http://127.0.0.1:8000](http://127.0.0.1:8000)

## More info

1. See the file `mkdocs.yml` for site config
2. Check out the docs for [mkdocs](https://www.mkdocs.org) and [mkdocs-material](https://squidfunk.github.io/mkdocs-material)

## Latest Updates

The Search plugin is enabled since March 18 2021
