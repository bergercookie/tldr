# npx

> Execute binaries from `npm` packages.
> More information: <https://www.npmjs.com/package/npx>.

- Execute the binary from a given npm module:

`npx {{module_name}}`

- Run react-app with npx:

`npx craete-react-app {{my-app}} --template typescript`

- In case a package has multiple binaries, specify the package name along with the binary:

`npx -p {{package_name}} {{module_name}}`

- View help contents:

`npx --help`
