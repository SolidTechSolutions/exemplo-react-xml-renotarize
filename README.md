# SolidSign API - Example Front-end: XML Renotarization (React)

Example front-end for adding a new ArchiveTimeStamp (renotarization) to an
existing XML/XAdES signature. By default it talks to the
[`exemplo-integracao-xml-renotarize`](https://github.com/SolidTechSolutions/exemplo-integracao-xml-renotarize)
example backend, which keeps the API credentials server-side — the
recommended integration pattern. An optional "Direct to SolidSign API" mode
lets you call the API straight from the browser, useful for a quick manual
check, but it exposes the token in the browser.

## How it works

- **Default mode (backend)**: `POST http://localhost:8102/api/xml/renotarize/form`.
- **Optional mode (direct)**: `POST {baseUrl}/solidsign/dsig/extending/xml/add-archivetimestamp`, with the token entered in the form.

## Prerequisites

1. Run the [`exemplo-integracao-xml-renotarize`](https://github.com/SolidTechSolutions/exemplo-integracao-xml-renotarize) backend locally (`mvn spring-boot:run`, default port `8102`) — or, for direct mode, have a valid JWT token.
2. One or more signed (XAdES) XML files to renotarize.

## Running

```bash
npm install
npm run dev
```

Open `http://localhost:5173`, upload the XML(s) and renotarize.
