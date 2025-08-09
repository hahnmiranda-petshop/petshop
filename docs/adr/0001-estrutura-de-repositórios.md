# ADR 0001: Estrutura de Repositórios

## Contexto
O repositório `petshop` é o ponto central de documentação, governança e templates.

## Decisão
Cada serviço (ex.: gateway, config-server, people-service) possui seu próprio repositório independente, com pipelines, issues e versionamento separados.

## Consequências
Facilita escalabilidade, porém exige maior coordenação entre equipes (quando houver) e gestão de múltiplos pipelines.
