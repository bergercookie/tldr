# vcstool

> Vcstool is a command line tool designed to make working with multiple
> repositories easier.
> More information: <https://github.com/dirk-thomas/vcstool>

- Get the status of multiple repositories under the current directory:

`vcs status /path/to/several/repos /path/to/other/repos /path/to/single/repo`

- Export list of repositories to the `my.repos` YAML file:

`vcs export > my.repos`

- Import list of repositories from YAML, clone them under the `src` directory:

`vcs import src < my.repos`

- Import list of repositories from YAML:

`vcs import < my.repos`

- Validate contents of YAML:

`vcs validate < my.repos`
