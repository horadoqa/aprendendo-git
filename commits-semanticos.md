# Commits semânticos

Commits semânticos, ou convenções de commits semânticos, referem-se a um padrão de nomenclatura para mensagens de commit que visa facilitar a compreensão do histórico de um projeto e melhorar a comunicação entre desenvolvedores. Esse padrão, conhecido como Conventional Commits, utiliza uma estrutura específica que ajuda a descrever claramente as mudanças realizadas no código.

## Estrutura dos Commits Semânticos

A estrutura básica de uma mensagem de commit semântica é a seguinte:

    <tipo>(<escopo>): <descrição>

    [opcional: corpo]

    [opcional: rodapé]

## Componentes

1. Tipo: Define a natureza da alteração. Exemplos comuns incluem:

    - feat: Uma nova funcionalidade.
    - fix: Correção de um bug.
    - docs: Mudanças na documentação.
    - style: Alterações que não afetam a lógica do código (espaçamento, formatação).
    - refactor: Alterações no código que não adicionam funcionalidades nem corrigem bugs.
    - test: Adição ou modificação de testes.
    - chore: Mudanças em tarefas de manutenção (ex.: configurações, ferramentas).

2. Escopo: Opcional, mas pode ser usado para indicar a parte do código afetada pela mudança (ex.: api, ui, etc.).

3. Descrição: Um resumo conciso da alteração, geralmente no imperativo (ex.: "adiciona novo botão").

4. Corpo: Explicações adicionais sobre a mudança, se necessário. Este componente é opcional.

5. Rodapé: Usado para referências a issues (ex.: "Fixes #123") ou para mencionar que uma alteração é quebradora (ex.: "BREAKING CHANGE: descrição").

## Exemplos de Mensagens de Commit Semânticas

**feat**    
    
    feat(api): adiciona suporte à autenticação JWT

    Implementa autenticação via JWT para melhorar a segurança da API.

    Fixes #45

**fix** 
    
    fix(ui): corrige erro de layout no menu de navegação

**docs** 
    
    docs(README): atualiza instruções de instalação

## Vantagens do Uso de Commits Semânticos

- Histórico Claro: Facilita a leitura do histórico do repositório, permitindo que outros desenvolvedores entendam rapidamente o que foi alterado.

- Automação: Ferramentas podem ser configuradas para gerar automaticamente notas de versão ou changelogs com base nas mensagens de commit, simplificando o processo de documentação.

- Identificação de Mudanças: Permite uma fácil identificação de mudanças que introduzem novas funcionalidades, correções de bugs e alterações na documentação.

- Consistência: Estabelece um padrão que todos os membros da equipe podem seguir, melhorando a comunicação e a colaboração.

## Como Usar

Estabeleça um Padrão: Defina o uso de commits semânticos na sua equipe ou projeto. É útil criar um guia de estilo.

- Use Ferramentas: Existem ferramentas que podem ajudar a enforce (forçar) convenções de commits semânticos, como o commitlint para validar mensagens de commit e semantic-release para automatizar o versionamento e publicação.

- Pratique: Incentive os desenvolvedores a escreverem commits semânticos. Isso se tornará um hábito com o tempo.

## Conclusão
Os commits semânticos são uma prática eficaz para melhorar a comunicação e a organização em projetos de software. Ao seguir um padrão consistente, equipes podem aumentar a clareza do histórico de versões e facilitar a colaboração. Se você tiver mais perguntas ou precisar de mais detalhes, sinta-se à vontade para perguntar!