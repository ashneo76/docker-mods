# java - Docker mod for code-server/openvscode-server

This mod adds a java dev environment to code-server/openvscode-server, to be installed/updated during container start.

In code-server/openvscode-server docker arguments, set an environment variable `DOCKER_MODS=linuxserver/mods:code-server-java`

You can define the java version to be installed via setting the environment variable `JAVA_MOD_VERSION` (accepts a version from https://bell-sw.com/pages/downloads/ Default: `21.0.1+12`)

You can also set the architecture: `JAVA_MOD_ARCH` (accepts one of `amd64` or `aarch64`. Default: `amd64`)

If adding multiple mods, enter them in an array separated by `|`, such as `DOCKER_MODS=linuxserver/mods:code-server-java|linuxserver/mods:code-server-mod2`
