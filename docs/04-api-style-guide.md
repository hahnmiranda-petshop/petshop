# Guia de Estilo para APIs

## Convenções de Endpoints
- Utilizar **kebab-case** para nomes de recursos.
- Versionamento no path (`/api/v1/...`).
- Usar **verbos HTTP** corretos:
  - GET: Consultas
  - POST: Criação
  - PUT: Atualização total
  - PATCH: Atualização parcial
  - DELETE: Remoção

## Respostas
- Padrão JSON.
- Estrutura uniforme para erros (`code`, `message`, `details`).

## Segurança
- Todas as APIs devem ser protegidas por autenticação.
