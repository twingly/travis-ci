# Travis CI

Repository used for [sharing Travis CI build configs][Build Config Imports] across repos.

## How to use

First you need to enable [Build Config Validation] for the repo, by adding the following to its `.travis.yml`:

```yml
version: ~> 1.0
```

Then just include the config(s) you want, for example:

```yml
import:
  - twingly/travis-ci:config/notifications.yml@master
  - twingly/travis-ci:config/ubuntu.yml@master
  - twingly/travis-ci:config/ruby.yml@master
```

[Build Config Imports]: https://docs.travis-ci.com/user/build-config-imports/
[Build Config Validation]: https://docs.travis-ci.com/user/build-config-validation
