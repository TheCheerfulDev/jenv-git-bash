# jenv-git-bash

jenv-git-bash is a command line tool to help you forget how to set the JAVA_HOME environment variable.

This version is a port/implementation of the original jenv (www.jenv.be), but is fully Windows git-bash compatible.

## Installation

Clone the repo:

```shell
$ git clone https://github.com/thecheerfuldev/jenv-git-bash ~/.jenv
```

Configure git-bash:

```shell
$ ~/.jenv/install_jenv_aliases.sh
```

Or, if you don't trust scripts you downloaded from the internet:

```shell
$ echo "alias java='source ${HOME}/.jenv/bin/java'" >> ~/.bashrc
$ echo "alias mvn='source ${HOME}/.jenv/bin/mvn'" >> ~/.bashrc
$ echo "alias jenv=${HOME}/.jenv/bin/jenv" >> ~/.bashrc
```

### Maven

To make sure that maven works, set either JENV_MAVEN_HOME, M2_HOME or MAVEN_HOME to a path that does __*NOT*__ contain a
whitespace.
