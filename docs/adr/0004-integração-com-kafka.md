# ADR 0004: Integração com Kafka

## Contexto
Foi necessário escolher um mecanismo de mensageria confiável para comunicação assíncrona entre serviços.

## Decisão
Usaremos Apache Kafka com Spring Cloud Stream, seguindo um padrão de nomenclatura e versionamento de eventos.

## Consequências
Melhora a escalabilidade e desacoplamento, mas adiciona complexidade operacional.
