# Mise Buildkite Plugin

A [Buildkite plugin](https://buildkite.com/docs/pipelines/integrations/plugins) that makes using [mise](https://mise.jdx.dev/) delightful in CI.

Mise is a fast, polyglot development tool that manages development tools, runtime versions (like Node, Python, Go), environment variables, and tasks on a per-project basis. It works by using a `mise.toml` file to create consistent environments, functioning as a faster alternative to `asdf`, `direnv`, `hermit` and similar tools.

## Example

Add the following to your `pipeline.yml`:

```yml
steps:
  - command: ls
    plugins:
      - elastic/mise#v1.0.1: ~
```
