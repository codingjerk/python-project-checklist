# Python Project Checklist

> Steps to check when starting on a python project

- [ ] Use [version control](#version-control)
- [ ] Setup [dependency management](#dependency-management)
- [ ] Add [documentation](#documentation)
- [ ] Add [license](#license)
- [ ] Add [tests](#tests)
- [ ] Add [linting](#linting)
- [ ] Check [logging](#logging)
- [ ] Setup [continuous integration](#continious-integration)
- [ ] Make [contribution](#contribution) easier

## Version Control

- [ ] Use **git**
- [ ] Add `.gitignore` ([gitignore.io](http://gitignore.io/))
- [ ] Use [conventional commits](https://www.conventionalcommits.org/en/v1.0.0/)
  - [ ] Consider using **cz** [(link)](https://commitizen-tools.github.io/commitizen/)

*Optionally you can use mercurial (hg), bazaar, darcs, etc.*

## Dependency Management

- [ ] Use **poetry** and `pyproject.toml` (see [PEP621](https://peps.python.org/pep-0621/))

*Optionally, you can stick with setuptools or hatchling*

## Documentation

- [ ] Add `README.md`
  - [ ] Have an intro
  - [ ] Have an installation/deploy section
  - [ ] Have a usage section
  - [ ] Have a live demo made with **termtosvg**
- [ ] Use **OpenAPI** for API documentation
- [ ] Create a documentation page with **mkdocs**, **mkdocs-material** and **mkdocstrings**
- [ ] Add badges
  - [ ] CI pipeline status
  - [ ] Code quality: code coverage, maintainability indexes
  - [ ] Package status: package health (see [Snyk](https://snyk.io/)), vulnerabilities, out of date dependencies
  - [ ] General status: maintenance status, uptime (for web)
  - [ ] Package info: size, lines of code, license, version
  - [ ] Popularity: stars, downloads
  - [ ] Discord server
  - [ ] Funding via [Open Collective](https://opencollective.com/)
  - Find more at [shields.io](https://shields.io/) and [badgen.net](https://badgen.net/)

## License

- [ ] Add `LICENSE.md` with [MIT license](https://raw.githubusercontent.com/IQAndreas/markdown-licenses/master/mit.md)

## Tests

- [ ] Use **pytest**
- [ ] Add unit tests
  - [ ] Use **faker** / **mimesis** for fake data
  - [ ] Use **hypothesis** for property testing
- [ ] Add e2e tests
  - [ ] Use **tavern** for API testing
  - [ ] Use **playwright** for UI testing
- [ ] Add smoke tests
- [ ] Add benchmarks with **pytest-benchmark**
  - [ ] Use **pytest-memray** to control memory usage
- [ ] Add test coverage with **pytest-cov**

## Linting

- [ ] Use **ruff**
- [ ] Use **mypy**
- [ ] Use `.editorconfig` (see [.editorconfig](./examples/.editorconfig))
- [ ] Use specific linters
  - [ ] Use **cspell** to check spelling
  - [ ] Use **shellcheck** for `shell` scripts
  - [ ] Use **sqlfluff** for `sql` files
  - [ ] Use **yamllint** for `yml` files
  - [ ] Use **hadolint** for `Dockerfile`s
  - [ ] Use **dotenv-linter** for `env` files

## Logging

- [ ] Use **loguru**
- [ ] Consider change default `LOGURU_LEVEL` to `INFO`

## Continuous integration

- [ ] Use **github actions**
- [ ] Add lint, test, build and publish pipeline stages
- [ ] Add badges to `README.md`

## Contribution

- [ ] Have `CONTRIBUTING.md` file (see [example](https://github.com/github/docs/blob/main/CONTRIBUTING.md) and [another one](https://gist.github.com/PurpleBooth/b24679402957c63ec426))
- [ ] Have "Contribution" section in your `README.md`
- [ ] Have `CODE_OF_CONDUCT.md` file (see [example](https://github.com/probot/template/blob/master/CODE_OF_CONDUCT.md))
