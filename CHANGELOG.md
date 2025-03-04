# Changelog

<sub>The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).</sub>

## [Unreleased]

## [0.4.0] - 2022-04-23

#### Added

- Update and copy methods:
    - Updating multiple fields at once is now directly possible from a pydantic model or
      a dictionary ([feature documentation](https://art049.github.io/odmantic/engine/#patching-multiple-fields-at-once),
      [sample use case with FastAPI](https://art049.github.io/odmantic/usage_fastapi/#updating-a-tree))
    - Changing the primary field of an instance is now easier
      ([documentation](https://art049.github.io/odmantic/engine/#changing-the-primary-field))

- Patch and copy Model instances ([#39](https://github.com/art049/odmantic/pull/39) by [@art049](https://github.com/art049))

#### Fixed

- Update example in README ([#192](https://github.com/art049/odmantic/pull/192) by [@jasper-moment](https://github.com/jasper-moment))

- Update README.md ([#129](https://github.com/art049/odmantic/pull/129) by [@Kludex](https://github.com/Kludex))

#### Internals

- ⬆️ Update motor requirement from >=2.1.0,<2.5.0 to >=2.1.0,<2.6.0 ([#160](https://github.com/art049/odmantic/pull/160) by [@dependabot[bot]](https://github.com/apps/dependabot))

- ⬆️ Update typer requirement from ^0.3.2 to ^0.4.1 ([#214](https://github.com/art049/odmantic/pull/214) by [@dependabot[bot]](https://github.com/apps/dependabot))

- ⬆️ Update mypy requirement from ^0.910 to ^0.942 ([#215](https://github.com/art049/odmantic/pull/215) by [@dependabot[bot]](https://github.com/apps/dependabot))

- ⬆️ Update fastapi requirement from >=0.61.1,<0.67.0 to >=0.61.1,<0.69.0 ([#166](https://github.com/art049/odmantic/pull/166) by [@dependabot[bot]](https://github.com/apps/dependabot))

- ⬆️ Update fastapi requirement from >=0.61.1,<0.64.0 to >=0.61.1,<0.67.0 ([#150](https://github.com/art049/odmantic/pull/150) by [@dependabot[bot]](https://github.com/apps/dependabot))

- ⬆️ Update mypy requirement from ^0.812 to ^0.910 ([#142](https://github.com/art049/odmantic/pull/142) by [@dependabot[bot]](https://github.com/apps/dependabot))

- ⬆️ Update pytest-asyncio requirement from ^0.14.0 to ^0.15.0 ([#125](https://github.com/art049/odmantic/pull/125) by [@dependabot[bot]](https://github.com/apps/dependabot))

- ⬆️ Update motor requirement from >=2.1.0,<2.4.0 to >=2.1.0,<2.5.0 ([#124](https://github.com/art049/odmantic/pull/124) by [@dependabot[bot]](https://github.com/apps/dependabot))

- ⬆️ Update importlib-metadata requirement from >=1,<4 to >=1,<5 ([#126](https://github.com/art049/odmantic/pull/126) by [@dependabot[bot]](https://github.com/apps/dependabot))

- ⬆️ Update pydocstyle requirement from ^5.1.1 to ^6.0.0 ([#119](https://github.com/art049/odmantic/pull/119) by [@dependabot[bot]](https://github.com/apps/dependabot))

- ⬆️ Update isort requirement from ~=5.7.0 to ~=5.8.0 ([#122](https://github.com/art049/odmantic/pull/122) by [@dependabot[bot]](https://github.com/apps/dependabot))

- ⬆️ Update flake8 requirement from ~=3.8.4 to ~=3.9.0 ([#116](https://github.com/art049/odmantic/pull/116) by [@dependabot[bot]](https://github.com/apps/dependabot))

## [0.3.5] - 2021-05-12

#### Security

- Change allowed pydantic versions to handle [CVE-2021-29510](https://github.com/samuelcolvin/pydantic/security/advisories/GHSA-5jqp-qgf6-3pvh) by [@art049](https://github.com/art049)

## [0.3.4] - 2021-03-04

#### Fixed

- Fix modified mark clearing on save for nested models ([#88](https://github.com/art049/odmantic/pull/88) by [@Olegt0rr](https://github.com/Olegt0rr))

- Don't replace default field description for ObjectId ([#82](https://github.com/art049/odmantic/pull/82) by [@Olegt0rr](https://github.com/Olegt0rr))

#### Internals

- Support pydantic 1.8 ([#113](https://github.com/art049/odmantic/pull/113) by [@art049](https://github.com/art049))

- Add nightly builds ([#114](https://github.com/art049/odmantic/pull/114) by [@art049](https://github.com/art049))

- CI Matrix with Standalone instances, ReplicaSets and Sharded clusters ([#91](https://github.com/art049/odmantic/pull/91) by [@art049](https://github.com/art049))

- Update mkdocstrings requirement from ^0.14.0 to ^0.15.0 ([#110](https://github.com/art049/odmantic/pull/110) by [@dependabot[bot]](https://github.com/apps/dependabot))

- Update mkdocs-material requirement from ^6.0.2 to ^7.0.3 ([#111](https://github.com/art049/odmantic/pull/111) by [@dependabot[bot]](https://github.com/apps/dependabot))

- Update mypy requirement from ^0.800 to ^0.812 ([#106](https://github.com/art049/odmantic/pull/106) by [@dependabot[bot]](https://github.com/apps/dependabot))

## [0.3.3] - 2021-02-13

#### Fixed

- Remove `bypass_document_validation` save option to avoid `Not Authorized` errors ([#85](https://github.com/art049/odmantic/pull/85) by [@Olegt0rr](https://github.com/Olegt0rr))

- Fix microseconds issue: use truncation instead of round ([#100](https://github.com/art049/odmantic/pull/100) by [@erny](https://github.com/erny))

- Add py.typed to ship typing information for mypy ([#101](https://github.com/art049/odmantic/pull/101) by [@art049](https://github.com/art049))

- Fix datetime field default example value naiveness ([#103](https://github.com/art049/odmantic/pull/103) by [@art049](https://github.com/art049))

#### Internals

- Update pytz requirement from ^2020.1 to ^2021.1 ([#98](https://github.com/art049/odmantic/pull/98) by [@dependabot[bot]](https://github.com/apps/dependabot))

- Update mkdocstrings requirement from ^0.13.2 to ^0.14.0 ([#92](https://github.com/art049/odmantic/pull/92) by [@dependabot[bot]](https://github.com/apps/dependabot))

- Update mypy requirement from ^0.790 to ^0.800 ([#97](https://github.com/art049/odmantic/pull/97) by [@dependabot[bot]](https://github.com/apps/dependabot))

- Update isort requirement from ~=5.6.4 to ~=5.7.0 ([#90](https://github.com/art049/odmantic/pull/90) by [@dependabot[bot]](https://github.com/apps/dependabot))

- Update fastapi requirement from >=0.61.1,<0.63.0 to >=0.61.1,<0.64.0 ([#84](https://github.com/art049/odmantic/pull/84) by [@dependabot[bot]](https://github.com/apps/dependabot))

## [0.3.2] - 2020-12-15

#### Added

- Fix embedded model field update ([#77](https://github.com/art049/odmantic/pull/77) by [@art049](https://github.com/art049))

- Fix `datetime` bson inheritance issue ([#78](https://github.com/art049/odmantic/pull/78) by [@Olegt0rr](https://github.com/Olegt0rr))

#### Internals

- Migrate to the updated prettier precommit hook ([#74](https://github.com/art049/odmantic/pull/74) by [@art049](https://github.com/art049))

- Fix tox dependency install ([#72](https://github.com/art049/odmantic/pull/72) by [@art049](https://github.com/art049))

- Update uvicorn requirement from ^0.12.1 to ^0.13.0 ([#67](https://github.com/art049/odmantic/pull/67) by [@dependabot[bot]](https://github.com/apps/dependabot))

- Update mypy requirement from ^0.782 to ^0.790 ([#48](https://github.com/art049/odmantic/pull/48) by [@dependabot[bot]](https://github.com/apps/dependabot-preview))

- Update importlib-metadata requirement from ^1.0 to >=1,<4 ([#54](https://github.com/art049/odmantic/pull/54) by [@dependabot[bot]](https://github.com/apps/dependabot))

- Update flake8 requirement from ==3.8.3 to ==3.8.4 ([#47](https://github.com/art049/odmantic/pull/47) by [@dependabot[bot]](https://github.com/apps/dependabot-preview))

- Update fastapi requirement from ^0.61.1 to >=0.61.1,<0.63.0 ([#59](https://github.com/art049/odmantic/pull/59) by [@dependabot[bot]](https://github.com/apps/dependabot))

## [0.3.1] - 2020-11-16

#### Added

- Add `schema_extra` config option ([#41](https://github.com/art049/odmantic/pull/41) by [@art049](https://github.com/art049))

#### Fixed

- Fix `setattr` error on a manually initialized EmbeddedModel ([#40](https://github.com/art049/odmantic/pull/40) by [@art049](https://github.com/art049))

## [0.3.0] - 2020-11-09

#### Deprecated

- Deprecate usage of `__collection__` to customize the collection name. Prefer the
  `collection` Config option ([more
  details](https://art049.github.io/odmantic/modeling/#collection))

#### Added

- Allow parsing document with unset fields defaults ([documentation](https://art049.github.io/odmantic/raw_query_usage/#advanced-parsing-behavior)) ([#28](https://github.com/art049/odmantic/pull/28) by [@art049](https://github.com/art049))

- Integration with Pydantic `Config` class ([#37](https://github.com/art049/odmantic/pull/37) by [@art049](https://github.com/art049)):

    - It's now possible to define custom `json_encoders` on the Models
    - Some other `Config` options provided by Pydantic are now available ([more
      details](https://art049.github.io/odmantic/modeling/#advanced-configuration))

- Support CPython 3.9 ([#32](https://github.com/art049/odmantic/pull/32) by
  [@art049](https://github.com/art049))

- Unpin pydantic to support 1.7.0 ([#29](https://github.com/art049/odmantic/pull/29) by
  [@art049](https://github.com/art049))

## [0.2.1] - 2020-10-25

#### Fixed

- Fix combined use of `skip` and `limit` with `engine.find` (#25 by @art049)

## [0.2.0] - 2020-10-25

#### Deprecated

- Deprecate `AIOEngineDependency` to prefer a global engine object, [more
  details](https://art049.github.io/odmantic/usage_fastapi/#building-the-engine) (#21 by
  @art049)

#### Added

- [Add sorting support](https://art049.github.io/odmantic/querying/#sorting) (#17 by @adriencaccia)
- Support motor 2.3.0 (#20 by @art049)

#### Fixed

- Fix FastAPI usage with References (#19 by @art049)

#### Docs

- Adding a CONTRIBUTING.md file to the root directory with link to docs (#8 by @sanders41)
- Raw Query Usage Documentation Fix (#10 by @adeelsohailahmed)
- Update Filtering to include Bitwise Operator Warning (#24 by @adeelsohailahmed)

## [0.1.0] - 2020-10-19

#### Initial Release

[0.1.0]: https://github.com/art049/odmantic/releases/tag/v0.1.0
[0.2.0]: https://github.com/art049/odmantic/compare/v0.1.0...v0.2.0
[0.2.1]: https://github.com/art049/odmantic/compare/v0.2.0...v0.2.1
[0.3.0]: https://github.com/art049/odmantic/compare/v0.2.1...v0.3.0
[0.3.1]: https://github.com/art049/odmantic/compare/v0.3.0...v0.3.1
[0.3.2]: https://github.com/art049/odmantic/compare/v0.3.1...v0.3.2
[0.3.3]: https://github.com/art049/odmantic/compare/v0.3.2...v0.3.3
[0.3.4]: https://github.com/art049/odmantic/compare/v0.3.3...v0.3.4
[0.3.5]: https://github.com/art049/odmantic/compare/v0.3.4...v0.3.5
[0.4.0]: https://github.com/art049/odmantic/compare/v0.3.5...v0.4.0
[unreleased]: https://github.com/art049/odmantic/compare/v0.4.0...HEAD
