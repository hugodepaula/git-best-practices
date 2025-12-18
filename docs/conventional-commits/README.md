# Conventional Commits: Um Tutorial

[![Conventional Commits](https://img.shields.io/badge/Conventional%20Commits-1.0.0-%23FE5196?logo=conventionalcommits&logoColor=white)](https://conventionalcommits.org)

Os **Conventional Commits** são uma convenção para estruturar mensagens de commit de forma padronizada. Eles seguem um formato específico que ajuda a identificar o tipo de alteração realizada.

## Como Utilizar Padrões de Commits Convencionais

1. **Escolha o Tipo**: Use palavras-chave como `feat`, `fix`, `docs`, etc., para indicar o tipo de alteração.
2. **Adicione Escopo (Opcional)**: Inclua um escopo entre parênteses para fornecer contexto adicional.
3. **Descreva a Alteração**: Forneça uma breve descrição da mudança.
4. **Inclua Corpo e Rodapés (Opcional)**: Adicione detalhes adicionais ou informações como `BREAKING CHANGE`.

Para Detalhes sobre formatos de mensagens de comits e listas de exemplos, veja [Guia Rápido de Padrões de Commits Convencionais](quick-guide.md).

> [!TIP]
> **[git-conventional-commits](https://github.com/qoomon/git-conventional-commits)** é uma ferramenta útil para validar mensagens de commit e garantir que estejam em conformidade com os padrões convencionais, determinar versões e gerar Changelogs.

## Formatos de Mensagens de Commit

### Mensagem padrão

```bash
<tipo>(<escopo opcional>): <descrição> \
# linha em branco 
<corpo opcional> \
# linha em branco
<rodapé opcional>
```

### Commit de Mesclagem (Merge)

```bash
Merge branch "<nome da branch>"
```

Segue a mensagem padrão de mesclagem do git

### Commit de Reversão (Revert)

```bash
Revert "<linha de assunto do commit revertido>"
```

Segue a mensagem padrão de reversão do git

### Commit Inicial

```bash
chore: init
```

Exemplo de mensagem de commit convencional:

```bash
git commit -m "feat: adiciona suporte a múltiplos idiomas \
 \ 
 \ 
 Refs. #1234"
```

---

[Saiba mais sobre Conventional Commits](https://www.conventionalcommits.org/pt-br/v1.0.0/)
