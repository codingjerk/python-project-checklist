# Python Project Checklist

> Steps to check when starting on a python project

- [ ] Use [version control](#version-control)
- [ ] Setup [dependency management](#dependency-management)
- [ ] Add [documentation](#documentation)
- [ ] Add [license](#license)
- [ ] Add [tests](#tests)
- [ ] Add [linting](#linting)
- [ ] Setup [continious integration](#continious-integration)

## Version Control

- [ ] Use **git**
- [ ] Add `.gitignore` ([gitignore.io](http://gitignore.io/))

*Optionally you can use mercurial (hg), bazaar, darcs, etc.*

## Dependency Management

- [ ] Use **poetry**

*Optionally, you can stick with `requirements.txt`
and/or `requirements-dev.txt`.*

## Documentation

- [ ] Add `README.md` with a [template](https://github.com/pagarme/opensource/tree/master/templates)
- [ ] Use **OpenAPI** for API documentation
- [ ] Have a live demo made with **termtosvg**
- [ ] Create a documentation page with **mkdocs**, **mkdocs-material** and **mkdocstrings**

## License

- [ ] Add `LICENSE.md` with [MIT license](https://raw.githubusercontent.com/IQAndreas/markdown-licenses/master/mit.md)

## Tests

- [ ] Use **pytest**
- [ ] Add unit tests
  - [ ] Use **faker** / **mimesis** for fake data
  - [ ] Use **hypothesis** for property testing
- [ ] Add e2e tests
  - [ ] Use **tavern** for API testing
  - [ ] Use **playwright** for web testing
- [ ] Add smoke tests
- [ ] Add benchmarks with **pytest-benchmark**
- [ ] Add test coverage with **pytest-cov**

## Linting

- [ ] Use **flake8** with **flake8-docstrings**, **flake8-isort**
- [ ] Use mypy with [strict config](TODO)
- [ ] Use `.editorconfig`

## Continious integration

- [ ] Use **github actions**
- [ ] Add lint, test, build and publish pipeline stages
- [ ] Add badges to `README.md`
