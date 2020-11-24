# Alloverse Placeserv

Server component of Alloverse. Basically a multiplayer game server, but for window manager-y
things.

## Setup 

* `git submodule update --init --recursive`

then...

### macOS
* `brew install elixir cmake`
* `mix deps.get`

### Ubuntu (including Ubuntu-on-Windows)

* `wget https://packages.erlang-solutions.com/erlang-solutions_1.0_all.deb `
* `sudo dpkg -i erlang-solutions_1.0_all.deb; rm erlang-solutions_1.0_all.deb`
* `sudo apt-get update`
* `sudo apt-get install esl-erlang`
* `sudo apt-get install elixir cmake clang openssl`
* `mix deps.get`

## Run

* `mix run --no-halt`

### Docker

* `docker build -t alloplace .`
* `ALLOPLACE_NAME="lol" docker run -p 21337:21337/udp -it alloplace`