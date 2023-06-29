# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

See this project's [releases](/../../../releases).

<!-- Types of Changes -->
<!-- ### Added -->
<!-- ### Changed -->
<!-- ### Deprecated -->
<!-- ### Removed -->
<!-- ### Fixed -->
<!-- ### Security -->
<!-- ### Notes -->

## [Unreleased]

Will become version 2.0.0.

TODO

## [1.1.9] - 2023-05-20

### Changed

- Styling.

## [1.1.8] - 2023-05-13

### Fixed

- Under Linux the color picker was not displayed.

## [1.1.7] - 2023-05-04

### Added

- It is possible to use wildcard ( \* ) for excluding languages. e.g.: ad-\* will exclude every codeblock where the language starts with ad- (ad-example, ad-bug, ad-summary etc.). The wildcard can be either at the beginning or at the end.

### Fixed

- Incorrect display of the header when using minimal theme and "Readable line length" was enabled.
- Printing to a PDF did not work until now. Now it works.

## [1.1.6] - 2023-04-23

### Fixed

- Incorrectly handled inline code in ReadingView.

## [1.1.5] - 2023-03-21

### Changed

- Refactored code.

### Fixed

- Fixed the bug mentioned in [1.1.4].

## [1.1.4] - 2023-03-19

### Fixed

- Added partial workaround for bug identified in [notes](#notes)

### Notes

Found a very strange bug, but most people won't even notice it. I added a workaround which unfortunately is not a 100% percent solution (maybe around 90%). This bug however originates either from Obsidian or CodeMirror itself. I am still investigating.

If a document is opened (only in editing mode), then in very rare cases the viewport is not processed to the end. This results, that the line numbers, background colors, and other styles are not set for those code block lines. As I said, it occurs in very rare cases, and the workaround helps, but it is not a permanent solution.

## [1.1.3] - 2023-03-18

### Fixed

- Fixed a minor bug in ReadingView.

## [1.1.2] - 2023-03-17

### Fixed

- Corrected minor bug in reading view - Thanks for [@mnaoumov](https://github.com/mnaoumov) for noticing it, and submitting a PR!

## [1.1.1] - 2023-03-16

### Fixed

- Corrected bug where line number was displayed incorrectly when a very long line was displayed which overflowed to multiple lines.
- Corrected bug where when the header was collapsed and below another codeblock was displayed without header, it appeared as it belonged to the header.

## [1.1.0] - 2023-03-14

### Added

- Feature: Add alternative highlights.
- Feature: Display language icons in header.

### Changed

- Line numbers in editing mode are displayed just as line numbers in reading mode. This change was necessary.

### Fixed

- Fixed a bug, which caused the text in the header to be displayed always in lower case.
- Fixed a bug, which caused unnecessary execution.

## [1.0.2] - 2023-02-07

### Changed

- Implemented changes recommended by the Obsidian team.

## [1.0.1] - 2023-01-29

### Added

- The theme is set now automatically according to the Obsidian theme.

### Fixed

- Corrected that empty lines were not shown in reading mode.

## [1.0.0] - 2023-01-25

### Added

- Initial plugin code added.

[Unreleased]: /../../../compare/mugiwara85:CodeblockCustomizer:1.1.9...HEAD
[1.1.9]: /../../../compare/mugiwara85:CodeblockCustomizer:1.1.8...mugiwara85:CodeblockCustomizer:1.1.9
[1.1.8]: /../../../compare/mugiwara85:CodeblockCustomizer:1.1.7...mugiwara85:CodeblockCustomizer:1.1.8
[1.1.7]: /../../../compare/mugiwara85:CodeblockCustomizer:1.1.6...mugiwara85:CodeblockCustomizer:1.1.7
[1.1.6]: /../../../compare/mugiwara85:CodeblockCustomizer:1.1.5...mugiwara85:CodeblockCustomizer:1.1.6
[1.1.5]: /../../../compare/mugiwara85:CodeblockCustomizer:1.1.4...mugiwara85:CodeblockCustomizer:1.1.5
[1.1.4]: /../../../compare/mugiwara85:CodeblockCustomizer:1.1.3...mugiwara85:CodeblockCustomizer:1.1.4
[1.1.3]: /../../../compare/mugiwara85:CodeblockCustomizer:1.1.2...mugiwara85:CodeblockCustomizer:1.1.3
[1.1.2]: /../../../compare/mugiwara85:CodeblockCustomizer:1.1.1...mugiwara85:CodeblockCustomizer:1.1.2
[1.1.1]: /../../../compare/mugiwara85:CodeblockCustomizer:1.1.0...mugiwara85:CodeblockCustomizer:1.1.1
[1.1.0]: /../../../compare/mugiwara85:CodeblockCustomizer:1.0.2...mugiwara85:CodeblockCustomizer:1.1.0
[1.0.2]: /../../../compare/mugiwara85:CodeblockCustomizer:1.0.1...mugiwara85:CodeblockCustomizer:1.0.2
[1.0.1]: /../../../compare/mugiwara85:CodeblockCustomizer:1.0.0...mugiwara85:CodeblockCustomizer:1.0.1
[1.0.0]: /../../../releases/tag/1.0.0