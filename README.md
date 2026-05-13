# gh-user

GitHub CLI User Management Extension

<img src="https://codeberg.org/norwd/human/raw/branch/main/docs/automatic-logo.svg" height="50" />

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

# I'm Using GitHub Under Protest

My projects are currently hosted on GitHub.
This is not ideal; GitHub is a proprietary, trade-secret system that is not Free and Open Source Software (FOSS).
I am deeply concerned about using a proprietary system like GitHub to develop my FOSS projects.
I have an [open discussion][Leaving GitHub Discussion] where I am planning how to move away from GitHub in the long term.
I urge you to read about the [Give up GitHub] campaign from the [Software Freedom Conservancy] to understand some of the reasons why GitHub is not a good place to host FOSS projects.

If you are a contributor who personally has already quit using GitHub, please [check this resource][Leaving GitHub Discussion] for how to send in contributions without using GitHub directly.

Any use of my projects' code by GitHub Copilot, past or present, is done without my permission.
I do not consent to GitHub's use of any of my projects' code in Copilot.

![Logo of the GiveUpGitHub campaign](https://sfconservancy.org/static/img/GiveUpGitHub.png)

[Leaving GitHub Discussion]: https://github.com/norwd/norwd/discussions/7
[Give up GitHub]: https://GiveUpGitHub.org
[Software Freedom Conservancy]: https://sfconservancy.org
    $ gh user bio $(fortune -s)
