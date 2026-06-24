# Vectros API — OpenAPI Specification

The canonical [OpenAPI 3](https://www.openapis.org/) description of the
**Vectros AI Platform API** — hybrid search, document ingestion, structured
records, and inference for your application.

| File | What it is |
|---|---|
| [`openapi.yaml`](./openapi.yaml) | The full OpenAPI 3 spec for the Vectros API. |
| [`llms.txt`](./llms.txt) | A condensed, LLM-friendly index of the API for use with coding assistants. |

## Using the spec

`openapi.yaml` is a standard OpenAPI document — point any compatible tool at it
to explore the API, generate a client, or drive contract tests. For example:

```bash
# Preview locally
npx @redocly/cli preview-docs openapi.yaml

# Generate a client in your language of choice
npx @openapitools/openapi-generator-cli generate -i openapi.yaml -g <generator> -o ./client
```

## Official SDKs

You usually don't need to generate your own client — Vectros publishes
maintained SDKs:

- **TypeScript / JavaScript** — [`@vectros-ai/sdk`](https://www.npmjs.com/package/@vectros-ai/sdk) ([source](https://github.com/vectros-ai/vectros-sdk-node))
- **Python** — [`vectros`](https://pypi.org/project/vectros/) ([source](https://github.com/vectros-ai/vectros-sdk-python))
- **Java** — [`ai.vectros:vectros-sdk`](https://central.sonatype.com/artifact/ai.vectros/vectros-sdk) ([source](https://github.com/vectros-ai/vectros-sdk-java))

## Documentation

Full guides and reference live at **[developers.vectros.ai](https://developers.vectros.ai)**.

## Notes

This repository is a **read-only mirror** — the spec is generated and published
automatically on each release, so changes made here directly will be overwritten.
Please report API issues or documentation feedback at
[vectros.ai](https://vectros.ai).

## License

Released under the [Apache License 2.0](./LICENSE).
