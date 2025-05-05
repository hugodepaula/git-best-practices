# Guia Rápido de Padrões de Commits Convencionais

[![Conventional Commits](https://img.shields.io/badge/Conventional%20Commits-1.0.0-%23FE5196?logo=conventionalcommits&logoColor=white)](https://conventionalcommits.org)
[![Gitmoji](https://img.shields.io/badge/gitmoji-%20😜%20😍-FFDD67.svg?style=flat-square)](https://gitmoji.dev)

## Tipos de Commits Convencionais

| Tipo de Commit | Exemplo de Uso          |
| :------------- | :---------------------- |
| **feat**       | `feat: adiciona funcionalidade de busca` |
| **fix**        | `fix: corrige erro de conexão` |
| **docs**       | `docs: atualiza documentação da API` |
| **refactor**   | `refactor: reestrutura código sem alterar comportamento` |
| **perf**       | `perf: melhora performance do código` |
| **style**      | `style: ajusta formatação do código` |
| **test**       | `test: adiciona testes para nova funcionalidade` |
| **build**      | `build: atualiza dependências do projeto` |
| **ops**        | `ops: modifica infraestrutura de deployment` |
| **chore**      | `chore: atualiza .gitignore` |
| **BREAKING CHANGE** | `feat! altera formato de dados` ou `BREAKING CHANGE: descrição da quebra` |

### Escopos

O `escopo` fornece informações contextuais adicionais.

* É uma parte **opcional** do formato
* Os Escopos permitidos dependem do projeto específico
* Não use identificadores de issue como escopos

**Exemplos de escopos**:

* `api`
* `triangulation`
* `auth`
* `web`
* `mobile`

### Indicador de Mudanças Quebradas (**BREAKING CHANGE**)

**BREAKING CHANGE** devem ser indicadas por um `!` antes do `:` na linha de assunto e.g. `feat(api)!: remove status endpoint`

* É uma parte **opcional** do formato
* Mudanças quebradas **devem** ser descritas na de rodapé

## Commits com Emojis

São opcionais, mas ajudam a identificar rapidamente o tipo de mudança. Não existe um padrão oficial, mas o [gitmoji.dev](https://gitmoji.dev) é uma boa referência.

Abaixo estão alguns exemplos de emojis e seus significados:

| Emoji | Tag                    | Descrição                                           |
|-------|------------------------|-----------------------------------------------------|
| 🎉   | :tada:                 | Cria um novo projeto ou repositório                 |
| ✨   | :sparkles:             | Adiciona uma nova funcionalidade                    |
| 🐛   | :bug:                  | Corrige um bug                                      |
| ⚡️   | :zap:                  | Melhora a performance do código                     |
| ♻️   | :recycle:              | Refatoração de código                               |
| 📝   | :memo:                 | Adiciona ou atualiza documentação                   |
| 💥   | :boom:                 | Introduz mudanças que quebram compatibilidade       |
| 🔥   | :fire:                 | Remove código ou arquivos não utilizados            |
| 🚑️   | :ambulance:            | Corrige um erro crítico                             |
| ✅   | :white_check_mark:     | Adiciona ou corrige testes existentes               |
| 💡   | :bulb:                 | Adiciona comentários                                |
| 🎨   | :art:                  | Melhora a estrutura ou formata o código             |
| 💄   | :lipstick:             | Melhora a aparência ou estilo do código             |
| 🚀   | :rocket:               | Realiza o deploy ou publicação de release           |
| 🔒   | :lock:                 | Corrige um problema de segurança                    |
| 🚧   | :construction:         | Trabalho em andamento                               |
| 🔧   | :wrench:               | Altera arquivos de configuração                     |
| 🛠️   | :hammer_and_wrench:    | Mudanças relacionadas a processos de build          |
| 👷   | :construction_worker:  | Atualizações no sistema de integração contínua      |
| 🌐   | :globe_with_meridians: | Internacionalização e localização                   |

## Exemplos de Commits Convencionais

```markdown
  feat: add notification service
```

 ```markdown
  feat(triangulation): add algorithm for triangulation
 ```

 ```markdown
  feat!: remove ticket list endpoint

  refers to #1337

  BREAKING CHANGE: ticket endpoints no longer supports list all entities.
```

```markdown
  fix(triangulation): improve triangulation algorithm performance
```

 ```markdown
  fix(api): fix expired token error
```

 ```markdown
  fix: add missing parameter to user api call

  The error occurred due to <reasons>.
```

 ```markdown
  perf: decrease storage footprint for tracking logs
```

```markdown
  build: update dependencies
```

```markdown
  build(release): up version to 1.0.0
```

```markdown
  refactor: implement fibonacci number calculation as recursion
```

```markdown
  style: remove empty line
```
