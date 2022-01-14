# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

### Added

* Content-encoding message property (for AMQP Publisher).
* Queue x-max-priority & message priority parameters (see jlavallee#42). Thanks to [@gregLibert](https://github.com/gregLibert), [@looseend](https://github.com/looseend).
* Request (for AMQP Publisher) and Response (for AMQP Consumer) headers.
* Option to configure transactional AMQP consumer from the UI (see jlavallee#38). Thanks to [@nicklasbondesson](https://github.com/nicklasbondesson).
* Auto-delete property for exchange (see jlavallee#33). Thanks to [@wneild](https://github.com/wneild).
* Heartbeat option (see zeph1rus/JMeter-Rabbit-AMQP@efddefa). Thanks to [@zeph1rus](https://github.com/zeph1rus).
* Jar with dependencies.
* Extra exception handling.

### Changed

* Maven instead of ant & ivy.
* Switch to maven directory layout.
* Switch to SLF4J API for logging.
* Samplers configuration screens adjusted.
* Scenario example updated.
* Code cleanup.

### Deprecated

### Removed

* Redundant dependencies removed.

### Fixed

* No header in reply-to message issue (see jlavallee#41). Thanks to [@gregLibert](https://github.com/gregLibert).
* Checkstyle issues.

### Dependency Updates

* Up jmeter-core version to 5.4.3.
* Up amqp-client version to 4.12.0.
* Up commons-lang3 version to 3.12.0.
