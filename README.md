<div align="center">
  <img src="share/orla_registry.png"></img>
</div>

---

Tools registry for the [orla](https://github.com/dorcha-inc/orla) MCP framework.

## Using the Registry

Install tools from this registry using:

```bash
orla install TOOL-NAME
```

For example:

```bash
orla install coinflip
```

## Adding Tools

To add a new tool to the registry:

1. Create a tool repository following the [orla RFC 3 tool package format](https://github.com/dorcha-inc/orla/blob/main/docs/rfcs/rfc3.txt)
2. Add an entry to `registry.yaml` with the tool's metadata
3. Submit a pull request

## Registry Format

The `registry.yaml` file follows this structure:

```yaml
version: 1
registry_url: https://github.com/dorcha-inc/orla-registry
tools:
  - name: tool-name
    description: Tool description
    repository: https://github.com/user/orla-tool-name
    versions:
      - version: 0.1.0
        tag: v0.1.0
    maintainer: maintainer-name
    keywords:
      - keyword1
      - keyword2
```
