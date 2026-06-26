# Changelog

All notable changes to this project will be documented in this file.

## [3.0.0] - 2026-06-26

### Changed
- Updated the default service URL to include the `/companies` path segment
  (`https://api.hubapi.com/crm/v3/objects/companies`). Resource paths no longer carry
  the `/companies` prefix (e.g. `companies/batch/read` → `batch/read`). This is a
  breaking change — existing callers must update resource call sites and any custom
  `serviceUrl` values.
- Improved operation summaries for all client resource methods.
