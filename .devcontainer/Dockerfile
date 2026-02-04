FROM elixir:1.19.5

RUN apt-get update && apt-get install -y \
  postgresql-client \
  && rm -rf /var/lib/apt/lists/*


RUN mix local.hex --force && \
    mix local.rebar --force && \
    mix archive.install hex phx_new --force