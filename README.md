# OpenFaaS Code Eval

Code eval as a service. Powered by [OpenFaaS](https://www.openfaas.com/). (WIP)

## Setup

Spin up OpenFaas:

```sh
$ docker swarm init
$ git clone https://github.com/openfaas/faas && \
  cd faas && \
  ./deploy_stack.sh
```

Run a build with the [faas-cli](https://github.com/openfaas/faas-cli):

```sh
$ faas-cli build -f template.yml
```

Deploy:

```sh
$ faas-cli deploy -f template.yml
```