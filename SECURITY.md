# Security Policy

## What this project is (and is not)

Social Agent Suite is a set of instruction files and small local,
dependency-free Python tools. The skills:

- **never** ask for, store or transmit platform passwords or tokens,
- **never** connect to a social platform by themselves,
- run their tools entirely on the user's own machine, on the user's own
  text, with no network calls.

Publishing and engagement happen through the hosting agent's own approved
routes (official CLIs, the platform's own app, a browser the user controls),
under the user's approval rules.

## Reporting a vulnerability

If you find a security problem — for example a tool that leaks data, a
skill instruction that would exfiltrate user information, or a dependency
or script doing something undocumented — please do **not** open a public
issue. Contact the maintainer privately via the contact links on the
GitHub profile of the repository owner, with:

- a description of the problem,
- the file(s) involved,
- steps to reproduce, if applicable.

You will get a response as soon as reasonably possible, and a fix or a
documented decision will follow in the repository changelog.

## Supported versions

Only the latest state of the `main` branch is supported.
