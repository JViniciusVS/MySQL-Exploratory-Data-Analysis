# Data Cleaning and Exploratory Data Analysis (EDA) Project

## Projeto: Limpeza de Dados e Análise Exploratória de Dados (EDA)

### Descrição

Este projeto envolve a limpeza de dados e análise exploratória de dados utilizando uma planilha Excel bruta e MySQL Workbench. O objetivo é transformar dados não tratados em um formato padronizado e limpo, seguido de análises que fornecem insights sobre os dados.

### Estrutura do Projeto

O projeto é dividido em duas partes principais:

1. **Limpeza de Dados (Data Cleaning)**
   - Remoção de duplicatas.
   - Padronização dos dados.
   - Tratamento de valores nulos ou em branco.
   - Remoção de colunas desnecessárias.
   - Criação de uma tabela staging para preservar os dados originais.

2. **Análise Exploratória de Dados (EDA)**
   - Análise das demissões por empresa, indústria e país.
   - Análise temporal das demissões.
   - Cálculo de totais acumulados e rankings anuais.

### Tecnologia Utilizada

- **MySQL Workbench**: Para manipulação e análise dos dados.
- **Excel**: Como fonte de dados bruta.

### Instruções de Uso

1. **Data Cleaning**

   O processo de limpeza dos dados é realizado através das seguintes etapas:

   - **Remoção de Duplicatas**: O código cria uma tabela staging e utiliza a função `ROW_NUMBER()` para identificar e remover registros duplicados.
   - **Padronização dos Dados**: Realiza ajustes nos valores de colunas como `company`, `industry`, e `country`, removendo espaços em branco e padronizando nomes.
   - **Tratamento de Valores Nulos ou em Branco**: Identifica e corrige registros com valores nulos ou em branco, incluindo uma tentativa de preencher valores faltantes com base em outras informações na tabela.
   - **Remoção de Colunas Desnecessárias**: Exclui colunas ou registros irrelevantes para a análise.

2. **Exploratory Data Analysis (EDA)**

   Após a limpeza dos dados, são realizadas várias consultas para explorar e obter insights dos dados:

   - **Análise por Percentual de Demissões**: Filtra empresas que demitiram 100% dos seus funcionários e ordena por fundos arrecadados.
   - **Soma das Demissões por Empresa, Indústria e País**: Agrupa e ordena os dados para mostrar o total de demissões.
   - **Análise Temporal das Demissões**: Agrupa as demissões por ano e mês, criando também um total acumulado ao longo do tempo.
   - **Ranking Anual das Empresas com Mais Demissões**: Utiliza a função `DENSE_RANK()` para gerar um ranking das empresas com mais demissões por ano.

### Execução

- **Passo 1**: Execute os scripts de limpeza de dados na sequência apresentada para preparar os dados.
- **Passo 2**: Execute as consultas de EDA para gerar os insights desejados.

### Contribuições

Sinta-se à vontade para abrir issues ou enviar pull requests para melhorias ou correções.

### Licença

Este projeto é de código aberto sob a licença [MIT](LICENSE).
