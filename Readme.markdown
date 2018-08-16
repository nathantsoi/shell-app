             __         ____
       _____/ /_  ___  / / /     ____ _____  ____
      / ___/ __ \/ _ \/ / /_____/ __ `/ __ \/ __ \
     (__  ) / / /  __/ / /_____/ /_/ / /_/ / /_/ /
    /____/_/ /_/\___/_/_/      \__,_/ .___/ .___/
                                   /_/   /_/

# shell-app

Turn a shell script into an OS X application.

## Usage

    shell-app example.sh example.app example.icns

## Description

Creates an OS X application bundle that calls a given shell script or
command.

This provides a command line alternative to creating application bundles with
Automator. The shell script is first wrapped in a short AppleScript
wrapper which is then compiled with `osacompile`. When the output file
includes the .app extension, `osacompile` outputs an application bundle
wrapping the AppleScript file.

## See also

- https://gist.github.com/mathiasbynens/674099
  - Creates very simple applications, but they are too simple to be
    recognized by Spotlight as applications.
- https://mathiasbynens.be/notes/shell-script-mac-apps
- http://www.sveinbjorn.org/platypus
