# Contributing to this Municipio bundle

Please read this document carefully before contributing to this package.

## Releases and versioning

When making a new release, the version tag should be chosen according to the
principles of [Semantic Versioning](https://semver.org/) with the
MAJOR.MINOR.PATCH pattern. If the new release introduces any breaking changes,
the _major_ version number MUST be increased to prevent consumers from
accidentally updating to an incompatible version of this package. The _minor_
version number is increased when backwards-compatible features are added. The
_patch_ version is increased only when making backwards-compatible bugfixes and
security updates. Examples:

1. If you add a new plugin to the bundle, increase the _minor_ version.
2. If you update a plugin and the update introduces breaking changes, bump the
   _major_ version.
3. If the updated plugin adds new backwards-compatible features, bump the
   _minor_ version.
4. If the update is a security update, bump the _patch_ version.
5. If you remove a plugin, increase the _major_ version.
6. If you update any metadata or documentation that has no effect on the actual
   code, increase the _patch_ version (if a new release is even necessary).

When making a new release, don’t forget to also update the version number in the
package.json file and update CHANGELOG.md

## Node modules

Use Yarn to manage Node module dependencies. Since this package is metapackage,
no JS code will be actually be used by the consumer so Node modules are only dev
dependencies, e.g. Prettier for code formatting. This repository will not be
published on NPM

## Code formatting

Format all files with Prettier before committing your changes by running
`yarn format`.
