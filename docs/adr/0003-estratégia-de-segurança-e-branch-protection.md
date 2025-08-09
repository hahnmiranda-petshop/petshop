# ADR 0003: Estratégia de Segurança e Branch Protection

## Contexto
Definir regras para proteger a integridade do código e evitar commits inseguros na branch principal.

## Decisão
Ativar proteção da branch `main`, exigir PRs com revisão obrigatória, habilitar Secret Scanning, Dependabot e Code Scanning.

## Consequências
Aumenta a segurança e qualidade do código, mas pode alongar o tempo de entrega de mudanças.
