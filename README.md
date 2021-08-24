[![license][license-img]][license-url]
[![latest tag][latest-tag-img]][latest-tag-url]
[![latest release][latest-release-img]][latest-release-url]

[![build][build-img]][build-url]
[![analyze][analyze-img]][analyze-url]
[![dependabot][dependabot-img]][dependabot-url]

[![languages][languages-img]][languages-url]
[![alerts][alerts-img]][alerts-url]
[![code quality][code-quality-img]][code-quality-url]

[![lines of code][lines-of-code-img]][lines-of-code-url]
[![maintainability][maintainability-img]][maintainability-url]
[![technical debt][technical-debt-img]][technical-debt-url]

# keycloak-impersonation-policy-enforcer

This project provides a [Keycloak][keycloak] browser authenticator that
enforces an impersonation policy restricting impersonators from access
service providers (clients) unless holding a client role.

## usage

### deployment

Copy `keycloak-impersionation-policy-enforcer-«version».ear` to `${KEYCLOAK_HOME}/deployments`.

### configuration

TODO

## development

### project structure

This project follows the module/bundle approach to packaging keycloak extensions:

* `module` builds the jar that contains the keycloak extensions

* `bundle` builds the ear that contains the jar from `module` and any jars that are
  not designated as `provided` dependencies

### coding conventions

This project uses:

* [checkstyle][checkstyle] to achieve compliance with the [Google Java Style Guide][style-guide].
  Please add the checkstyle plugin to your IDE.

* [SonarLint][sonarlint] to improve code quality and code security.
  Please add the SonarLint plugin to your IDE.

---
Copyright 2021 Luca Filipozzi. Some rights reserved. See [LICENSE][license-url].

[keycloak]: https://keycloak.org/

[style-guide]: https://google.github.io/styleguide/javaguide.html
[checkstyle]: https://checkstyle.sourceforge.io/
[sonarlint]: https://www.sonarlint.org/

[latest-release-img]: https://badgen.net/github/release/LucaFilipozzi/keycloak-impersonation-policy-enforcer?icon=github&label=latest%20release
[latest-release-url]: https://github.com/LucaFilipozzi/keycloak-impersonation-policy-enforcer/releases/latest
[latest-tag-img]: https://badgen.net/github/tag/LucaFilipozzi/keycloak-impersonation-policy-enforcer?icon=github
[latest-tag-url]: https://github.com/LucaFilipozzi/keycloak-impersonation-policy-enforcer/tags
[license-img]: https://badgen.net/github/license/LucaFilipozzi/keycloak-impersonation-policy-enforcer?icon=github
[license-url]: https://github.com/LucaFilipozzi/keycloak-impersonation-policy-enforcer/blob/main/LICENSE

[analyze-img]: https://github.com/LucaFilipozzi/keycloak-impersonation-policy-enforcer/actions/workflows/analyze.yml/badge.svg
[analyze-url]: https://github.com/LucaFilipozzi/keycloak-impersonation-policy-enforcer/actions/workflows/analyze.yml
[build-img]: https://github.com/LucaFilipozzi/keycloak-impersonation-policy-enforcer/actions/workflows/build.yml/badge.svg
[build-url]: https://github.com/LucaFilipozzi/keycloak-impersonation-policy-enforcer/actions/workflows/build.yml
[dependabot-img]: https://badgen.net/github/dependabot/LucaFilipozzi/keycloak-impersonation-policy-enforcer?icon=dependabot
[dependabot-url]: https://github.com/LucaFilipozzi/keycloak-impersonation-policy-enforcer/network/dependencies

[languages-img]: https://badgen.net/lgtm/langs/g/LucaFilipozzi/keycloak-impersonation-policy-enforcer?icon=lgtm
[languages-url]: https://lgtm.com/projects/g/LucaFilipozzi/keycloak-impersonation-policy-enforcer/logs/languages/lang:java
[alerts-img]: https://badgen.net/lgtm/alerts/g/LucaFilipozzi/keycloak-impersonation-policy-enforcer/java?icon=lgtm
[alerts-url]: https://lgtm.com/projects/g/LucaFilipozzi/keycloak-impersonation-policy-enforcer/alerts
[code-quality-img]: https://badgen.net/lgtm/grade/g/LucaFilipozzi/keycloak-impersonation-policy-enforcer/java?icon=lgtm
[code-quality-url]: https://lgtm.com/projects/g/LucaFilipozzi/keycloak-impersonation-policy-enforcer/context:java

[lines-of-code-img]: https://badgen.net/codeclimate/loc/LucaFilipozzi/keycloak-impersonation-policy-enforcer?icon=codeclimate
[lines-of-code-url]: https://codeclimate.com/github/LucaFilipozzi/keycloak-impersonation-policy-enforcer
[maintainability-img]: https://badgen.net/codeclimate/maintainability/LucaFilipozzi/keycloak-impersonation-policy-enforcer?icon=codeclimate
[maintainability-url]: https://codeclimate.com/github/LucaFilipozzi/keycloak-impersonation-policy-enforcer/maintainability
[technical-debt-img]: https://badgen.net/codeclimate/tech-debt/LucaFilipozzi/keycloak-impersonation-policy-enforcer?icon=codeclimate
[technical-debt-url]: https://codeclimate.com/github/LucaFilipozzi/keycloak-impersonation-policy-enforcer/maintainability
