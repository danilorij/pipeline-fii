# pipeline-fii
Projeto desenvolvido em Python para execução no Google Colab. Realiza a extração de dados de fundos imobiliários (FIIs) a partir de uma fonte online, aplica tratamento, filtros e classificação com base em critérios definidos, e exporta os resultados automaticamente para uma planilha no Google Sheets.


## Critérios de filtragem aplicados
Após a coleta e o tratamento dos dados, os fundos imobiliários são filtrados com base nos seguintes critérios:

P/VP ≥ 0,80

Número de cotistas ≥ 15.000

Patrimônio líquido > R$ 200 milhões

Liquidez diária > R$ 400 mil

Dividend Yield > 0,65% (relativo ao pagamento do ultimo mês)


## Contribuições e melhorias
Este projeto foi desenvolvido com critérios básicos que considero relevantes para análise de FIIs, mas você pode (e deve) ajustar os filtros e parâmetros conforme seus próprios critérios de investimento. Sinta-se à vontade para adaptar o código às suas necessidades.

Pretendo continuar trabalhando no código, realizando melhorias e ajustes futuros, como novas fontes de dados, inclusão de métricas adicionais e uma interface mais interativa. Contribuições são bem-vindas!
