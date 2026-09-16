# Verification plan — Baldur's Gate 3

Status: NOT RUN. There is no executable implementation to test.

## Module acceptance criteria

### 1. Party resource scenarios

- [ ] Define a versioned input fixture specifically for party resource scenarios.
- [ ] Document the expected output and units before implementation.
- [ ] Test valid, missing, malformed, and unsupported-version inputs.
- [ ] Repeat with the same fixture and compare results.
- [ ] Confirm that source files and unrelated settings remain unchanged.

### 2. Save-copy checkpoints

- [ ] Define a versioned input fixture specifically for save-copy checkpoints.
- [ ] Document the expected output and units before implementation.
- [ ] Test valid, missing, malformed, and unsupported-version inputs.
- [ ] Repeat with the same fixture and compare results.
- [ ] Confirm that source files and unrelated settings remain unchanged.

### 3. Build-specific option notes

- [ ] Define a versioned input fixture specifically for build-specific option notes.
- [ ] Document the expected output and units before implementation.
- [ ] Test valid, missing, malformed, and unsupported-version inputs.
- [ ] Repeat with the same fixture and compare results.
- [ ] Confirm that source files and unrelated settings remain unchanged.

## Release gate

- [ ] Implement the proposed modules and add automated tests.
- [ ] Record exact tested versions; leave untested versions marked unknown.
- [ ] Verify backups and restoration where state changes are supported.
- [ ] Review privacy, permissions, and product rules.
- [ ] Publish source and reproducible build instructions before claiming a working release.
- [ ] Do not present the retained external resource as a verified download.

## Scope

Only user-owned local scenarios and manual notes. Offline availability and parameter editing for a particular build are NOT verified. No online-match features, ranking changes, or online currency operations. No process modification is implemented. Any future testing needs a separate save copy and a review of game rules.
