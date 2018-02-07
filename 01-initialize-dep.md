# Initializing dep in a new project

Execute in the root directory of your project (e.g.
`$GOPATH/src/github.com/example/example`):

```
dep init
```

As a result of running this command you'll get 2 files (`Gopkg.toml`,
`Gopkg.lock`) and a folder (`vendor/`). As you'd expect, the `vendor` folder
will contain the source code of the dependencies.

### Gopkg.toml

`Gopkg.toml` is the file that will you'll edit yourself when needed. It contains
rules related to dependencies.  The format spec is available
[here](https://golang.github.io/dep/docs/Gopkg.toml.html).

### Gopkg.lock

`Gopkg.lock` is the pair file of `Gopkg.toml` and is generated when running `dep
init` and `dep ensure`. It contains the complete dependency graph (including
transitive dependencies) of the project.


# Moving an existing project to dep

Migrating an existing project that already has dependencies to `dep` could be
slightly more complicated.  Details about this can be found in [Migrating to dep](https://golang.github.io/dep/docs/migrating.html).
