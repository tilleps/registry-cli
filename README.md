# registry-cli


```sh
NAME

    registry-cli -- remove older image(s) from a private Docker Registry

SYNOPSIS

    registry-cli [-d] registry_url image_name limit [username] [password]
    registry-cli -h

DESCRIPTION

    Removes the tagged image(s) from the local Docker Registry.

    The following options are available:

    registry_url  The domain/host of the registry, include the protocol (https/http), exclude the path (/v2/*)
    image_name    The image you want to delete
    limit         The number of tags you want to keep for a specific image, set to 0 to delete all, -1 to keep all
    username      [OPTIONAL] The username to connect to the Docker registry
    password      [OPTIONAL] The password to connect to the Docker registry

    -d [OPTIONAL] Enables delete mode is enabled
    -h [OPTIONAL] Display this help

EXAMPLES

    $ registry-cli https://registry.example.local app 5 username password
```