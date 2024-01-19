# {{ cookiecutter.project_name }}

{{ cookiecutter.project_description }}

## dependencies

| name                                       | description                                |
|--------------------------------------------|--------------------------------------------|
| [pyenv](https://github.com/pyenv/pyenv)    | python version management                  |
| [poetry](https://github.com/python-poetry) | python packaging and dependency management |
| [terraform](https://www.terraform.io/)     | infrastructure as code automation          |

## install

development:
```shell
poetry install
poetry shell
pre-commit install
```

production:
```shell
poetry install --without dev
```

## build

package:
```shell
poetry build
```

## usage

run:
```shell
terraform init
terraform plan
terraform apply
```

test:
```shell
tox run
```

doc:
```shell
make -C docs html
```

check:
```shell
pre-commit run
```
