
---

# Padrões de Commits: Convenção e Especificação

## Visão Geral

A especificação **Conventional Commits** define uma convenção clara para mensagens de commit, que proporciona uma forma legível tanto para desenvolvedores humanos quanto para ferramentas automatizadas. Ela permite a organização do histórico de código de maneira que facilite a geração de logs de mudanças (CHANGELOGs), determine de forma automática o versionamento semântico (SemVer) e comunique de maneira eficiente a natureza das modificações entre os membros da equipe e usuários.

### Estrutura da Mensagem de Commit

A convenção define que as mensagens de commit devem ser estruturadas da seguinte forma:

```
<tipo>[escopo opcional]: <descrição>

[corpo opcional]

[rodapé(s) opcional(is)]
```

## Tipos de Commit

A especificação define os seguintes tipos para as mensagens de commit:

- **`feat`**: Implementação de novo recurso ou funcionalidade. Relacionado a mudanças **MINOR** no versionamento semântico.
  
- **`fix`**: Correção de um erro no código. Relacionado a mudanças **PATCH** no versionamento semântico.
  
- **`docs`**: Alterações relacionadas à documentação do projeto.
  
- **`test`**: Modificações nos testes, como adição ou atualização.
  
- **`build`**: Mudanças em dependências, builds ou configurações relacionadas.
  
- **`perf`**: Melhorias de desempenho no código.
  
- **`style`**: Mudanças que afetam a formatação do código (sem alterar o comportamento do código).
  
- **`refactor`**: Alterações no código que não afetam funcionalidades, mas melhoram a estrutura.
  
- **`chore`**: Tarefas auxiliares, como modificações em ferramentas de desenvolvimento ou configurações gerais.
  
- **`ci`**: Mudanças em configurações de integração contínua.
  
- **`raw`**: Alterações relacionadas à estrutura de arquivos e dados.
  
- **`cleanup`**: Remoção de código não utilizado ou obsoleto.
  
- **`remove`**: Exclusão de arquivos ou funcionalidades.
  
- **`BREAKING CHANGE`**: Alterações que quebram a compatibilidade da API. Pode ser adicionado como rodapé ou com o símbolo **`!`** no tipo de commit.

## Exemplo de Mensagens de Commit

- **Commit com tipo e descrição simples**  
  `feat: adicionar suporte a idiomas adicionais`

- **Commit com tipo, escopo e BREAKING CHANGE**  
  `feat(api)!: introduzir nova estrutura para a API de usuários`  
  `BREAKING CHANGE: a estrutura de dados foi alterada de JSON para XML.`

- **Commit com corpo explicativo**  
  `fix: corrigir erro de cálculo em função de desconto`  
  `A correção resolve um erro que ocorria quando o desconto era maior que o preço original.`

- **Commit com rodapé, incluindo referência a um ticket**  
  `fix: corrigir erro de digitação no código`  
  `veja o ticket para detalhes sobre os erros corrigidos`  
  `Refs #123`

## Rodapés Opcionais

Além da descrição e do corpo do commit, você pode incluir rodapés que fornecem mais contexto. Alguns exemplos:

- **`BREAKING CHANGE`**: Usado para indicar mudanças que quebram a compatibilidade.  
- **`Closes`**: Usado para fechar um ticket ou issue, ex: `Closes #123`.  
- **`Reviewed-by`**: Indica quem revisou o commit, ex: `Reviewed-by: João Silva`.

## Regras e Especificações

A mensagem de commit **deve** seguir a estrutura definida, com tipo seguido de uma descrição clara. O uso de escopo é opcional, mas recomendado para fornecer mais contexto. Além disso, é importante que o tipo de commit seja escolhido com precisão, para garantir que o histórico de versões seja bem organizado.

### Requisitos do Commit:

1. **Tipo de Commit**: Deve ser um substantivo claro, como `feat`, `fix`, `docs`, etc.
2. **Escopo (opcional)**: Fornece contexto adicional sobre a parte do código afetada, como `feat(auth)` ou `fix(parser)`.
3. **Descrição**: Um resumo claro e conciso da mudança realizada.
4. **Corpo (opcional)**: Explicações detalhadas ou razões para a alteração.
5. **Rodapé (opcional)**: Para contextualizar mais informações, como referências a tickets ou menções a breaking changes.

## Por que Usar o Conventional Commits?

- **Automatização**: Facilita a criação de CHANGELOGs automatizados.
- **Versionamento Semântico**: Permite determinar automaticamente o tipo de versão a ser incrementada (MAJOR, MINOR, PATCH).
- **Facilidade de Colaboração**: Facilita a comunicação sobre as mudanças no projeto e contribuições de outros desenvolvedores.
- **Processos Automatizados**: Pode ser integrado a ferramentas de CI/CD para disparar processos de build, testes e deploy.

## Perguntas Frequentes (FAQ)

1. **Como devo lidar com commits durante o desenvolvimento inicial?**  
   Mesmo nas fases iniciais de desenvolvimento, é recomendável seguir a convenção, pois isso ajuda a documentar o progresso e mantém o histórico organizado.

2. **Devo sempre usar letras maiúsculas ou minúsculas para os tipos de commit?**  
   A escolha entre maiúsculas ou minúsculas é flexível, mas deve-se manter consistência em todo o projeto.

3. **Como lidar com commits de múltiplos tipos?**  
   Sempre que possível, quebre os commits em unidades mais específicas. Caso contrário, o uso de múltiplos tipos em um único commit deve ser documentado claramente no corpo.

4. **Isso não limita o desenvolvimento rápido?**  
   A ideia do Conventional Commits não é desencorajar a agilidade, mas sim garantir que o desenvolvimento seja organizado e bem documentado, mesmo em iterações rápidas.

5. **Como o Conventional Commits se relaciona com o SemVer?**  
   - `feat` → MINOR (novos recursos)
   - `fix` → PATCH (correções)
   - `BREAKING CHANGE` → MAJOR (alterações incompatíveis)

## Considerações Finais

A adoção da especificação **Conventional Commits** é altamente recomendada para equipes que desejam manter um histórico de código organizado, facilitar o versionamento semântico e automatizar processos como a geração de CHANGELOGs. Além disso, a convenção ajuda a comunicar as intenções dos desenvolvedores de forma mais clara, beneficiando todos os envolvidos no ciclo de vida do software.

--- 
Se você quer voltar, clique em [Retornar ⏎](../README.md)