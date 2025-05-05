# Versionamento Semântico: Um Tutorial

O **versionamento semântico** é uma abordagem para controlar versões de software, seguindo o formato `MAJOR.MINOR.PATCH-EXTRA+META`. Cada parte do número de versão tem um significado específico:

- **MAJOR**: Alterações que quebram a compatibilidade.
- **MINOR**: Novos recursos mantendo a compatibilidade.
- **PATCH**: Correções de bugs sem alterar a funcionalidade.
- **EXTRA**: Versão extra quando você faz um novo pré-lançamento ou outros parâmetros de versionamento extra.
- **META**: Metadados sobre a versão, como informações de build ou commit.

## Como Utilizar Versionamento Semântico

1. **Defina a Versão Inicial**: Comece com uma versão como `1.0.0`. Ou `0.0.0` se quiser considerar versões temporárias, do tipo _pre-release_
2. **Atualize a Versão**:
    - **MAJOR**: Quando há quebras de compatibilidade.
    - **MINOR**: Ao adicionar novos recursos (_feat_, _fix_).
    - **PATCH**: Para correções de bugs.
    - **EXTRA**: Para versões pré-lançamento ou outros parâmetros de versionamento extra.

Exemplo de atualização de versão:

```bash
# Versão inicial
1.0.0

# Adiciona novo recurso
1.1.0

# Corrige bug
1.1.1

# Quebra compatibilidade
2.0.0
```

## Versões Extras (EXTRA)

As versões extras são usadas para indicar estágios específicos do desenvolvimento antes do lançamento oficial:

- **alpha**: Versões iniciais, geralmente com funcionalidades incompletas (exemplo: `1.0.0-alpha.1`)
- **beta**: Versões mais estáveis que alpha, mas ainda em teste (exemplo: `1.0.0-beta.2`)
- **rc** (_Release Candidate_): Versões candidatas ao lançamento final (exemplo: `1.0.0-rc.1`)
- **snapshot**: Captura do código em um momento específico (exemplo: `1.0.0-snapshot.20230301`)
- **dev**: Versões em desenvolvimento (exemplo: `1.0.0-dev.4`)

Exemplo de fluxo de versões extras:

```bash
# Versão alpha inicial
1.0.0-alpha.1

# Segunda versão alpha com melhorias
1.0.0-alpha.2

# Primeira versão beta
1.0.0-beta.1

# Release candidate
1.0.0-rc.1

# Versão final
1.0.0
```

---

[Saiba mais sobre versionamento semântico no site oficial](https://semantic-versioning.org/)
