<!--suppress HtmlDeprecatedAttribute -->
<h1 align="center">
  <br>
  <a href="https://www.sphereon.com"><img src="https://sphereon.com/content/themes/sphereon/assets/img/logo.svg" alt="Sphereon" width="400"></a>
  <br>Veramo BBS+ signature support 
  <br>
</h1>

---

__Warning: These packages still is in a very early development stage. Breaking changes without notice will happen at this
point!__

---

# Veramo BBS+ signature support

This is mono repository, with packages that add BBS+ signature support to [Veramo](https://veramo.io) modules. The packages are drop in replacements for Veramo packages:

- bls-did-provider-key:
  - DID Key provider with support for BBS+
- bls-did-resolver-key:
  - DID Key resolver with support for BBS+
- bls-key-manager:
  - Veramo Key provider with support for BBS+
- bls-kms-local:
  - Veramo local KMS with support for BBS+

## Building and testing

### Lerna

This package makes use of Lerna for managing multiple packages. Lerna is a tool that optimizes the workflow around managing multi-package repositories with git and npm / yarn.

### Build

The below command builds all packages for you using lerna

```shell
yarn build
```

### Test

The test command runs:

* `jest`
* `coverage`

You can also run only a single section of these tests, using for example `yarn test:watch`.

```shell
yarn test
```

### Utility scripts

There are other utility scripts that help with development.

* `yarn prettier` - runs `prettier` to fix code style.

### Publish

There are scripts that can publish the following versions:

* `latest`
* `next`
* `unstable`

```shell
yarn publish:[version]
```
