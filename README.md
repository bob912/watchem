# watchem

Forked from https://github.com/tartley/rerun2 and modified to make it watch for file access instead of modification.

Save *watchem* on your PATH, and invoke it using:

    watchem COMMAND

It runs COMMAND every time there's a filesystem access event within your current
directory (recursive).

COMMAND needs to be a single parameter to `watchem`, hence if it contains
spaces, either quote the whole thing:

    watchem "ls ~"

or escape them:

    watchem ls\ ~

