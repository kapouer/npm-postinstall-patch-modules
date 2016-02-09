# npm-postinstall-patch-modules
An example of how package.json postinstall script can apply patches to node_modules from a directory

`npm install`

will install patches that are in `patches/` directory and
that are listed in the `patches/series` file.

This example uses `quilt(1)` utility to manage how patches are applied.

In particular it is quite resilient against updates and failures.
