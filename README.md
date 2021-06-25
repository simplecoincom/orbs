# simplecoin-orbs/simplecoin-utils orb

[![CircleCI Build Status](https://circleci.com/gh/simplecoincom/orbs.svg?style=shield "CircleCI Build Status")](https://circleci.com/gh/simplecoincom/orbs) [![CircleCI Orb Version](https://badges.circleci.com/orbs/simplecoin-orbs/simplecoin-utils.svg)](https://circleci.com/orbs/registry/orb/simplecoin-orbs/simplecoin-utils) [![GitHub License](https://img.shields.io/badge/license-MIT-lightgrey.svg)](https://raw.githubusercontent.com/simplecoincom/orbs/master/LICENSE)


The purpose of the simplecoin-utils orb is to provide a single orb to automate semantic-release's and other delivery in the SimpleCoin orginisation.

Additional READMEs are available in each directory.

## Resources

[CircleCI Orb Registry Page](https://circleci.com/orbs/registry/orb/simplecoin-orbs/orbs) - The official registry page of this orb for all versions, executors, commands, and jobs described.

### How to Contribute

We welcome [issues](https://github.com/simplecoincom/orbs/issues) to and [pull requests](https://github.com/simplecoincom/orbs/pulls) against this repository!

### How to Publish
* Create and push a branch with your new features.
* When ready to publish a new production version, create a Pull Request from _feature branch_ to `master`.
* The title of the pull request must contain a special semver tag: `[semver:<segment>]` where `<segment>` is replaced by one of the following values.

| Increment | Description|
| ----------| -----------|
| major     | Issue a 1.0.0 incremented release|
| minor     | Issue a x.1.0 incremented release|
| patch     | Issue a x.x.1 incremented release|
| skip      | Do not issue a release|

Example: `[semver:major]`

* Squash and merge. Ensure the semver tag is preserved and entered as a part of the commit message.
* On merge, after manual approval, the orb will automatically be published to the Orb Registry.


## Jobs

- [semantic-release](src/jobs/semantic-release.yml)
- [test](src/jobs/test.yml)

## Commands

- [install-packages](src/commands/install-packages.yml)

## Executors

- [default](src/executors/default.yml)

## Contributing

Too add a new job or command to the orb, please open a PR with your changes explaining in detail what the orb does. Also refer the the Orb Authoring docs.

## See:
 - [Orb Author Intro](https://circleci.com/docs/2.0/orb-author-intro/#section=configuration)
 - [Reusable Configuration](https://circleci.com/docs/2.0/reusing-config)
 - [Orb Concepts](https://circleci.com/docs/2.0/orb-author/?section=configuration)
