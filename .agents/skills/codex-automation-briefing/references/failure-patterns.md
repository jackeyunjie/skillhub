# Failure Patterns

Common failures:

- goal exists but sources are undefined
- output style exists but output path is missing
- multiple unrelated jobs are packed into one automation
- failure handling is omitted

Default response:

- report which source or dependency failed
- keep partial success explicit
- do not pretend the run fully succeeded

