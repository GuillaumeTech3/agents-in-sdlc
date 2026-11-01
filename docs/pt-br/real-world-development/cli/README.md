---
slug: pt-br/real-world-development/cli
title: "CLI do GitHub Copilot"
authors:
  - geektrainer
lastUpdated: 2026-09-18
---

O **[GitHub Copilot CLI](https://docs.github.com/copilot/concepts/agents/about-copilot-cli)** coloca o GitHub Copilot no seu terminal como um assistente de programação baseado em agentes. Ele explora bases de código, gera código, executa comandos e se conecta a ferramentas externas — tudo pela linha de comando, para que você mantenha o foco sem trocar para um editor gráfico.

O workshop acompanha um fluxo contínuo de trabalho na Tailspin Toys: prepare o projeto no GitHub Codespaces, instale o Copilot CLI e faça uma pequena alteração para exibir avaliações com estrelas antes de criar seu primeiro pull request. Em seguida, comece pela issue de filtros, planeje a abordagem, implemente o recurso e revise o resultado. Atualize as instruções do repositório, personalize uma skill de verificações de qualidade, teste o comportamento com o Playwright MCP e crie um agente de QA. Por fim, revise a mudança completa, use o Agent Merge no pull request de filtros e explore comandos de barra úteis. Você também pode seguir uma [série opcional de três módulos com GitHub Copilot CLI e Foundry][foundry].

Para manter o foco do workshop, você criará dois pull requests: um para as avaliações com estrelas e outro para os filtros, incluindo as atualizações de instruções, skill, perfil de QA e testes. O fluxo de filtros e qualidade compartilha uma conversa e uma branch para que você aproveite o trabalho anterior enquanto explora cada ferramenta.

## Lições

| Lição | Tópico | Descrição |
|----------|-------|-------------|
| [0. Pré-requisitos][ex0] | Configuração | Prepare seu repositório e o Codespace |
| [1. Instalar o Copilot CLI][ex1] | Instalação | Instale e autentique o Copilot CLI e conheça os recursos básicos |
| [2. Adicionar avaliações com estrelas: uma vitória rápida][ex2] | Primeira mudança | Exiba as avaliações existentes e a alternativa para valores nulos; depois, mescle seu primeiro PR |
| [3. Modos do agente: Plan e Autopilot][ex3] | Modos do agente | Planeje o recurso a partir da issue, implemente com Autopilot e revise no modo Interactive |
| [4. Orientar o Copilot com instruções personalizadas][ex4] | Contexto | Explore e atualize as instruções e aplique-as ao trabalho de filtros |
| [5. Personalizar e usar uma skill de verificações de qualidade][ex5] | Verificações repetíveis | Explore a skill existente, altere o formato do relatório e execute-a |
| [6. Validar a funcionalidade com o Playwright MCP][ex6] | Observação no navegador | Configure o MCP na CLI e inspecione o comportamento dos filtros |
| [7. Criar e usar um agente de QA][ex7] | Requisitos e cobertura | Crie e selecione um perfil especialista e reúna evidências da verificação final |
| [8. Criar e mesclar o pull request do recurso][ex8] | Revisão e merge | Revise a mudança completa, crie o PR e use o Agent Merge |
| [9. Comandos de barra no GitHub Copilot CLI][ex9] | Recursos da CLI | Explore contexto, modelos, compartilhamento e delegação opcional para o agente de nuvem |
| [10. Resumo e próximos passos][ex10] | Resumo | Revise o fluxo, as personalizações reutilizáveis e outros recursos |
| [Opcional: Incorporar o Foundry][foundry] | Agentes hospedados | Prepare um modelo, implante um agente baseado em catálogo e conecte-o ao site |

## Pré-requisitos

Antes de participar deste workshop, verifique se você tem:

- [ ] Uma conta do GitHub com um plano ativo **Copilot Student, Pro, Pro+, Business ou Enterprise**
- [ ] Permissão para criar um repositório e um Codespace
- [ ] Familiaridade básica com o terminal ou a linha de comando

> [!TIP]
> Não tem um plano pago? Estudantes verificados podem obter o GitHub Copilot gratuitamente por meio do [GitHub Education][callout-student-plan-education]. O plano **Copilot Student** inclui os recursos de agente, MCP, revisão de código e Copilot CLI usados neste workshop.

> [!NOTE]
> Se você usa o Copilot Business ou o Copilot Enterprise, verifique se o administrador habilitou o Copilot CLI para uso.

## Começar

[**Comece pela Lição 0: Pré-requisitos →**][ex0]

[ex0]: 0-prerequisites/
[ex1]: 1-install-copilot-cli/
[ex2]: 2-add-star-rating/
[ex3]: 3-agent-modes/
[ex4]: 4-custom-instructions/
[ex5]: 5-agent-skills/
[ex6]: 6-mcp-playwright/
[ex7]: 7-qa-agent/
[ex8]: 8-create-pull-request/
[ex9]: 9-cli-power-tools/
[ex10]: 10-review/
[foundry]: 8-foundry-agent/
[callout-student-plan-education]: https://github.com/education/students
