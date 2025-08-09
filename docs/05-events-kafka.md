# Eventos no Kafka

## Padrão de Mensagens
- Formato JSON.
- Incluir `eventId`, `timestamp` e `payload`.

## Tópicos
- Nomeação: `servico.evento.versao` (ex: `pet.created.v1`).

## Boas Práticas
- Publicar apenas eventos necessários.
- Garantir idempotência no consumo.
