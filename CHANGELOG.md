# Changelog

All notable changes to this project will be documented in this file.

The format is based on Keep a Changelog and this project adheres (loosely) to Semantic Versioning.

## [2.3.0] - 2025-09-29
### Added
- `--regions-from-file` option to map differing region names across multiple ROOT files.
- `--list-regions` option to discover available region directories containing a `cutflow` histogram.
- Support for per-file region name mapping with canonical display naming.
- Enhanced error messages suggesting closest region names when a region is missing.
- Option `--separate-selections` now pads mismatched selection lengths instead of failing.
- Strict behavior in merged (default) mode: mismatched selection lengths now skip the region.
- Colored banners and hints for selection length mismatches.
- Added `__version__` constant in `cutflow_compare.__init__` for programmatic access.

### Changed
- Version bumped from 2.2.0 to 2.3.0 in `setup.py`, `pyproject.toml`, and `__init__.py`.
- README updated with new feature documentation, region mapping examples, and publishing instructions.
- Improved description in packaging metadata.

### Fixed
- Avoided DataFrame length mismatch crashes by padding only when `--separate-selections` is used.

### Maintenance
- Added `CHANGELOG.md`.

## [2.2.0] - 2025-??-??
- Previous stable release (details not retroactively recorded).

[2.3.0]: https://github.com/ibeuler/cutflow_compare/releases/tag/v2.3.0
