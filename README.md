# prompts-cli [![npm version](http://img.shields.io/npm/v/prompts-cli.svg?style=flat-square)](https://www.npmjs.org/package/prompts-cli)

> Use [prompts] from shell scripts.

[prompts]: https://www.npmjs.com/package/prompts

## Usage

```
Usage: prompts <type> <message> [options]
       prompts <type> <message> [options] < choices
```

## Example

```sh
name=$(prompts text "What's your name?")
age=$(prompts number 'How old are you?' --min 18)
beer=$(printf 'Pilsner\nStout\nIPA\n\nNEIPA\nOther' | prompts select 'Favorite beer?')
confirm=$(prompts toggle 'Are you sure?' --active yes --inactive no)
```
