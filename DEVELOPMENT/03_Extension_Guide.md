# Extension Guide — K_PYPREP

**Company:** Anticloud FZ LLE

## Adding New Features

1. Fork the upstream codebase
2. Add integration hooks in `anticloud/` module
3. Ensure PAX inference path is tested offline
4. Add AIOSS audit entries for all mutations
5. Submit PR with AIOSS proof-of-integrity

## API Extension

All public APIs wrapped with AIOSS decorators.
New endpoints must declare `@aioss_audit` to be accepted.
