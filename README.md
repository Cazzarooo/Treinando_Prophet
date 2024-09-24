# Previsão da Variação do IPCA com Prophet

Este projeto utiliza a biblioteca Prophet para prever a variação do IPCA (Índice de Preços ao Consumidor Amplo) nos próximos 10 anos, com base em dados históricos.

## Pré-requisitos

Antes de executar o código, você precisa ter o Python instalado em sua máquina, além das seguintes bibliotecas:

- `pandas`
- `prophet`
- `matplotlib`

Você pode instalar essas bibliotecas usando pip:

```bash
pip install pandas prophet matplotlib
```

## Dataset

O código utiliza um arquivo CSV chamado `inflacao.csv` que deve estar no mesmo diretório que o script. O arquivo deve conter pelo menos duas colunas:

- `referencia`: A data em formato 'YYYY-MM'.
- `ipca_variacao`: A variação percentual do IPCA.

Este código pode ser adaptado para funcionar com outros arquivos CSV, desde que as colunas relevantes sejam renomeadas de acordo e o formato da data seja compatível.

## Como usar

1. **Carregar o Dataset**: O código começa carregando os dados do arquivo CSV.
2. **Preparar os Dados**: Os dados são preparados para o modelo Prophet. As colunas são renomeadas e a coluna de data é convertida para o formato datetime.
3. **Ajustar o Modelo**: O modelo Prophet é criado e ajustado aos dados.
4. **Fazer Previsões**: Um dataframe futuro é gerado para os próximos 120 meses, e as previsões são realizadas.
5. **Plotar Resultados**: As previsões são plotadas em um gráfico, mostrando a tendência da variação do IPCA.
6. **Exibir Resultados**: O código imprime as previsões para os últimos 10 anos.

## Exemplo de Uso

Para executar o código, basta rodar o script Python. Certifique-se de que o arquivo `inflacao.csv` está corretamente configurado.

```bash
python seu_script.py
```

## Resultados

O script gera um gráfico mostrando a previsão da variação do IPCA e também imprime as previsões em formato tabular para os últimos 10 anos.

## Contribuições

Contribuições são bem-vindas! Sinta-se à vontade para fazer um fork do repositório e enviar pull requests.

Sinta-se à vontade para fazer mais ajustes se necessário!
