# ADR 0006: Política de Configuração e Segredos

## Contexto
Foi preciso definir como gerenciar variáveis de configuração e segredos de forma segura.

## Decisão
Utilizar GitHub Secrets e config-server para armazenar segredos e configurações, evitando qualquer exposição em código.

## Consequências
Garante segurança, mas requer processos claros para atualização e rotação de segredos.
