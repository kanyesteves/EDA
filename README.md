# Documentação para análises de dados

Nesse repositório vou colocar todos os arquivo do curso `Análise exploratória de dados`.

### O que vai ser aprendido nesse curso

- O que é análise exploratória de dados.
- Entender um dataset e explorando seus valores.
- Gráficos: Boxplot, Histograma e Violino.
- Normalidade e outras métricas de dispersão.
- Correlação e gráficos de espalhamento.
- Cálculo de coeficientes de correlação.
- Modelos de regressão linear.

#### Bibliotecas que serão usadas:

- Pandas.
- Seaburn.
- Plotly
- Matplotlib.
- Re - Expressões Regulares

## O que é EDA?
`Exploratory Data Analysis` ou `Análise Explotatória de dados`. É uma abordagem inicial e crucial para entender a natureza e as características dos dados antes de aplicar métodos mais avançados de análises. 

#### Indicadores do EDA:
Explorar e visualizar os dados para identificar padrões, tendências, anomalias e insights preliminares.

#### Objetivo do EDA:
Ganhar uma compreensão intuitiva dos dados, identificar possíveis problemas, e formular hipóteses que possam ser testadas em estágios subsequentes da análise.

## Funções criadas

- Remover html: 

```
def remove_html(html):
    pattern = re.compile('<.*?>')
    cleantext = re.sub(pattern, '', html)
    return cleantext.replace('*', '').strip()
```

- Formatar valores nulos:

```
def format_percent(value):
    return f'{100 * value:.2f}%'
```

