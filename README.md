# ETL para identificação dos melhores preços de vendas de calça jeans - Star Jeans
Projeto de ETL de dados de um e-commerce de roupas

<div align="center">
 <img height="400em" src="https://github.com/laaisfmaia/webscraping_HM_Star_Jeans/blob/main/modulos/Fabricas-de-jeans-em-Rio-do-Sul.jpg">
</div>

## 1. Objetivo do Projeto
Esse projeto tem como objetivo principal fazer o ETL (extração, transformação, carregamento) e posterior análise de dados referentes a informações sobre o preço, tipo e material para a fabricação de calças jeans. 

A motivação para o projeto é a demanda por informações pelo e-commerce fictício chamado Star Jeans que está entrando no mercado de varejo de moda dos USA e não tem expertise para precificar e identificar os materiais para a fabricação dos produtos.

## 2. Questão de negócio

As principais perguntas de negócio são:

- Qual o melhor preço de venda para as calças?
- Quantos tipos de calças e suas cores para o produto inicial?
- Quais as matérias-primas necessárias para confeccionar as calças?

## 3. Etapas do projeto

Esse projeto baseia-se na metodologia CRISP (Cross Industry Standard Process for Data Mining) que é um método cíclico de desenvolvimento em que se passa várias vezes pela mesma etapa do projeto para que em cada passo você avance um pouco mais.

<div align="center">
 <img height="350em" src="https://github.com/laaisfmaia/webscraping_HM_Star_Jeans/blob/main/modulos/crisp.png">
</div>

- **Entendimento do negócio:** pesquisar quais empresas são grandes concorrentes e possuem as informações necessárias de preço e material. 
- **Coleta de dados:** A coleta de dados vai ser feita através de Webscraping com Python usando a biblioteca BeautifulSoup no site da H&M (uma grande varejista do USA).
- **Limpeza dos dados**
- **Exploração dos dados:** Análise dos dados para poder gerar insights e também para perceber quais são as variáveis mais relevantes e que podem impactar uma possível modelagem de Machine Learning.

## 4. Premissas do negócio
- Os dados foram coletados em dois dias em horários diferentes
- As informações sobre os materiais usados na fabricação do bolso das calças foram descartados.
- As variáveis coletadas no site da H&M são:

<table border="1">
    <thead>
    <tr>
        <th>Variável</th>
        <th>Definição</th>
    </tr>
    </thead>
    <tr>
        <td>product_id</td>
        <td>Número de identificação de cada produto</td>
    </tr>
    <tr>
        <td>style_id</td>
        <td>Código do estilo do produto baseado no SKU (Stock Keeping Unit)</td>
    </tr>
    <tr>
        <td>color_id</td>
        <td>Código da cor do produto baseado no SKU (Stock Keeping Unit)</td>
    </tr>
    <tr>
        <td>product_name</td>
        <td>O tipo da calça jeans</td>
    </tr>
    <tr>
        <td>color_name</td>
        <td>A cor do produto</td>
    </tr>
    <tr>
        <td>fit</td>
        <td>A modelagem do produto</td>
    </tr>
    <tr>
        <td>color_name</td>
        <td>A cor do produto</td>
    </tr>
    <tr>
        <td>product_price</td>
        <td>Preço do produto</td>
    </tr>
    <tr>
        <td>cotton</td>
        <td>Percentual de cotton no produto</td>
    </tr>
    <tr>
        <td>polyester</td>
        <td>Percentual de polyester no produto</td>
    </tr>
    <tr>
        <td>spandex</td>
        <td>Percentual de spandex no produto</td>
    </tr>
    <tr>
        <td>scrapy_datetime</td>
        <td>	Data e hora de coleta dos dados</td>
    </tr>
</table>
	
## 5. Ferramentas utilizadas
 
Python, Pandas, Numpy, BeautifulSoup e sqlalchemy

## 6. Conclusão

Esse projeto ainda está em desenvolvimento
- Para acessar o código completo [clique aqui](https://github.com/laaisfmaia/webscraping_HM_Star_Jeans/blob/main/webscraping_hm.ipynb)



	

