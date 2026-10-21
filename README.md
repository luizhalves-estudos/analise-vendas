
<p align="center">
  <img src="assets/animacao_analise_vendas.gif" alt="Animação de análise de dados com gráficos e programação" width="850">
</p>

## Sobre o projeto

Este projeto analisa dados de vendas de uma empresa de varejo utilizando Python, com foco em exploração de dados, qualidade das informações e identificação de padrões comerciais que possam apoiar a tomada de decisão.

Desenvolvido como projeto de portfólio acadêmico, reúne análises de faturamento por mês, produtos e países, além da investigação de registros atípicos e cancelamentos.

## Objetivos

- Explorar e compreender a estrutura dos dados de vendas.
- Identificar valores ausentes e possíveis inconsistências.
- Analisar o faturamento ao longo do tempo.
- Identificar produtos com maior faturamento.
- Comparar o desempenho comercial entre países.
- Investigar registros atípicos e cancelamentos.
- Comunicar os resultados por meio de tabelas e gráficos.

## Tecnologias utilizadas

- **Python** — linguagem de programação.
- **Pandas** — manipulação e análise de dados.
- **NumPy** — operações numéricas.
- **Matplotlib** — criação de visualizações.
- **Jupyter Notebook** — desenvolvimento e documentação da análise.
- **Visual Studio Code** — ambiente de desenvolvimento.

## Dados utilizados

O projeto utiliza o conjunto de dados **Online Retail**, armazenado localmente em `data/raw/Online Retail.xlsx`.

A base original contém 541.909 registros, abrangendo o período de 1º de dezembro de 2010 a 9 de dezembro de 2011.

## Principais resultados

- **530.104 registros** mantidos na base filtrada de vendas positivas.
- **£ 10.666.684,54** em valor bruto de vendas positivas incluídas na análise.
- **3.922 códigos de produtos** e **38 países** presentes na base filtrada.
- O **Reino Unido** apresentou o maior faturamento entre os países analisados.
- **Novembro de 2011** apresentou o maior total mensal na análise, com aproximadamente £ 1,51 milhão.
- A análise dos produtos permitiu comparar faturamento e volume de unidades vendidas.

## Qualidade dos dados e limitações

Para uma visão inicial das vendas positivas, foi criada uma base de análise com registros que apresentam quantidade e preço unitário maiores que zero.

Essa abordagem resultou em 530.104 registros e £ 10.666.684,54 em vendas positivas. Esse valor representa o total bruto das vendas incluídas na análise, não necessariamente o faturamento líquido definitivo, pois os cancelamentos não estão incluídos nessa visão.

A exploração também identificou valores ausentes, quantidades negativas, preços inválidos e uma venda excepcional de 80.995 unidades, seguida de um cancelamento correspondente 12 minutos depois. Os dois registros apresentam valores iguais e sinais opostos, anulando-se financeiramente. Esse caso reforça a importância de investigar registros atípicos antes de tirar conclusões comerciais.

Dezembro de 2011 está incompleto, com registros somente até o dia 9. Por isso, comparações desse mês com meses completos devem considerar essa limitação.

Valores atípicos não devem ser excluídos automaticamente: é necessário investigar seu contexto e documentar os critérios adotados.

## Como executar o projeto

1. Instale Python e Visual Studio Code.
2. Instale as bibliotecas necessárias:

   ```bash
   py -m pip install pandas numpy matplotlib openpyxl ipykernel
   ```

3. Abra a pasta do projeto no Visual Studio Code.
4. Abra o notebook `analise_vendas.ipynb`.
5. Selecione um kernel Python com as dependências instaladas.
6. Execute as células na ordem apresentada.

O arquivo Excel deve estar disponível no caminho `data/raw/Online Retail.xlsx`.

> **Observação sobre os dados:** antes de publicar o arquivo Excel no GitHub, verifique a licença e as condições de distribuição do conjunto. Se não puder redistribuí-lo, mantenha-o fora do repositório e explique no README como obtê-lo.

## Aprendizados

Este projeto permitiu praticar a importação e exploração de dados, a identificação de problemas de qualidade, a criação de indicadores, a construção de gráficos e a investigação de registros atípicos.

Também reforçou a importância de documentar os critérios de análise e considerar as limitações dos dados antes de transformar resultados em conclusões de negócio.

## Próximos passos

- Aprofundar a análise de cancelamentos e faturamento líquido.
- Melhorar a apresentação visual dos indicadores.
- Desenvolver um dashboard para complementar a análise exploratória.

## Estrutura do projeto

```text
Projeto analise venda/
├── assets/
│   └── animacao_analise_vendas.gif
├── data/
│   └── raw/
│       └── Online Retail.xlsx
├── analise_vendas.ipynb
└── README.md
```

## Autor

**Luiz Alves** · Projeto de portfólio em Ciência de Dados e Análise de Dados.
