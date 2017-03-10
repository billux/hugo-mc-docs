# MakinaCorpus documentation Theme for hugo

## install/usage

- Download
    ```sh
    mkdir hugoproject
    cd hugoproject
    git submodule add https://github.com/makinacorpus/hugo-mc-docs.git themes/hugo-mc-docs
    ```
- non docker
    ```sh
    themes/hugo-mc-docs/bin/control.sh install
    # This start the gulp development server after build)
    themes/hugo-mc-docs/bin/control.sh serve
    ```

- Via docker, not that the script will start the gulp development server after build
    ```sh
    themes/hugo-mc-docs/bin/docker.sh
    ```
- Create a content
    ```sh
    ./bin/control.sh hugo new content/doc.md
    ```

## Notes
- This theme install its own hugo, node & virtualenv flavors
    on local folders along the project (./var).
- Livesearch is enabled throrough lunr.js and a special crafted (via hugo at build time) JSON file.
