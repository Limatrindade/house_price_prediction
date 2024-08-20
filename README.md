# house_price_prediction

![Status do Projeto](https://img.shields.io/badge/status-concluído-brightgreen)
![Version](https://img.shields.io/badge/version-1.0.0-blue)

## Descrição

Este projeto tem como objetivo principal estabelecer o preço de venda de uma casa através de uma análise detalhada das variáveis que mais influenciam essa precificação. Em um mercado imobiliário dinâmico e competitivo, a determinação precisa do valor de uma propriedade é essencial para vendedores, compradores e investidores. Em vez de depender de uma única variável, o preço de venda de uma casa é afetado por uma combinação de diversos fatores que podem impactar significativamente o valor final.

A primeira etapa deste projeto é identificar e entender as variáveis explicativas que afetam o preço de venda de uma casa. Essas variáveis podem incluir, mas não se limitam a:

- Localização: A região em que a casa está situada, que pode influenciar o valor devido à demanda local e à qualidade do bairro.
-  Número de Quartos: A quantidade de quartos pode afetar o valor da propriedade, refletindo seu tamanho e adequação para famílias.
-  Tamanho do Lote: A área total do terreno pode impactar o valor, especialmente em áreas urbanas e suburbanas.
-  Idade do Imóvel: A idade da casa pode influenciar o preço, com imóveis mais novos geralmente valendo mais devido a menos necessidade de reparos.
-  Proximidade de Serviços: A proximidade de escolas, centros comerciais, transporte público e outras comodidades pode afetar o valor da propriedade.

A análise dessas variáveis tem um duplo propósito:

1. Precificação de Imóveis: Fornecer uma estimativa precisa do valor de uma casa específica com base em suas características. Isso ajuda vendedores a definir preços competitivos e compradores a avaliar ofertas.

2. Insights sobre o Mercado Imobiliário: Proporcionar uma compreensão mais profunda do comportamento do mercado imobiliário, identificando quais fatores têm maior impacto no preço de venda e como eles interagem.

Mas qual foi a Metodologia aplicada?

- Coleta de Dados: Reunir dados sobre diversas propriedades, incluindo suas características e preços de venda históricos.
- Pré-processamento: Limpar e preparar os dados para análise, lidando com dados ausentes e variáveis categóricas.
- Análise Exploratória: Realizar uma análise descritiva e visualização dos dados para entender as distribuições e correlações entre variáveis.
- Construção do Modelo: Desenvolver e treinar modelos preditivos usando técnicas de machine learning para prever o preço de venda com base nas variáveis identificadas.
- Avaliação do Modelo: Avaliar a performance dos modelos utilizando métricas apropriadas para garantir sua precisão e robustez.

Ao final do projeto, espera-se obter um modelo robusto que possa prever o preço de venda de uma casa com base nas características identificadas. Além disso, o projeto proporcionará uma compreensão clara sobre quais fatores desempenham papéis mais significativos na definição do valor de uma propriedade. Essa abordagem permitirá uma negociação mais estratégica e informada no mercado imobiliário, beneficiando vendedores, compradores e investidores.

## Sumário

- [Descrição](#descrição)
- [Sumário](#sumário)
- [Instalação](#instalação)
- [Tecnologias](#tecnologias)
- [Uso](#uso)
- [Resultados](#resultados)
- [Contribuição](#contribuição)
- [Contato](#contato)

## Instalação

Para configurar o ambiente e iniciar o projeto, siga as etapas de instalação abaixo. Estas instruções garantem que todas as dependências necessárias sejam instaladas e que você possa executar o projeto localmente sem problemas.

**Exemplo:**

```bash
# Clone este repositório
git clone https://github.com/Limatrindade/house_price_prediction.git

# Entre no diretório do projeto
cd nome-do-projeto

# Acesse o notebook de sua preferência
Jupyter notebook
Google colabory
VScode com Jupyter notebook
Pycharm
Outros
```

## Tecnologias

Tecnologias e bibliotecas utilizadas no projeto.

**Exemplo:**

- **Linguagem**: Python 3.10
- **Análise de Dados**: Pandas, Numpy
- **Machine Learning**: Scikit-learn
- **Visualização de Dados**: Matplotlib, Seaborn, Plotly
- **Ambiente de Desenvolvimento**: Jupyter Notebook, VSCode
- **Versionamento de Código**: Git, GitHub
- **Outras**: Statsmodels

## Uso

Para começar a utilizar este projeto, siga as instruções abaixo. Elas irão guiá-lo desde a configuração do ambiente até a execução do código. Se você estiver interessado em explorar as funcionalidades ou adaptar o projeto para suas necessidades, os exemplos fornecidos ajudarão a facilitar o processo.

```bash
# Abra o Jupyter Notebook
jupyter notebook

# Navegue até o arquivo principal
```

## Resultados

Os resultados obtidos mostram o impacto significativo das análises realizadas, destacando insights valiosos e métricas de desempenho robustas que demonstram a eficácia das soluções propostas. Veja abaixo os principais resultados e conclusões.

**Exemplo:**

- Aparentemente, à medida que a área aumenta, o preço também aumenta. Talvez, para casas com uma área maior, os preços não estabeleçam uma relação tão linear, pois há uma explosão em determinado ponto do gráfico. Porém, essa relação linear ainda é visível.
- A observação principal é que a maioria das casas tem um preço de venda de até 1 milhão, aproximadamente, com algumas casas mais caras, em menor quantidade, ultrapassando os 2 milhões. Esse padrão sugere uma distribuição com uma cauda mais longa à direita, como frequentemente descrevemos. É crucial compreender que essa variável é a nossa resposta principal, aquela que buscamos prever com precisão.
- Para analisar cada efeito, podemos observar a area_primeiro_andar, que analisamos no modelo zero. Ela informa que, ao aumentar 1 metro quadrado de área construída no primeiro andar, esperamos que o preço de venda aumente, em média, 6.119 reais. Esse é um efeito isolado, por isso, quando comparamos um modelo com mais de uma variável explicativa, todas as outras variáveis precisam estar constantes para que esse efeito seja interpretado dessa maneira.
- Quando observamos a quantidade_banheiros, por exemplo, também temos um número bem grande, que é um efeito atrelado a essa variável. Esperamos, por exemplo, que quando construímos mais um banheiro, tenhamos um efeito de aumento do preço de venda da casa em 149.036 reais. Lembrando que todas as outras variáveis precisam estar constantes, porque esse efeito é isolado em relação à quantidade de banheiros.
- Quando falamos sobre existe_segundo_andar, temos o valor de 221.306 reais, porque estamos falando sobre o preço de venda da casa. Mas essa interpretação está ligada à natureza dessa variável ser 0 ou 1, existindo ou não. Portanto, quando a casa tem um segundo andar, esperamos que o preço de venda daquela casa aumente, em média, 221.306 reais, em comparação àquela casa que não tem o segundo andar.
- Já quando observamos a qualidade_da_cozinha_Excelente, mantendo as outras variáveis constantes, também vamos comparar se a cozinha é classificada como excelente ou não. Assim, temos um efeito bem grande: se a cozinha é classificada como excelente, temos um aumento esperado do preço de venda daquela casa em 444.391 reais. Portanto, ter uma cozinha excelente na casa valoriza bem o preço de venda.
- Todos esses números ajudam a estabelecer o preço estimado de venda da casa. Além disso, é possível prever o melhor retorno financeiro de cada atributo da casa. No cenário de uma casa na qual temos o mesmo valor de custo para construir um segundo andar e para estabelecer uma cozinha excelente, por exemplo, podemos inferir que reformar a cozinha e deixá-la excelente tem maior retorno financeiro para o preço da casa do que construir um segundo andar, somente com base nesses coeficientes.

## Contribuição

Achou o projeto interessante e quer contribuir, melhorar, ou simplesmente criar a sua própria versão? Ótimo! Siga os passos abaixo.

Exemplo:

```bash
1. Faça um fork deste repositório

2. Crie uma branch para sua feature (git checkout -b feature/nova-feature)

3. Faça commit das suas alterações (git commit -m 'Adiciona nova feature')

4. Envie para a branch original (git push origin feature/nova-feature)

5. Abra um Pull Request
```

## Contato

Gostou do que viu? Entre em contato comigo para saber mais ou discutir colaborações!

**Exemplo:**

- **Email**: [teulima20@hotmail.com](mailto:teulima20@hotmail.com)
- **LinkedIn**: [Matheus Lima](https://www.linkedin.com/in/matheus-lima-809407191/)
- **GitHub**: [Meu GitHub](https://github.com/Limatrindade)
