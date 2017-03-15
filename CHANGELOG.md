# `stratic-date-in-path` changelog

`stratic-date-in-path` follows [Semantic Versioning][1].

## 3.0.0 - 2017-03-14

### Breaking

* Post data is expected to be on `file.data`, not `file` (straticjs/RFCs#2)

## 2.0.0 - 2016-05-28

### Fixed

* Fix an off-by-one error where January would result in a path with '00', February would be '01', etc.

## 1.0.0 - 2016-05-26

### Added

* Initial release

 [1]: http://semver.org/
