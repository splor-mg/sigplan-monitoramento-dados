# sigplan-monitoramento-dados

[![Updated](https://github.com/splor-mg/sigplan-monitoramento-dados/actions/workflows/all.yaml/badge.svg)](https://github.com/splor-mg/sigplan-monitoramento-dados/actions/)

## Pré-requisitos

Esse projeto utiliza Docker para gerenciamento das dependências. Para fazer _build_  da imagem execute:

```bash
docker build --tag sigplan-monitoramento-dados .
```

## Uso

Para executar o container

```bash
docker run -it --rm --mount type=bind,source=$(PWD),target=/project sigplan-monitoramento-dados bash
```

Uma vez dentro do container execute os comandos do make

```bash
make all
```

_Gerado a partir de [cookiecutter-datapackage@fbd0381](https://github.com/splor-mg/cookiecutter-datapackage/commit/fbd03815a2b2ff23169bba81d3bf619dfb8d7038)_
