
# Previsão de Séries Temporais: Análise dos Preços de Ações da Petrobras (PETR4)

Este projeto utiliza um modelo de regressão linear para realizar a previsão do preço de fechamento ajustado das ações da Petrobras (PETR4). O objetivo é analisar a viabilidade da predição linear para dados financeiros, avaliando o desempenho do modelo em diferentes escalas temporais (diária, semanal e mensal).

## Objetivo do Projeto

Prever o preço das ações da Petrobras utilizando um modelo de predição linear. A previsão desse tipo de dado pode auxiliar em estratégias financeiras e operações de trade, uma vez que permite antecipar tendências de mercado.

## Estrutura do Projeto

O projeto segue as seguintes etapas:
1. **Coleta de Dados**: Dados históricos do preço das ações PETR4 são coletados usando o pacote `yfinance`.
2. **Divisão dos Dados**: Os dados são divididos em conjuntos de treino e teste, com 70% para treino e 30% para teste.
3. **Implementação do Modelo Linear**: Um modelo de regressão linear é treinado usando a descida de gradiente, com implementação manual e cálculo do gradiente via `autograd`.
4. **Avaliação do Modelo**: O modelo é avaliado no conjunto de teste, gerando métricas de erro e gráficos comparativos.
5. **Análise em Diferentes Escalas**: O modelo é reavaliado em escalas semanais e mensais, para observar sua performance em horizontes temporais mais amplos.

## Resultados

As métricas de erro no conjunto de teste foram:
- **Erro Médio Absoluto (MAE)**: 4,43
- **Erro Quadrático Médio (MSE)**: 31,61

Ao realizar a análise em escalas semanais e mensais, notou-se uma leve melhora nas métricas de erro, indicando que o modelo linear captura melhor tendências em períodos mais amplos.

## Requisitos

As bibliotecas necessárias para a execução do projeto estão listadas no arquivo `requirements.txt`. Para instalar todas as dependências, use:

```bash
pip install -r requirements.txt
```

### Bibliotecas Principais

- `numpy`: Manipulação de arrays e operações matemáticas.
- `autograd`: Cálculo automático do gradiente para a implementação da descida de gradiente.
- `yfinance`: Coleta de dados financeiros diretamente do Yahoo Finance.
- `matplotlib`: Geração de gráficos para visualização dos resultados.

## Como Executar

1. **Clone o Repositório**:
   ```bash
   git clone https://github.com/joaowcitino/regresao-linear.git
   cd regresao-linear
   ```

2. **Instale as Dependências**:
   ```bash
   pip install -r requirements.txt
   ```

3. **Execute o Notebook**:
   Abra e execute o arquivo `app.ipynb` para reproduzir todas as etapas do projeto. 

## Estrutura de Arquivos

- `regresao-linear.ipynb`: Notebook com o código completo do projeto.
- `requirements.txt`: Lista de bibliotecas necessárias.
- `README.md`: Documentação do projeto.

## Observações

Este projeto é uma abordagem inicial para prever séries temporais financeiras com modelos lineares. Por ser um modelo simples, ele apresenta limitações para capturar a alta variabilidade dos dados diários de mercado. Em análises futuras, o uso de modelos mais complexos poderia fornecer predições mais precisas.

## Autor

Desenvolvido por [João Whitaker Citino](https://github.com/joaowcitino).
