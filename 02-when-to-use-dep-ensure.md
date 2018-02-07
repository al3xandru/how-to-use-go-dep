# Using dep ensure

The command that you'll be using most frequently is `dep ensure`.  The
[official
documentation](https://golang.github.io/dep/docs/ensure-mechanics.html) explains in detail how it works: 

> Hey dep, please make sure that my project is in sync: that Gopkg.lock satisfies
> all the imports in my project, and all the rules in Gopkg.toml, and that vendor/
> contains exactly what Gopkg.lock says it should.

You'll be running `dep ensure` in 4 scenarios:

1.  adding a dependency
2.  updating a dependency
3.  updating after adding or removing imports for a package
4.  updating after editing the rules in
    [`Gopkg.toml`](01-initialize-dep.md#gopkgtoml)`
