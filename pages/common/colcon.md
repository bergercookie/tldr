# colcon

> colcon is a command line tool to improve the workflow of building, testing and
> using multiple software packages. It automates the process, handles the
> ordering and sets up the environment to use the packages.
> More information: <https://colcon.readthedocs.io/en/released/index.html>

- Create symlinks instead of copying executables and libraries:

`colcon build --symlink-install`

- Build only a package and its dependencies:

`colcon build --packages-up-to {{package-name}}`

- Trace what files are being sourced and how the environment changes:

`COLCON_TRACE=1 colcon ...`

- List packages, in topological ordering (breadth-first):

`colcon list -t`

- Generate a visual representation of the dependency graph (optionally include legend):

`colcon graph {{--legend}}`

- Colcon to generate `compile_commands.json` file for a cmake-based project:

`colcon build --cmake-args -DCMAKE_EXPORT_COMPILE_COMMANDS=1`
