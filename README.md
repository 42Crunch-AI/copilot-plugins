# 42Crunch GitHub Copilot Plugins

The official [42Crunch](https://www.42crunch.com) plugin marketplace for GitHub Copilot — a catalog of AI-powered plugins that bring 42Crunch's API security capabilities directly into your GitHub Copilot workflow.

42Crunch plugins give Copilot the ability to audit OpenAPI specs, scan live APIs for vulnerabilities, and apply fixes to ensure APIs meet security guardrails.

## Structure

```
.github/plugin
  marketplace.json              # Plugin registry manifest
plugins/                        # Copilot plugins developed by 42Crunch
  api-security-testing/
    plugin.json                 # Plugin metadata
    skills/                     # Skill definitions
    references/                 # Reference definitions
    README.md                   # Documentation
    LICENSE                     # License
```

## Adding this Marketplace

Register the 42Crunch marketplace with GitHub Copilot once, then install any plugin from it:

```
copilot plugin marketplace add 42Crunch-AI/copilot-plugins
```

Or from an interactive Copilot session:

```
/plugin marketplace add 42Crunch-AI/copilot-plugins
```

## Available Plugins

### [api-security-testing](./plugins/api-security-testing/)

AI-powered API security plugin backed by 42Crunch. Audit OpenAPI specs, detect OWASP API Security vulnerabilities (including BOLA/BFLA), run live conformance and authorization scans against running APIs, and apply AI-assisted fixes — all through natural language.

**Install:**
After registering the marketplace (see above), install the plugin:

```
copilot plugin install api-security-testing@42crunch-marketplace
```

Or from an interactive Copilot session:

```
/plugin install api-security-testing@42crunch-marketplace
```

See the [plugin README](./plugins/api-security-testing/README.md) for full documentation.


## Links

- [42Crunch](https://42crunch.com/)
- [42Crunch Documentation](https://docs.42crunch.com)
- [42Crunch on GitHub](https://github.com/42Crunch)
- Support: support@42crunch.com
