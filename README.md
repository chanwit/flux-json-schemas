# Flux JSON Schemas

This experimental repo contains an auto-generated Flux JSON schemas for VSCode.

The schema requires the YAML extension. Here's how to find the settings for adding a new schema.

![Selection_516](https://user-images.githubusercontent.com/10666/141793911-2ab4a4fd-5b18-48d1-bdf0-659073f92755.png)

Inside your `settings.json`, add the following lines for example:
```json
{
    "yaml.maxItemsComputed": 5000,
    "yaml.schemas": {
        "https://raw.githubusercontent.com/chanwit/flux-json-schemas/main/flux_v0.23.0.json": ["*.yaml"]
    },
    "yaml.trace.server": "verbose",
    "yaml.disableAdditionalProperties": true
}
```

If you already used some YAML schemas, you need to add only this line to the "yaml.schemas" key,

```json
    "https://raw.githubusercontent.com/chanwit/flux-json-schemas/main/flux_v0.23.0.json": ["*.yaml"]
```
