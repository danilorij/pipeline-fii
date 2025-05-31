# pipeline-fii

Projeto desenvolvido em **Python** para execução no **Google Colab**.  
Realiza a extração de dados de Fundos Imobiliários (FIIs) a partir de uma fonte online, aplica tratamento, filtros e classificação com base em critérios definidos, e exporta os resultados automaticamente para uma planilha no Google Sheets.

---

## Critérios de Filtragem Aplicados

Após a coleta e o tratamento dos dados, os FIIs são filtrados com base nos seguintes critérios:

- **P/VP ≥ 0,80**
- **Número de cotistas ≥ 15.000**
- **Patrimônio líquido > R$ 200 milhões**
- **Liquidez diária > R$ 400 mil**
- **Dividend Yield > 0,65%** (relativo ao pagamento do último mês)

---

## Saída de Dados

O programa possui duas versões com diferentes formas de exportação dos resultados finais:

### Versão Python (.py)

- Gera um arquivo Excel chamado:  
  `fiis_filtrados.xlsx`
- Caminho de salvamento automático:  
  `~/Documents/Dados_FII/fiis_filtrados.xlsx`

### Versão Jupyter Notebook (Google Colab)

- Cria uma planilha online chamada `pipeline-fii` diretamente no seu Google Sheets
- É necessário estar autenticado com uma conta Google para permitir o acesso e escrita no seu Drive

---

## Contribuições e Melhorias

Este projeto foi desenvolvido com critérios básicos que considero relevantes para análise de FIIs, mas você pode (e deve) ajustar os filtros e parâmetros conforme seus próprios critérios de investimento.  
Sinta-se à vontade para adaptar o código às suas necessidades.

Pretendo continuar trabalhando no código, realizando melhorias e ajustes futuros, como:

- Novas fontes de dados
- Inclusão de métricas adicionais
- Interface mais interativa

**Contribuições são bem-vindas.**

---

## Requisitos

Este projeto requer as seguintes bibliotecas Python:

- `selenium >= 4.0.0`
- `beautifulsoup4 >= 4.11.1`
- `pandas >= 1.5.0`
- `numpy >= 1.23.0`
- `webdriver-manager >= 3.8.0`
- `openpyxl >= 3.0.0`
