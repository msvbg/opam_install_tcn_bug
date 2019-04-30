Reproduces https://github.com/darklang/tablecloth/issues/45.

Using [esy](https://esy.sh/), run `esy install` and then `esy build`. Returns:
```
$ esy build
info esy build 0.5.6 (using package.json)
File "dune", line 5, characters 13-30:
5 |   (libraries tablecloth-native))
                 ^^^^^^^^^^^^^^^^^
Error: Library "tablecloth-native" not found.
Hint: try: dune external-lib-deps --missing @@default
error: command failed: 'dune' 'build' (exited with 1)
esy-build-package: exiting with errors above...
error: build failed with exit code: 1

esy: exiting due to errors above
```
