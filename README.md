# Country Travel Information

Hasura query action handler for reading country travel information.

## Development Environment

A batch file to set environment variables, named `set_env.bat`, can be useful.

```
@ECHO OFF
SET COVID_DB_HOST=<host>
SET COVID_DB_NAME=<db-name>
SET COVID_DB_USER=<db-user>
SET COVID_DB_PASS=<password>
```

### Run Example

```bash
uvicorn main:app --reload --no-use-colors
```
