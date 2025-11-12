# Projeto: Monitor Financeiro Acessível

## (a) Descrição Sucinta da Ideia do Projeto

**Ideia do Projeto:**
O projeto consiste no desenvolvimento de um aplicativo mobile de monitoramento de custos e investimentos focado em **simplicidade e acessibilidade**. O objetivo é criar uma ferramenta financeira que possa ser utilizada por qualquer pessoa, independentemente de sua afinidade com tecnologia ou limitações.

**Como será usado e Contexto:**
Esperamos que o sistema seja usado para o controle financeiro diário ou semanal. O usuário poderá registrar gastos de forma rápida (com o mínimo de campos possível) e consultar visualizações claras de onde seu dinheiro está sendo gasto. O contexto de uso principal é em dispositivos móveis (celulares), permitindo o registro de um gasto no momento em que ele ocorre, ou uma consulta rápida em casa para planejar o mês.

**Por quem será usado (Público-alvo):**
O design será focado em usuários frequentemente negligenciados por aplicativos financeiros tradicionais:
1.  **Idosos:** Que podem ter dificuldades com interfaces complexas, fontes pequenas ou excesso de informações.
2.  **Pessoas com Deficiências (PCDs):** Especificamente usuários com baixa visão (que necessitam de fontes ajustáveis, alto contraste) ou dificuldades motoras (que se beneficiam de botões grandes e navegação simples).
3.  **Usuários Iniciantes:** Pessoas com baixa literacia financeira que se sentem intimidadas por ferramentas complexas.

---

## (b) Lista de Stakeholders e Descrição

### 1. Usuários Principais (Primários)

* **Idosos (Ex: Aposentados):**
    * **Descrição:** Podem ter experiência limitada com aplicativos modernos. A confiança é um fator chave; eles precisam sentir que o app é seguro e que não vão "quebrar" nada.
    * **Necessidades:** Fontes grandes (que respeitem a configuração do celular), navegação linear (poucas telas), ícones claros e mínimo de campos para preenchimento.

* **PCDs (Ex: Usuários com Baixa Visão):**
    * **Descrição:** Experiência variável com tecnologia, mas dependem de recursos de acessibilidade (como leitores de tela ou ajuste de fonte/contraste).
    * **Necessidades:** Conformidade total com as diretrizes de acessibilidade da plataforma (iOS/Android), feedback tátil/sonoro e visualizações de dados que não dependam apenas de cores (ex: gráficos com texturas ou rótulos claros).

* **Pessoas com Dificuldades Cognitivas ou Baixa Literacia Financeira:**
    * **Descrição:** Podem se sentir sobrecarregados ("confusa, muitas opções de análise", como visto na entrevista).
    * **Necessidades:** Linguagem simples (evitar jargão financeiro), foco em uma ou duas tarefas principais (Registrar Gasto, Ver Saldo) e talvez um assistente (IA) para tirar dúvidas simples.

### 2. Stakeholders Secundários

* **Familiares e Cuidadores:**
    * **Descrição:** Podem ser responsáveis por configurar o aplicativo para o usuário principal ou por revisar os gastos periodicamente com eles. São "usuários-assistentes".

* **Equipe de Desenvolvimento:**
    * **Descrição:** Responsáveis por implementar e manter os requisitos de acessibilidade e a simplicidade do design.

* **Instituições Financeiras (Bancos):**
    * **Descrição:** (Se o app evoluir) Podem ser parceiros para integração de contas, mas sua complexidade (visto na entrevista: "conectado direto com o banco mas não categorizava direito") é um risco para a simplicidade.

---

## (c) Métodos de Pesquisa, Justificativa e Descobertas

Para entender os problemas e o contexto dos usuários, selecionamos dois métodos complementares do IDEO: **Entrevistas (Interviews)** e **Pesquisas (Surveys)**.

### Método 1: Entrevistas (Interviews)

* **Justificativa:** Escolhemos entrevistas para obter dados qualitativos profundos. Elas nos permitem entender o *porquê* por trás das frustrações dos usuários, capturando emoções e contextos específicos (como a confusão com "muitas opções") que um formulário quantitativo não conseguiria.
* **Resumo das Descobertas (Baseado na Entrevista n1):**
    * A usuária atual já tenta se organizar (usa app "Minhas Economias" e planilhas), mas ainda sente "falta de clareza".
    * **Problema Principal:** Os apps atuais são confusos, têm "muitas opções de funcionalidade" e exigem muito esforço para registrar um simples gasto ("preencher muita coisa").
    * **Problema de Visualização:** Dificuldade em entender *onde* está gastando (ex: "qual banco"), sugerindo que os gráficos atuais são ineficazes.
    * **Problema de Automação:** A conexão bancária (Open Finance) falha na categorização, o que gera retrabalho e desconfiança.
    * **Desejo (Oportunidade):** A usuária busca simplicidade ("fácil navegação, menos botões"), quer saber "o quanto ainda pode gastar" (foco no futuro, não só no passado) e valoriza acessibilidade (letra personalizada).

