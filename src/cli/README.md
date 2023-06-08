# Using the ocaml-docs ci tool

## Usage

`dune exec -- ocaml-docs-ci-client --ci-cap <path to cap file> --project <project name>`

-- Notes

`ocaml-docs-ci` default command brings up help

`ocaml-docs-ci list --ci-cap <path to cap file> --project <project-name-infix>` shows a list of project names that have the given string as an infix

`ocaml-docs-ci status --ci-cap <path to cap file>` shows a dashboard of documentation build results across opam-repository packages. Packages can be filtered by maintainer substrings or tag names in the opam package description.

`ocaml-docs-ci status --ci-cap <path to cap file> --project <project_name>` show the build status of all versions of a project.

`ocaml-docs-ci status --ci-cap <path to cap file> --project <project_name> --version <version>` show the build status of a single version of a project.

`ocaml-docs-ci status --ci-cap <path to cap file> --project <project_name> --version <version> --job <job-id>` show the build status of a single job

`ocaml-docs-ci logs --ci-cap <path to cap file> --job <job-id>` display logs for an individual job

`ocaml-docs-ci rebuild --ci-cap <path to cap file> --job <job-id>` rebuild a specific job

## Reference

https://github.com/ocaml/infrastructure/wiki/Using-the-opam-ci-tool