# gh-user

GitHub CLI User Management Extension

## Installation

```sh
gh extension install norwd/gh-user

```

### Building locally

```sh
gh repo clone norwd/gh-user
cd gh-user
# optionally make edits or changes
gh extension install .
```

## Usage

### Work with GitHub User Profiles

*USAGE*

    gh user <command> [flags] [arguments ...]

*COMMANDS*

    help:      Show this message
    status:    Set user status emoji
    bio:       Set user bio/blurb

*FLAGS*

    -h, --help:    Show help for command

*EXAMPLES*

    $ gh user status -b --emoji=:dart: "Focusing"
    $ gh user bio "Hi! I'm Octocat :smile:"

*LEARN MORE*

    Use 'gh user <subcommand> --help' for more info

### Work with GitHub User Statuses

*USAGE*

    gh user status [-h|--help]
    gh user status [-b|--busy] [-e|--emoji EMOJI] MESSAGE ...

*FLAGS*

    -h, --help:           Show help for command
    -b, --busy:           Mark status as busy
    -e, --emoji EMOJI:    Set emoji for status

*ARGUMENTS*

    Trailing arguments are combined as the status message.

*EXAMPLES*

    $ gh user status I'm working on a PR
    $ gh user status -b --emoji :dart: "Focusing"
    $ gh user status --busy=false --emoji=:video_game:

### Work with GitHub User Biography Descriptions

*USAGE*

    gh user bio [-h|--help]
    gh user bio MESSAGE ...

*FLAGS*

    -h, --help:    Show help for command

*ARGUMENTS*

    Trailing arguments are combined as the bio message.

*EXAMPLES*

    $ gh user bio "Hi! I'm Octocat :smile:"
    $ gh user bio $(fortune -s)
