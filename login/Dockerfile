FROM docker:latest

LABEL "name"="OpenFaaS Login Action"
LABEL "maintainer"="Lucas Roesler <roesler.lucas@gmail.com>"
LABEL "version"="1.0.0"

LABEL "com.github.actions.name"="GitHub Action for OpenFaaS Login"
LABEL "com.github.actions.description"="Wraps the OpenFaaS CLI to enable the faas-cli login command."
LABEL "com.github.actions.icon"="package"
LABEL "com.github.actions.color"="blue"

RUN apk add --no-cache \
		git \
        ca-certificates

COPY --from=openfaas/faas-cli:0.12.4 /usr/bin/faas-cli /usr/bin/
