# Violência Doméstica

![Página 1]()

***

## 1. Dashboard de Violência Doméstica

### Contexto de Negócio
Este dashboard é uma ferramenta estratégica desenvolvida para o acompanhamento e análise dos registros de Violência Doméstica e Familiar contra a Mulher no estado de Minas Gerais. A iniciativa visa transformar dados brutos, provenientes do Sistema Integrado de Defesa Social (SIDS/REDS) da Polícia Civil de Minas Gerais, em insights acionáveis para a gestão de segurança pública e a formulação de políticas preventivas.

### Visão Geral do Dashboard
Este dashboard foi desenvolvido para oferecer um controle integrado sobre violência doméstica. Estruturado para análises temporal e geográfica, a ferramenta proporciona visibilidade completa sobre os totais de ocorrências e vítimas, a média mensal de registros, e a distribuição dos delitos. O dashboard permite filtros dinâmicos, sendo crucial para a tomada de decisão focada e baseada em dados.

### Perguntas Respondidas
- Como se comportou a evolução mensal dos registros de violência? 
- Quais as principais naturezas de delito? 
- Quais categorias de despesas precisam de atenção? 
- Qual a Distribuição de Violências?

### **Principais Indicadores:**
- Total de Violências
- Média de Violências por Mês
- Município com Mais Casos
- Concentração Regional (MG)
- Quantidade de Municípios
- Média de Casos por Município

### Medidas utilizadas
- `Média de Casos por Município = DIVIDE([Total de Violências], DISTINCTCOUNT(violencia_domestica_2023[municipio]))`
- `Media Vitimas por Violência = DIVIDE([Total Vitimas], [Total de Violências], 0)`
- `Quantidade de Municípios = DISTINCTCOUNT(violencia_domestica_2023[Municipio])`
- `Total Consumados = CALCULATE(COUNTROWS(violencia_domestica_2023), violencia_domestica_2023[tentado_consumado] = "Consumado")`
- `Total de Violências = COUNTROWS('violencia_domestica_2023')`
- `Total Vitimas = SUM(violencia_domestica_2023[qtde_vitimas])`

***

### Dados utilizados

Utilizei os dados estatísticos sobre Violência Doméstica e Familiar contra a Mulher no estado de Minas Gerais. A base de dados utilizada tem como fonte primária a Polícia Civil de Minas Gerais, e os dados foram extraídos do Armazém de Dados do Sistema Integrado de Defesa Social (SIDS/REDS), que compila notificações de diversas forças de segurança (PM, PC, CBM, etc.).

- [Link da base de dados utilizada](https://dados.mg.gov.br/dataset/violencia-contra-mulher)

***  

## Contribuições

Contribuições são **muito bem-vindas**. Se você tem sugestões ou melhorias, fique à vontade para abrir uma **issue** ou enviar um **pull request**.

## Sobre mim

[![Avatar GitHub](https://avatars.githubusercontent.com/u/102989796?v=4&s=150)](https://github.com/asergioscosta)

