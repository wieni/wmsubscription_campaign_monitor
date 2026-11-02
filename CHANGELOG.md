# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [2.0.0] - 2026-11-02
### Added
- Drupal 9, 10 and 11 support (`core_version_requirement: ^9 || ^10 || ^11`), tested on Drupal 11.4 with PHP 8.5
- Allow `campaignmonitor/createsend-php` ^7.1 next to ^6.1. 7.x no longer calls `utf8_encode()`
  (deprecated since PHP 8.2); `curl_close()` (deprecated since PHP 8.5) is still called by both
  versions until https://github.com/campaignmonitor/createsend-php/pull/129 is merged

### Removed
- **Breaking:** Drupal 8 support (`core: 8.x`) and PHP < 8.1. Drupal 8 sites keep using 1.0.0.

## [1.0.0] - 2020-09-16
Initial release
