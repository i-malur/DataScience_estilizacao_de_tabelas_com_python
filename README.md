# 📊 Estilização de Tabelas com Python

## 📚 Sobre

Este repositório contém o projeto para o curso Alura "Data Visualization: estilização de tabelas com Python".

Este projeto teve como objetivo analisar e visualizar dados de vendas para auxiliar diferentes times de uma empresa.

Inicialmente, foi realizada a coleta e preparação dos dados, carregando o arquivo CSV relatorio_vendas.csv em um DataFrame pandas. Foi feita uma inspeção inicial dos dados com dados.info() para verificar os tipos de dados e a presença de valores nulos. A coluna data_pedido foi convertida para o tipo datetime para permitir análises temporais.

Em seguida, foram abordadas as seguintes missões:

Missão 1: Time de vendas Foi criada uma visualização para identificar os 10 maiores clientes por total de venda. Para isso, os dados foram agrupados por nome_cliente e a soma das vendas foi calculada, utilizando groupby() e sum(). Os 10 maiores clientes foram selecionados com nlargest(10), o DataFrame resultante foi resetado e renomeado para melhor clareza. A tabela foi estilizada com Styler para formatar os valores de vendas.

Missão 2: Time comercial O objetivo foi associar o total ganho em vendas e o total lucrado por tipo de produto. Os dados foram agrupados por tipo_produto, calculando a soma das colunas vendas e lucro com groupby() e sum(). A tabela resultante foi estilizada usando Styler com formatação de moeda, destaque para valores máximos e mínimos, e gradiente de cores para facilitar a visualização.

Missão 3: Time de logística (Distribuição de pedidos por região) Para entender a distribuição de pedidos por região do Brasil, foi calculada a contagem de pedidos por regiao usando value_counts(). Em seguida, foi calculada a porcentagem de pedidos por região. A tabela foi estilizada com Styler, formatando a porcentagem e adicionando barras de dados para uma representação visual da distribuição.

Missão 4: Time de logística (Quantidade de produtos solicitados por mês por departamento) Esta missão visou identificar o padrão de quantidade de produtos solicitados por mês por departamento. A coluna data_pedido foi utilizada para extrair o mês e ano (%Y - %b) em uma nova coluna meses. Foi utilizada a função pivot_table para criar uma tabela dinâmica com os departamentos como índice, os meses como colunas e a soma da quantidade como valores. A tabela foi estilizada com Styler para melhor apresentação.

Missão 5: Relatório de performance Para o relatório de performance, foi criada uma visualização da relação entre tipos de clientes e modo de envio de produtos de acordo com as vendas. Foi utilizada a função pivot_table para agregar as vendas pela segmento_cliente e modo_envio. Totais por linha e coluna foram adicionados ao DataFrame. A tabela foi estilizada com Styler, formatando os valores e aplicando estilos condicionais para destacar linhas e colunas de total.

Ao longo do projeto, diversas técnicas de manipulação e visualização de dados com pandas foram utilizadas, incluindo:

* Carregamento e inspeção de dados (read_csv, info())
* Conversão de tipos de dados (pd.to_datetime)
* Agrupamento e agregação de dados (groupby(), sum(), value_counts())
* Seleção e manipulação de dados (nlargest(), reset_index(), set_index(), sort_values())
* Criação de colunas derivadas (dt.strftime)
* Remodelação de dados (pivot_table)
* Estilização de tabelas com Styler (format(), highlight_max(), highlight_min(), background_gradient(), bar(), set_table_styles(), set_sticky(), set_td_classes())
* Este projeto demonstra a aplicação de técnicas essenciais de análise e visualização de dados para gerar insights acionáveis para diferentes áreas de negócio.


## 🔍 Sobre este projeto

Neste projeto, explorei técnicas de **estilização de tabelas** usando Python (usando bibliotecas como `pandas`, `Styler`, etc.). O objetivo foi tornar as tabelas mais visuais e informativas, aplicando cores, formatações condicionais, estilos customizados e melhorias de layout para facilitar a leitura e interpretação dos dados.

Este repositório serve como uma demonstração prática de como tabelas bem estilizadas podem contribuir com a apresentação de resultados em relatórios e dashboards.

---

## 🗂️ Estrutura do repositório

- `Estilizacao_de_tabelas.ipynb` — notebook principal com demonstrações e exemplos de estilização.  
- `README.md` — este arquivo, com explicações sobre o projeto.  

---

## Tecnologias usadas
[![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)](https://jupyter.org/)
[![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![Data Visualization](https://img.shields.io/badge/Data%20Visualization-0A66C2?style=for-the-badge&logo=tableau&logoColor=white)](https://en.wikipedia.org/wiki/Data_visualization)
[![Google Colab](https://img.shields.io/badge/Google%20Colab-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=white)](https://colab.research.google.com/)

## ⚙️ Como executar

1. Clone este repositório:

   ```bash
   git clone https://github.com/i-malur/DataScience_estilizacao_de_tabelas_com_python.git
   cd DataScience_estilizacao_de_tabelas_com_python
   ````


2. Certifique-se de ter Python instalado.

3. Instale dependências básicas (caso use `requirements.txt`, ou instale manualmente):

   ```bash
   pip install pandas jupyterlab
   ```

4. Abra o notebook:

   ```bash
   jupyter lab
   # ou
   jupyter notebook
   ```

5. Execute as células e explore os estilos aplicados nas tabelas.

## 🏅 Certificado
[📄 Visualizar](https://drive.google.com/file/d/1wdhxNURfQjRd3TR-PDNMKQgbBpaQo04E/view?usp=drive_link)

## 👩‍💻 Autora

**Maria Luiza Fernandes**
🌐 [GitHub - i-malur](https://github.com/i-malur)




