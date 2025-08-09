# Guia de Contribuição - Petshop

Bem-vindo ao repositório **Petshop**! Este documento descreve como você pode contribuir para o projeto, mantendo um fluxo de trabalho organizado e seguindo boas práticas de desenvolvimento.

---

## 📋 Sumário
1. [Sobre o Projeto](#sobre-o-projeto)
2. [Pré-requisitos](#pré-requisitos)
3. [Clonando o Repositório](#clonando-o-repositório)
4. [Fluxo de Trabalho](#fluxo-de-trabalho)
5. [Padrões de Código e Commits](#padrões-de-código-e-commits)
6. [Execução Local](#execução-local)
7. [Boas Práticas](#boas-práticas)
8. [Suporte](#suporte)

---

## Sobre o Projeto

O **Petshop** é o repositório pai de um ecossistema de serviços e aplicações que compõem um sistema distribuído, utilizado como **case de portfólio para um desenvolvedor sênior**.  
Este repositório concentra **issues, milestones e gestão Kanban**, além de documentar os fluxos de contribuição.

---

## Pré-requisitos

Antes de contribuir, você deve ter instalado:

- **Java 21+**
- **Spring Boot 3.4.0**
- **Gradle com Kotlin DSL**
- **Docker** e **Docker Compose**
- **Git**
- IDE recomendada: [IntelliJ IDEA Ultimate](https://www.jetbrains.com/idea/)

Além disso, configure o Git com seu nome e e-mail:
```bash
git config --global user.name "Seu Nome"
git config --global user.email "seu-email@dominio.com"
```

---

## Clonando o Repositório

```bash
git clone git@github.com:SEU-USUARIO/petshop.git
cd petshop
```

> ℹ️ Caso o projeto use **submódulos** ou outros repositórios vinculados, siga as instruções do README principal para configurá-los.

---

## Fluxo de Trabalho

O fluxo de trabalho segue a seguinte estrutura:

1. **Criação da Issue**
   - Toda alteração começa com uma *issue* no repositório `petshop`.
   - As issues são categorizadas por *labels* (`bug`, `feature`, `enhancement`, etc.).

2. **Criação da Branch**
   - Nome da branch deve seguir o padrão:
     - `feature/nome-da-feature`
     - `bugfix/descricao-bug`
     - `hotfix/ajuste-critico`
   ```bash
   git checkout -b feature/nome-da-feature
   ```

3. **Desenvolvimento**
   - Mantenha commits pequenos e descritivos.
   - Teste localmente antes de enviar.

4. **Pull Request (PR)**
   - Abra o PR no repositório correto.
   - Relacione a PR com a issue usando `Closes #numero-da-issue`.

5. **Revisão e Aprovação**
   - PRs passam por revisão de código antes do *merge*.
   - Ajustes solicitados devem ser aplicados antes da aprovação.

6. **Kanban Automático**
   - Issues e PRs abertas no `petshop` são automaticamente adicionadas ao GitHub Project Kanban.

---

## Padrões de Código e Commits

**Commits:**
- `feat:` nova funcionalidade
- `fix:` correção de bug
- `docs:` alteração de documentação
- `style:` alterações de formatação
- `refactor:` refatoração de código
- `test:` adição ou modificação de testes
- `chore:` mudanças de build ou ferramentas

Exemplo:
```bash
git commit -m "feat: adicionar endpoint de cadastro de pets"
```

**Código:**
- Seguir padrões de formatação da IDE configurada.
- Respeitar a estrutura de pacotes definida.

---

## Execução Local

1. **Subir ambiente com Docker Compose**
   ```bash
   docker compose up
   ```
2. **Serviços disponíveis:**
   - API: `http://localhost:8080`
   - Grafana: `http://localhost:3000`
   - Prometheus: `http://localhost:9090`
   - Loki: `http://localhost:3100`

3. **Rodar testes localmente**
   ```bash
   ./gradlew test
   ```

---

## Boas Práticas

- Sempre crie branchs a partir da `main` atualizada.
- Adicione testes unitários para novas funcionalidades.
- Mantenha o histórico de commits limpo e organizado.
- Documente endpoints novos na OpenAPI.

---

## Suporte

Se tiver dúvidas:
1. Consulte a documentação no README.
2. Verifique issues abertas no GitHub.
3. Abra uma nova issue com a tag `question`.

---

✍️ **Obrigado por contribuir!**
