# JavaFX Scientific Calculator

JavaFX calculator with expression evaluation, MariaDB history, and JSON/XML handling.

Requires JDK 23 or newer, Maven, and MariaDB for database history.

```sh
cd calculator
mvn javafx:run
```

The interface supports arithmetic expressions, parentheses, powers, square roots,
factorials, and calculation history. The `%` operation follows the original
percentage behavior rather than integer remainder.

For database history, create an empty MariaDB database named `Calculator` and set
`DB_USER` and `DB_PASSWORD` in your shell. Optionally set `DB_URL` (defaults to
`jdbc:mariadb://localhost:3306/Calculator`). The application includes history-table creation.
On Windows, use `$env:DB_USER = "calculator_user"` and
`$env:DB_PASSWORD = "your-local-password"` in PowerShell before launching Maven.

This is a coursework snapshot. Expression edge cases and error handling need more
tests; the existing Maven test is a starter smoke test, not calculation coverage.

## Project background

A group coursework project. This portfolio copy does not claim sole authorship; original contributors are credited below. See [ATTRIBUTION.md](ATTRIBUTION.md) for the original repository, source revision, and contributor names.

This repository is a portfolio snapshot of existing coursework. Runtime limitations are documented above; publishing it does not imply production readiness.

