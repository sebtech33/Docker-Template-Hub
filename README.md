# Where to start?
To make this easier for others to navigate there has been made the following file structure:

## Configurations
Here will all configuration files for different software be located. This can be the static configuration for Traefik for example. The reason to split this from the compose file (if using Docker Compose) is to allow users to find relevant information easier rather than digging though different setups from K3S to Docker run and converting it to what you personally use.
```
/Configurations/<PROGRAM>/<VERSION>/
```

### `<PROGRAM>`
This represents the name of the program.

### `<VERSION>`
This represents the version of the program that i will leave so that you know what version is used for a working example. This will lower failiures when there becomes a new version available that can break things. If possible I will link to migration documentation of each program.

## Container Engine
Here is the program configuration/start file for the engine you use to run a program. 
```
/Container-Engine/<Engine Type>/
```

### `<Engine Type>`
Type of engine can be containers like Docker, Docker Compose, Helm, K3S, LXC. This will allow you to use what you want and have the configuration be applicable regardless of what you use.
