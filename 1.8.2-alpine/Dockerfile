FROM elixir:1.8.2-alpine

apk update \
  && apk add build-base postgresql-client nodejs nodejs-npm bash openssl-dev \
  && mix local.rebar --force \
  && mix local.hex --force

USER default
CMD ["bin/sh"]
