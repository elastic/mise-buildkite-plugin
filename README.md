# Mise Buildkite Plugin

> **Warning:** This plugin is currently in a **proof-of-concept** state and is not intended to be used.

## Example

Add the following to your `pipeline.yml`:

```yml
steps:
  - command: ls
    plugins:
      - elastic/mise#v1.0.1: ~
```
