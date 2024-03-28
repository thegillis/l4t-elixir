
FROM dustynv/jetson-inference:r35.4.1

RUN add-apt-repository -y ppa:rabbitmq/rabbitmq-erlang

RUN apt-get update -y && apt-get install -y build-essential git vim elixir erlang-dev erlang-xmerl

RUN mix do local.hex --force, local.rebar --force

RUN wget -O /usr/local/bin/bazel https://github.com/bazelbuild/bazelisk/releases/download/v1.19.0/bazelisk-linux-arm64 && chmod a+x /usr/local/bin/bazel

