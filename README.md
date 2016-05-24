## Lima Tool

This is a simple tool to wrap *docker* and *docker-compose* commands.

## Motivation

I've start use docker-compose and it's lot easier than the default *docker* command. But when I use *docker-compose* for development it's common to send a lot of commands to the container, sometimes I get myself writing `docker-compose -f docker-compose.test.yml -p "$(pwd)test" run webserver bundle exec rspec <test path>`. Well it's a lot of things, of course I wrote some aliases but in some cases I need a more complex script.
When I need this script I need to go on internet to find it again.

## Installation

To install **Lima** you just need to clone this repository and call `./lima install`.
```
  git clone https://github.com/brunodles/lima.git
  git checkout tags/2.0.0
  ./lima install
```

## Modules

Lima have some modules to specific languages, this will help to send some commands language tools inside the container.

### Install a Module

To install a module you just need to call the *lima script* from the *repository*.
```
  ./lima module -i <module name>
```

### Uninstall a Module

To uninstall a module you just need to call the *lima script* from the *repository*.
```
  ./lima module -u <module name>
```

## Tests

I want to include some tests, by now I'm thinking to check the helper command that this tool will generate.

## Contributors

If you:
* want to help with something
* want to add a new module,
* have some idea how to test it
You can create a issue here on github or talk with me on Twitter(`brunodles`).
