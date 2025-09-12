# Atomic Commits

Os **commits atômicos** são uma prática recomendada no desenvolvimento de software que envolve realizar alterações pequenas e focadas no código-fonte.

- Cada commit deve representar uma mudança única e coerente, facilitando a revisão, teste e manutenção do código.
- Cada commit deve ser capaz de ser revertido sem causar efeitos colaterais indesejados além do que está descrito na própria mensagem do commit

## Como Utilizar Commits Atômicos

1. **Identifique a Mudança**: Antes de começar a codificar, defina claramente o que você deseja alterar ou adicionar. Cada commit deve tratar de apenas uma alteração lógica: uma feature, um bugfix, uma refatoração, etc. Não misture correções de bugs com novas funcionalidades no mesmo commit.
2. **Faça a Alteração**: Realize a mudança necessária, mantendo-a o mais simples possível. Se uma alteração lógica exige modificações em vários arquivos, agrupe-as em um único commit, desde que todas estejam relacionadas ao mesmo objetivo.
3. **Verifique o Código**: Execute testes locais para garantir que a alteração não introduz erros.
4. **Commit Atômico**: Use `git add` para adicionar os arquivos alterados e, em seguida, faça o commit com uma mensagem clara e concisa. Utilize o padrão de [Conventional Commits](../conventional-commits/README.md) para garantir que a mensagem siga um formato consistente.

Exemplos de mensagens de commit atômico:

```bash
git commit -m "feat(auth): adiciona autenticação OAuth2 no backend"
git commit -m "feat(mobile): implementa trilateração para cálculo de posição"
git commit -m "fix(api): corrige endpoint de histórico de localização"
git commit -m "docs(requirements): adiciona requisitos não-funcionais de segurança"
git commit -m "refactor(backend): separa lógica de logs estruturados em módulo próprio"
git commit -m "test(web): adiciona testes automatizados para RBAC"
git commit -m "chore(ci): adiciona pipeline de build para aplicação mobile"
git commit -m "feat(web): exibe mapa interativo com localização em tempo real"
git commit -m "feat(backend): registra logs de operações dos dispositivos"
git commit -m "feat(mobile): integra notificações push via Firebase"
```

## Mensagens de commit

- Use o imperativo presente (“Adiciona validação de email”).
- Limite a linha de resumo a 50 caracteres.
- Use o corpo da mensagem para detalhes adicionais, se necessário (até 75 caracteres por linha).
- Referencie issues ou tickets relevantes (ex: “Closes #123”).
- Não use mensagens vagas como “update”, “fix” ou “wip”. Seja específico sobre o que foi alterado e por quê.

**Exemplos de mensagens de commit atômico (sem resumo):**

```bash
git commit -m "feat(auth): adiciona autenticação OAuth2 no backend"
git commit -m "feat(mobile): implementa trilateração para cálculo de posição"
git commit -m "fix(api): corrige endpoint de histórico de localização"
git commit -m "docs(requirements): adiciona requisitos não-funcionais de segurança"
git commit -m "refactor(backend): separa lógica de logs estruturados em módulo próprio"
git commit -m "test(web): adiciona testes automatizados para RBAC"
git commit -m "chore(ci): adiciona pipeline de build para aplicação mobile"
git commit -m "feat(web): exibe mapa interativo com localização em tempo real"
git commit -m "feat(backend): registra logs de operações dos dispositivos"
git commit -m "feat(mobile): integra notificações push via Firebase"
```

**Exemplos de mensagens de commit atômico (com resumo):**

```markdown
fix(web): Corrige cálculo de desconto na tela de checkout

Ajusta a função applyDiscount para considerar cupons expirados.
Relacionado a issue #456.
```

```markdown
fix(auth): adiciona validação de senha forte no cadastro de usuários

Implementa regras de senha mínima e caracteres especiais.
Relacionado a issue #789.
```

## **Dicas Finais**

- Não tenha medo de muitos commits; commits pequenos facilitam a manutenção.
- Utilize branches para cada tarefa ou feature.
- Se necessário, utilize squash apenas para limpar commits intermediários sem sentido, mas evite perder granularidade importante.
- Prefira qualidade e clareza no histórico ao invés de quantidade de commits.

---
