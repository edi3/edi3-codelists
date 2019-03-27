# edi3 Code Lists Specifications

The edi3 Code Lists Specifications are based on ...

* [Code Lists GitHub repository](https://github.com/edi3/edi3-codelists)
* [Code Lists Slack Channel](https://edi3.slack.com/messages/spec-codelists/) ([you must signup to edi3 slack first](https://join.slack.com/t/edi3/shared_invite/enQtNTY5OTkzMjQ0NjcyLTM1MzYyNjg5M2RlMWIyZjUzMDBlNWQ3OWIyZTNhMDhhN2UzYjIyMjk4M2VhM2ViNzhhM2Y1OWE0Y2FhYTc1ZTg))

| Specification URL | Version | Status | API Definition | Issues List |
| ----------------- | ------  | ------ | -------------- | ----------- |
| [Code Lists spec Recommendation 20](//edi3.org/specs/edi3-codelists/develop/recommendation-20/) | Working Draft | ![Raw](https://rfc.unprotocols.org/spec:2/COSS/raw.svg) | [ReDoc](//edi3.org/specs/edi3-codelists/develop/recommendation-20/redoc-static.html) |  [Code Lists Issues](https://github.com/edi3/edi3-codelists/issues)  |
| [Code Lists spec Recommendation 21](//edi3.org/specs/edi3-codelists/develop/recommendation-21/) | Working Draft | ![Raw](https://rfc.unprotocols.org/spec:2/COSS/raw.svg) | [ReDoc](//edi3.org/specs/edi3-codelists/develop/recommendation-21/redoc-static.html) |  [Code Lists Issues](https://github.com/edi3/edi3-codelists/issues)  |
| [Code Lists spec Recommendation 24](//edi3.org/specs/edi3-codelists/develop/recommendation-24/) | Working Draft | ![Raw](https://rfc.unprotocols.org/spec:2/COSS/raw.svg) | [ReDoc](//edi3.org/specs/edi3-codelists/develop/recommendation-24/redoc-static.html) |  [Code Lists Issues](https://github.com/edi3/edi3-codelists/issues)  |

## Known Implementations

Known implementations (open source or otherwise) are listed here.  Please modify this page and make a pull request to add your own.

|Provider|Implementation URL|Comments|
|--------|------------------|--------|
|  |  |  |

## Github Specification repository usage

The files from the repository `docs` direcotry are puplished on [edi3.org](https://edi3.org). The specification is presented at least by the specification page `index.md` with the configuration header, which is later processed by Jekyll build and converted to `index.html`. If there is a Rest API applied for the specification, it is presented by Open API specification `swagger.yml`(or `swagger.yaml`). Open API specification file is processed by Redoc (https://github.com/Rebilly/ReDoc) with the output `redoc-static.html` file.
 
The following files are the part of the standard approach:

 * [docs](./docs)
   * [index.md](./docs/index.md)
   * [swagger.yaml](./docs/swagger.yaml)
 * [resources](./resources)
   * [filename.ext](./resources/filename.ext)
 * [.gitignore](./.gitignore)  
 * [LICENSE.txt](./LICENSE.txt)
 * [README.md](./README.md)

In case if there are more than one specification in the repo, the sub-directories are added to the `docs` directory:

 * [docs](./docs)
   * [recommendation-20](./recommendation-20)
     * [index.md](./docs/index.md)
     * [swagger.yaml](./docs/swagger.yaml)
   * [recommendation-21](./recommendation-21)
     * [index.md](./docs/index.md)
     * [swagger.yaml](./docs/swagger.yaml)
   * [recommendation-24](./recommendation-24)
     * [index.md](./docs/index.md)
     * [swagger.yaml](./docs/swagger.yaml)
 * [resources](./resources)
   * [filename.ext](./resources/filename.ext)
 * [.gitignore](./.gitignore)  
 * [LICENSE.txt](./LICENSE.txt)
 * [README.md](./README.md)

To support versioning, all branches and tags are getting published on [edi3.org](https://edi3.org) with the following structure:

 * [specs](https://github.com/edi3/edi3.github.io/tree/master/specs)
   * [edi3-codelists](https://github.com/edi3/edi3.github.io/tree/master/specs/edi3-codelists)
     * [develop](https://github.com/edi3/edi3.github.io/tree/master/specs/edi3-codelists/develop)
       * [docs](./docs)
         * [recommendation-20](./recommendation-20)
           * [index.html](./docs/index.html)
           * [redoc-static.html](./docs/redoc-static.html)
           * [swagger.yaml](./docs/swagger.yaml)
         * [recommendation-21](./recommendation-21)
           * [index.html](./docs/index.html)
           * [redoc-static.html](./docs/redoc-static.html)
           * [swagger.yaml](./docs/swagger.yaml)
         * [recommendation-24](./recommendation-24)
           * [index.html](./docs/index.html)
           * [redoc-static.html](./docs/redoc-static.html)
           * [swagger.yaml](./docs/swagger.yaml)
     * [master](https://github.com/edi3/edi3.github.io/tree/master/specs/edi3-codelists/master)
       * [docs](./docs)
         * [recommendation-20](./recommendation-20)
           * [index.html](./docs/index.html)
           * [redoc-static.html](./docs/redoc-static.html)
           * [swagger.yaml](./docs/swagger.yaml)
         * [recommendation-21](./recommendation-21)
           * [index.html](./docs/index.html)
           * [redoc-static.html](./docs/redoc-static.html)
           * [swagger.yaml](./docs/swagger.yaml)
         * [recommendation-24](./recommendation-24)
           * [index.html](./docs/index.html)
           * [redoc-static.html](./docs/redoc-static.html)
           * [swagger.yaml](./docs/swagger.yaml)

The default branch is develop and it represents the current Working Draft version. When a release is ready, a tag is added and merged to the master branch, so the master branch always is the latest release version. Contributiros shall fork the specification repo and create a PR against the develop branch. For minor version updates hotfix branches shall be created from the corresponding tag.