### Método 2: Pesquisas (Surveys via Forms)

* **Justificativa:** Enquanto a entrevista nos deu profundidade (o "porquê"), a pesquisa (Survey) foi usada para obter amplitude (o "quantos"). O objetivo foi validar se as frustrações encontradas na Entrevista n1 (complexidade, visualização ruim) eram comuns a um grupo maior de pessoas e coletar dados demográficos sobre nosso público.
* **Resumo das Descobertas (Baseado no Forms):
*    Ferramentas Atuais: Os usuários gerenciam finanças majoritariamente via Aplicativos de Banco e Planilhas.

*    Prioridades de Usabilidade e comunicação, o feedback indica uma alta demanda por interfaces simples, claras e diretas:
   *    Evitar jargões financeiros complexos. Usar linguagem natural e direta.
   *    Investir em uma arquitetura de informação e navegação excepcionalmente clara.
   *    Telas de confirmação de ações (transações, cadastros) são essenciais.
   *    Usar ícones com rótulos de texto claros para garantir a compreensão da função dos botões.

*    Acessibilidade e Design Visual (UX/UI)
As preferências dos usuários destacam a importância de opções de personalização visual e legibilidade:

*   Design Visual:

   Modo Escuro (Dark Mode): Forte preferência.
   Densidade de Informação: Evitar telas com "muita coisa junta". Priorizar layouts limpos e com bom espaçamento.

*   Acessibilidade:

   Escalabilidade: Implementar a opção de aumentar o tamanho da fonte.
   Contraste: Garantir altas taxas de contraste em todo o design.

---

## (d) Reflexão sobre o Uso dos Métodos

* **O que deu certo:** A combinação dos métodos foi eficaz. A **Entrevista** forneceu "insights de ouro" muito específicos, como a frustração com o excesso de campos e a má categorização do banco, além da excelente ideia sobre a "letra personalizada". O **Formulário** *(aguardando dados)* nos ajudou a... *(ex: confirmar que isso não era um problema de uma pessoa só)*.

* **O que deu errado (ou foi um desafio):**
    * *Na Entrevista:* Alguns dos entrevistados já eram usuários de apps financeiros. Embora ótimo para entender as *falhas* dos concorrentes, pode ter um viés.
    * *No Formulário:* * Tivemos dificuldade em conseguir respondentes da faixa etária mais alta (idosos), pois a distribuição de formulários online tende a atingir um público mais jovem e tecnológico.*
    
* **O que faríamos diferente:** Complementaríamos com um terceiro método IDEO: **Observação (Observation)** ou **Shadowing**. Teria sido muito valioso *assistir* algum entrevistado tentando usar o app "Minhas Economias" ou suas planilhas. Ver onde eles pausam, onde eles "travam" ou suspiram de frustração, revelaria problemas de usabilidade que eles talvez nem saibam articular em uma entrevista.

---

## (e) Lista de 6-8 Descrições de Tarefas

Baseado nas descobertas (especialmente na Entrevista n1), estas são as tarefas centrais que os usuários precisam realizar:

1.  **Registrar um gasto rapidamente** (com o mínimo de campos: Valor, Categoria simples).
2.  **Verificar "quanto ainda posso gastar"** (um indicador visual claro do orçamento restante).
3.  **Entender onde meu dinheiro foi gasto este mês** (visualização simples por categoria).
4.  **Diferenciar gastos por banco/cartão** (resolvendo a dor da "falta de clareza" por banco).
5.  **Ajustar o tamanho do texto do aplicativo** (para corresponder às configurações de acessibilidade do celular).
6.  **Corrigir a categoria de um gasto** (seja ele manual ou vindo do banco).
7.  **Visualizar o crescimento de um investimento** (um gráfico de linhas simples).
8.  **Pedir ajuda ou uma explicação** (interagindo com a "IA" sugerida para entender um gasto).

---
## Provas da Pesquisa (Links)
