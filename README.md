# MuCrucible: Your MuFoundry Game Starter

## What is this?
MuCrucible is a "project template / starting project skeleton" for creating your own MuFoundry-based game/project.

## How you're intended to use it:

1. Clone this repository.
2. Customize it to fit your game's needs.
3. Build and run your game using the provided structure.

That sounds simple, but for some more details:

### Virtual Environments
You will likely want to create a `Virtual Environment` for python to hold all dependencies and install MuForge and MuPlugins into.

To create a Virtual Environment:
`python -m venv .venv`

And to activate it:
`source .venv/bin/activate`
Or, on windows:
`.\.venv\Scripts\activate`

## config directory
The `config` directory holds .toml files for configuring your game. the `muforge` launch process will load and merge them using `Dynaconf` and generate a final configuration object as a Python dictionary. Both the Game and Portal will have access to the configuration.

## webserver directory
The `webserver` directory has both a static folder and a root folder for serving web content.
