### Versionamento Semântico: Um Tutorial

O **versionamento semântico** é uma abordagem para controlar versões de software, seguindo o formato `MAJOR.MINOR.PATCH`. Cada parte do número de versão tem um significado específico:

- **MAJOR**: Alterações que quebram a compatibilidade.
- **MINOR**: Novos recursos mantendo a compatibilidade.
- **PATCH**: Correções de bugs sem alterar a funcionalidade.


#### Como Utilizar Versionamento Semântico

1. **Defina a Versão Inicial**: Comece com uma versão como `1.0.0`. Ou `0.0.0` se quiser considerar versões temporárias, do tipo _pre-release_
2. **Atualize a Versão**:
    - **MAJOR**: Quando há quebras de compatibilidade.
    - **MINOR**: Ao adicionar novos recursos.
    - **PATCH**: Para correções de bugs.

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

---

[Saiba mais sobre versionamento semântico no site oficial](https://semver.org/lang/pt-BR/)