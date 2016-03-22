## What is nvm?

[nvm] is a tool for managing multiple versions of node and npm.

[nvm]: https://github.com/creationix/nvm/blob/master/README.markdown

## What is fast-nvm-fish?

It's a utility that manipulates your PATH to include the desired version of node. Other solutions require parsing `env`'s output and do other slow things. Before this, there was an extra second or two added to my shell startup time. With about 10 versions of node installed this script takes 50ms to run.

## Usage

```sh
nvm install 5
nvm use 5 # or e.g. 5.8 or 5.8.1
```

## Install:

```sh
curl -sSL https://raw.githubusercontent.com/brigand/fast-nvm-fish/master/nvm.fish > ~/.config/fish/functions/nvm.fish
```

To make it work on new shells you'll need to set a version in your config.fish.

```sh
fish use 5
```


