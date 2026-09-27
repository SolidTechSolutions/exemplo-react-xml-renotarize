# 🇧🇷 SolidSign API - Front-end de Exemplo: Renotarização (ArchiveTimeStamp) XML (React)

## Como funciona

"Via example backend" (padrão) chama `POST /api/xml/renotarize/form` no back-end de exemplo (`http://localhost:8102`), que repassa pra `POST /solidsign/dsig/extending/xml/add-archivetimestamp` da SolidSign API. "Direct to SolidSign API" (opcional) chama a API direto do navegador.

## Requisitos

Rode **um** destes back-ends de exemplo localmente (portas diferentes — ajuste `backendUrl` no formulário pra combinar):

- **Java** (porta 8102): [`exemplo-integracao-xml-renotarize`](https://github.com/SolidTechSolutions/exemplo-integracao-xml-renotarize)
- **C#** (porta 5099): [`exemplo-csharp-integracao-xml-renotarize`](https://github.com/SolidTechSolutions/exemplo-csharp-integracao-xml-renotarize)
- **JavaScript** (porta 8101): [`exemplo-javascript-integracao-xml-renotarize`](https://github.com/SolidTechSolutions/exemplo-javascript-integracao-xml-renotarize)
- **TypeScript** (porta 8101): [`exemplo-typescript-integracao-xml-renotarize`](https://github.com/SolidTechSolutions/exemplo-typescript-integracao-xml-renotarize)
- **Node.js** (porta 3101): [`exemplo-nodejs-integracao-xml-renotarize`](https://github.com/SolidTechSolutions/exemplo-nodejs-integracao-xml-renotarize)
- **PHP** (porta 8101): [`exemplo-php-integracao-xml-renotarize`](https://github.com/SolidTechSolutions/exemplo-php-integracao-xml-renotarize)
- **Python** (porta 8101): [`exemplo-python-integracao-xml-renotarize`](https://github.com/SolidTechSolutions/exemplo-python-integracao-xml-renotarize)

- Um token JWT válido (`POST /solidsign/auth/token`)

## Como rodar

```bash
npm install
npm run dev
```

Abra `http://localhost:5173`, preencha o formulário e envie.

## Variáveis do formulário

| Campo | Significado | Default |
|---|---|---|
| `mode` | Via backend de exemplo (padrão) ou direto à API | `backend` |
| `backendUrl` | URL do back-end de exemplo | `http://localhost:8102` |
| `authorization` | Token JWT (Bearer) | (vazio) |
| `documents` | Documento(s) a carimbar | (vazio) |
| `hashAlgorithm` | Algoritmo de hash | `SHA256` |
| `canonicalizationMethod` | Método de canonicalização | `EXCLUSIVE` |
| `nodeId / nodeName` | Nó a carimbar (opcional) | (vazio) |

---

# 🇬🇧 SolidSign API - Example Front-end: XML Renotarization (ArchiveTimeStamp) (React)

## How it works

"Via example backend" (default) calls `POST /api/xml/renotarize/form` on the example backend (`http://localhost:8102`), which forwards to `POST /solidsign/dsig/extending/xml/add-archivetimestamp` on the SolidSign API. "Direct to SolidSign API" (optional) calls the API straight from the browser.

## Requirements

Run **one** of these example backends locally (different ports — adjust `backendUrl` in the form to match):

- **Java** (port 8102): [`exemplo-integracao-xml-renotarize`](https://github.com/SolidTechSolutions/exemplo-integracao-xml-renotarize)
- **C#** (port 5099): [`exemplo-csharp-integracao-xml-renotarize`](https://github.com/SolidTechSolutions/exemplo-csharp-integracao-xml-renotarize)
- **JavaScript** (port 8101): [`exemplo-javascript-integracao-xml-renotarize`](https://github.com/SolidTechSolutions/exemplo-javascript-integracao-xml-renotarize)
- **TypeScript** (port 8101): [`exemplo-typescript-integracao-xml-renotarize`](https://github.com/SolidTechSolutions/exemplo-typescript-integracao-xml-renotarize)
- **Node.js** (port 3101): [`exemplo-nodejs-integracao-xml-renotarize`](https://github.com/SolidTechSolutions/exemplo-nodejs-integracao-xml-renotarize)
- **PHP** (port 8101): [`exemplo-php-integracao-xml-renotarize`](https://github.com/SolidTechSolutions/exemplo-php-integracao-xml-renotarize)
- **Python** (port 8101): [`exemplo-python-integracao-xml-renotarize`](https://github.com/SolidTechSolutions/exemplo-python-integracao-xml-renotarize)

- A valid JWT token (`POST /solidsign/auth/token`)

## Running

```bash
npm install
npm run dev
```

Open `http://localhost:5173`, fill in the form and submit.

## Form fields

| Field | Meaning | Default |
|---|---|---|
| `mode` | Via example backend (default) or direct to API | `backend` |
| `backendUrl` | Example backend URL | `http://localhost:8102` |
| `authorization` | JWT (Bearer) token | (empty) |
| `documents` | Document(s) to timestamp | (empty) |
| `hashAlgorithm` | Hash algorithm | `SHA256` |
| `canonicalizationMethod` | Canonicalization method | `EXCLUSIVE` |
| `nodeId / nodeName` | Node to timestamp (optional) | (empty) |
