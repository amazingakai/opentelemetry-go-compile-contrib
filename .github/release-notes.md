### Added

- Migrate instrumentation/ and pkg/ to contrib repo (#9)
- Migrate test suite and CI workflows to contrib repo (#22)
- Add clickhouse-go/v2 native API instrumentation (#54)
- Filter unwanted root spans (#51)
- Let instrumentation register resource detectors (#90)

### Fixed

- Update intra-repo pseudo-versions to latest commit (#41)
- Keep the detected resource when one detector reports an error (#48)
- Prevent Oracle password disclosure (#86)
- Split NewClient rule at v1.81.0 for native tracing (#89)
- Skip leading comments when naming the operation (#58)
- Name client spans "{operation} {namespace}" (#53)
- Correct version matrix lower bounds for stripe, linodego, and amqp091 (#88)
- Report the first broker when a writer has several (#52)
- Report the first host of a ClickHouse host list (#49)
- Look for the MySQL address parentheses only before the database name (#46)
- Leave a shutdown signal alone when it is ignored at startup (#57)

### Changed

- Drop runtime instrumentation (#23)
- Add no imports from the SDK init and sdk/trace files (#56)

## What's Changed
* chore: initial repository setup by @darkraider01 in https://github.com/open-telemetry/opentelemetry-go-compile-contrib/pull/8
* ci: move security scanning to shared workflow by @opentelemetrybot in https://github.com/open-telemetry/opentelemetry-go-compile-contrib/pull/10
* chore(deps): update github actions by @renovate[bot] in https://github.com/open-telemetry/opentelemetry-go-compile-contrib/pull/2
* Update github actions (major) by @renovate[bot] in https://github.com/open-telemetry/opentelemetry-go-compile-contrib/pull/3
* chore(ci): use regular zizmor persona by @trask in https://github.com/open-telemetry/opentelemetry-go-compile-contrib/pull/13
* docs: migrate docs/instrument-guide.md from otelc with full history by @om7057 in https://github.com/open-telemetry/opentelemetry-go-compile-contrib/pull/11
* chore: address initial repo setup gaps and follow-up items by @darkraider01 in https://github.com/open-telemetry/opentelemetry-go-compile-contrib/pull/12
* fix(deps): update module github.com/golangci/golangci-lint/v2 to v2.14.0 by @renovate[bot] in https://github.com/open-telemetry/opentelemetry-go-compile-contrib/pull/14
* feat: migrate instrumentation/ and pkg/ to contrib repo by @amazingakai in https://github.com/open-telemetry/opentelemetry-go-compile-contrib/pull/9
* chore(deps): update module github.com/klauspost/compress to v1.18.7 [security] by @renovate[bot] in https://github.com/open-telemetry/opentelemetry-go-compile-contrib/pull/19
* fix(deps): update module github.com/golangci/golangci-lint/v2 to v2.15.0 by @renovate[bot] in https://github.com/open-telemetry/opentelemetry-go-compile-contrib/pull/16
* fix(deps): update go.opentelemetry.io/contrib/instrumentation/go.mongodb.org/mongo-driver/v2/mongo/otelmongo digest to e9cd3e0 by @renovate[bot] in https://github.com/open-telemetry/opentelemetry-go-compile-contrib/pull/17
* chore(deps): update github actions by @renovate[bot] in https://github.com/open-telemetry/opentelemetry-go-compile-contrib/pull/15
* feat: migrate test suite and CI workflows to contrib repo by @amazingakai in https://github.com/open-telemetry/opentelemetry-go-compile-contrib/pull/22
* refactor: drop runtime instrumentation by @amazingakai in https://github.com/open-telemetry/opentelemetry-go-compile-contrib/pull/23
* fix(deps): update module github.com/aws/aws-sdk-go-v2 to v1.48.0 by @renovate[bot] in https://github.com/open-telemetry/opentelemetry-go-compile-contrib/pull/27
* chore: sync upstream otelc changes (1689..1841) by @amazingakai in https://github.com/open-telemetry/opentelemetry-go-compile-contrib/pull/40
* fix: update intra-repo pseudo-versions to latest commit by @amazingakai in https://github.com/open-telemetry/opentelemetry-go-compile-contrib/pull/41
* fix(pkg/runtime): keep the detected resource when one detector reports an error by @vignesh2027 in https://github.com/open-telemetry/opentelemetry-go-compile-contrib/pull/48
* fix(instrumentation/database/sql): prevent Oracle password disclosure by @amazingakai in https://github.com/open-telemetry/opentelemetry-go-compile-contrib/pull/86
* fix(instrumentation/anthropic): split NewClient rule at v1.81.0 for native tracing by @Aryanbhargava18 in https://github.com/open-telemetry/opentelemetry-go-compile-contrib/pull/89
* docs: overhaul documentation for initial release by @amazingakai in https://github.com/open-telemetry/opentelemetry-go-compile-contrib/pull/43
* fix(instrumentation/database/sql): skip leading comments when naming the operation by @Elvand-Lie in https://github.com/open-telemetry/opentelemetry-go-compile-contrib/pull/58
* refactor(instrumentation/otel): add no imports from the SDK init and sdk/trace files by @Itz-Agasta in https://github.com/open-telemetry/opentelemetry-go-compile-contrib/pull/56
* feat(instrumentation): add clickhouse-go/v2 native API instrumentation by @akshatagarwl in https://github.com/open-telemetry/opentelemetry-go-compile-contrib/pull/54
* fix(instrumentation/database/sql): name client spans "{operation} {namespace}" by @akshatagarwl in https://github.com/open-telemetry/opentelemetry-go-compile-contrib/pull/53
* fix(instrumentation): correct version matrix lower bounds for stripe, linodego, and amqp091 by @Aryanbhargava18 in https://github.com/open-telemetry/opentelemetry-go-compile-contrib/pull/88
* fix(otelckafka): report the first broker when a writer has several by @vignesh2027 in https://github.com/open-telemetry/opentelemetry-go-compile-contrib/pull/52
* fix(database/sql): report the first host of a ClickHouse host list by @vignesh2027 in https://github.com/open-telemetry/opentelemetry-go-compile-contrib/pull/49
* fix(database/sql): look for the MySQL address parentheses only before the database name by @vignesh2027 in https://github.com/open-telemetry/opentelemetry-go-compile-contrib/pull/46
* fix(pkg/runtime): leave a shutdown signal alone when it is ignored at startup by @Elvand-Lie in https://github.com/open-telemetry/opentelemetry-go-compile-contrib/pull/57
* feat(runtime): filter unwanted root spans by @darkraider01 in https://github.com/open-telemetry/opentelemetry-go-compile-contrib/pull/51
* chore(deps): bump github.com/klauspost/compress from 1.18.0 to 1.18.7 in /.tools by @dependabot[bot] in https://github.com/open-telemetry/opentelemetry-go-compile-contrib/pull/32
* chore(deps): bump github.com/docker/cli from 28.3.0+incompatible to 29.2.0+incompatible in /.tools by @dependabot[bot] in https://github.com/open-telemetry/opentelemetry-go-compile-contrib/pull/31
* chore(deps): bump go.opentelemetry.io/otel/trace from 1.46.0 to 1.47.0 in /instrumentation/github.com/segmentio/kafka-go/otelckafka by @dependabot[bot] in https://github.com/open-telemetry/opentelemetry-go-compile-contrib/pull/24
* feat(pkg/runtime): let instrumentation register resource detectors by @wpessers in https://github.com/open-telemetry/opentelemetry-go-compile-contrib/pull/90

## New Contributors
* @darkraider01 made their first contribution in https://github.com/open-telemetry/opentelemetry-go-compile-contrib/pull/8
* @opentelemetrybot made their first contribution in https://github.com/open-telemetry/opentelemetry-go-compile-contrib/pull/10
* @renovate[bot] made their first contribution in https://github.com/open-telemetry/opentelemetry-go-compile-contrib/pull/2
* @trask made their first contribution in https://github.com/open-telemetry/opentelemetry-go-compile-contrib/pull/13
* @om7057 made their first contribution in https://github.com/open-telemetry/opentelemetry-go-compile-contrib/pull/11
* @vignesh2027 made their first contribution in https://github.com/open-telemetry/opentelemetry-go-compile-contrib/pull/48
* @Aryanbhargava18 made their first contribution in https://github.com/open-telemetry/opentelemetry-go-compile-contrib/pull/89
* @Elvand-Lie made their first contribution in https://github.com/open-telemetry/opentelemetry-go-compile-contrib/pull/58
* @Itz-Agasta made their first contribution in https://github.com/open-telemetry/opentelemetry-go-compile-contrib/pull/56
* @akshatagarwl made their first contribution in https://github.com/open-telemetry/opentelemetry-go-compile-contrib/pull/54
* @dependabot[bot] made their first contribution in https://github.com/open-telemetry/opentelemetry-go-compile-contrib/pull/32
* @wpessers made their first contribution in https://github.com/open-telemetry/opentelemetry-go-compile-contrib/pull/90

**Full Changelog**: https://github.com/open-telemetry/opentelemetry-go-compile-contrib/commits/v0.1.0
