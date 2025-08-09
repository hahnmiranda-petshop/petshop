# Arquitetura do Sistema

O sistema adota uma **arquitetura baseada em microsserviços**, onde cada serviço é independente e se comunica preferencialmente por eventos assíncronos (Kafka) ou APIs REST.

## Componentes Principais
- **Gateway API**: Ponto único de entrada para as requisições externas.
- **Shared Libraries**: Bibliotecas compartilhadas entre serviços, contendo utilitários, DTOs e contratos de comunicação.
- **Serviços de Domínio**: Implementam as regras de negócio específicas de cada módulo.
- **Config Server**: Centraliza as configurações dos serviços.
- **Kafka**: Intermedia a comunicação assíncrona entre serviços.
- **Banco de Dados**: Cada serviço mantém seu próprio schema para garantir independência.

## Comunicação
- **Síncrona:** REST com autenticação e versionamento.
- **Assíncrona:** Eventos publicados e consumidos via Kafka.

## Segurança
- Autenticação e autorização via OAuth2/OpenID Connect.
- Proteção de endpoints sensíveis com roles e escopos.

## Benefícios
- Escalabilidade horizontal.
- Baixo acoplamento entre módulos.
- Maior resiliência e facilidade de manutenção.
