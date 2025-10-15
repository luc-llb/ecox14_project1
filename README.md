# Projeto de Análise de Dados de Anime - ETL com Pandas e Matplotlib

## 📊 Descrição do Projeto

Este projeto realiza análises exploratórias e visualizações de dados sobre animes utilizando datasets de animes e ratings. O projeto é composto por 5 notebooks Jupyter que implementam processos de ETL (Extração, Transformação e Carga) com visualizações usando Matplotlib.

## 📁 Estrutura do Projeto

```
project/
│
├── datas/                          # Datasets de entrada
│   └── dataset.txt                 # Link com os datasets
│
├── outputs/                        # Gráficos gerados
│
├── nb1.ipynb                       # Notebook 1: Animes por Tipo (Gráfico de Barras)
├── nb2.ipynb                       # Notebook 2: Ratings por Ano (Gráfico de Linha)
├── nb3.ipynb                       # Notebook 3: Distribuição de Gêneros (Gráfico de Pizza)
├── nb4.ipynb                       # Notebook 4: Score e Quantidade (2 Séries em Y)
├── nb5.ipynb                       # Notebook 5: Distribuição de Scores (Histograma)
│
├── requirements.txt                # Dependências do projeto
└── README.md                       # Este arquivo
```

## 📚 Notebooks e Análises

### Resumo das Análises

| Notebook | Análise | Group By | Tipo de Gráfico | Séries em Y | Observações |
|----------|---------|----------|-----------------|-------------|-------------|
| **nb1.ipynb** | Animes por Tipo | ✅ | 📊 Barras | 1 | ETL inicial + tratamento dos dados |
| **nb2.ipynb** | Ratings + Avaliações por Ano | ✅ | 📈 Linha | **2** | Merge + Eixos Y duplos |
| **nb3.ipynb** | Distribuição de Gêneros | ✅ | 🍕 Pizza | 1 | Expansão de múltiplos gêneros |
| **nb4_.ipynb** | Score vs Quantidade por ano | ✅ | 📊 Linha | **2** | Eixos Y duplos |
| **nb5.ipynb** | Distribuição de Scores | ❌ | 📊 Histograma | 1 | Análise estatística |

### 🚀 Ordem de Execução Recomendada

1. **nb1.ipynb** - **Comece aqui** para entender os dados e tratar os dados do dataset animes.csv (sem esse tratamento outras analises não ocorrerão da forma correta) 
2. **nb2.ipynb** - Análise temporal
3. **nb3.ipynb** - Análise categórica
4. **nb4.ipynb** - Análise multivariada
5. **nb5.ipynb** - Análise estatística

## 🔧 Instalação e Execução

### 1. Instalar Dependências

```bash
pip install -r requirements.txt
```

### 2. Executar os Notebooks

Abra cada notebook no Jupyter ou VS Code e execute as células sequencialmente:

```bash
# Para Jupyter Notebook
jupyter notebook

# Para VS Code
# Abra os arquivos .ipynb diretamente
```

### 3. Verificar Outputs

Os gráficos serão salvos automaticamente na pasta `outputs/`

## 📦 Dependências

- **pandas**: Manipulação e análise de dados
- **matplotlib**: Visualização de dados
- **os**: Acesso a diretórios

## 📊 Datasets
<table style="border-collapse: collapse; text-align: left;">
    <tr>
        <th style="text-align: center;">
            <h4>animes.csv</h4>
        </th>
        <th style="text-align: center;">
            <h4>ratings.csv</h4>
        </th>
    </tr>
    <tr>
        <td>
            <li>
                <strong>animeID</strong>: ID único do anime
            </li>
            <li>
                <strong>type</strong>: Título do anime
            </li>
            <li>
                <strong>title</strong>: Tipo (TV, Movie, OVA, Special, ONA)
            </li>
            <li>
                <strong>year</strong>: Ano de lançamento
            </li>
            <li>
                <strong>score</strong>: Score médio (1-10)
            </li>
            <li>
                <strong>episodes</strong>: Número de episódios
            </li>
            <li>
                <strong>genres</strong>: Gêneros do anime
            </li>
        </td>
        <td>
            <li>
                <strong>userID</strong>: ID do usuário
            </li>
            <li>
                <strong>animeID</strong>: ID do anime
            </li>
            <li>
                <strong>rating</strong>: Avaliação (1-10)
            </li>
        </td>
    </tr>
</table>


## 👨‍💻 Autor

Projeto desenvolvido por [Lucas Luan B. Barbosa](https://github.com/luc-llb), para a disciplina **ECOX14 - Tópicos Especiais em Programação I**, ministrada pelo professor [Dr. Enzo Seraphim](https://sigaa.unifei.edu.br/sigaa/public/docente/portal.jsf?siape=1543328) pelo curso de **Engenharia da Computação** na _Universidade Federal de Itajubá_.

## 📝 Licença

Este projeto é para fins educacionais.