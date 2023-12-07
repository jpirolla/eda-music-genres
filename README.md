Projeto de análise exploratória utilizando o dataset "Music: 1950 - 2019" disponível no OpenML. 
## Motivação
A análise destes dados é relevante dado que a partir dele podemos obter insights sobre tendências musicais, preferências do público ao longo das décadas, ou até mesmo refletir aspectos culturais e sociais do período. Compreender tais aspectos pode ser útil para profissionais da indústria musical, pesquisadores e entusiastas, promovendo uma apreciação mais abrangente da música e suas transformações ao longo do tempo.

## Sobre o dataset
Nosso dataset abarca mais de 28 mil músicas de mais de 5 mil artistas diferentes. O período analisado é de 70 anos, onde temos 7 gêneros musicais diferentes. Todas as músicas contêm letras em inglês, mas não foi possível verificar se seriam todas as músicas originadas em um único país.
Cada música é associada a 16 parâmetros de "tópicos" diferentes, que foram organizados de acordo com as 10 palavras mais frequentes em suas letras.


## Metodologia
A ferramenta usada na análise foi a plataforma Colab, do Google, e linguagem Python. As bibliotecas usadas foram: openml, pandas, numpy, seaborn e matplotlib. A seguir temos uma breve descrição de como cada uma delas foram utilizadas:
- Openml: Esta biblioteca nos permitiu importar facilmente o nosso amplo conjunto de dados, o que nos permitiu explorar características importantes das músicas analisadas;
- Pandas: Utilizamos Pandas para a manipulação e limpeza dos dados. Com ela, conseguimos realizar operações de filtragem, tratamento de dados ausentes e organização dos dados em um formato adequado para análise. O Pandas também nos permitiu calcular as estatísticas descritivas;
- NumPy: Foi uma biblioteca importante para realizarmos operações matemáticas em arrays multidimensionais, como a contagem de palavras nas letras das músicas;
- Seaborn: Para a visualização dos dados, utilizamos o Seaborn para plotar gráficos diversos que nos permitiram a identificação de padrões e insights relevantes nos dados;
- Matplotlib: Esta biblioteca foi utilizada em conjunto com o Seaborn para a criação de gráficos adicionais e personalizados. Com esta biblioteca pudemos customizar os gráficos gerados, ajustando cores, legendas e outros elementos visuais de acordo com nossas necessidades.


## Resumo do processo

O presente trabalho tem como objetivo realizar uma análise exploratória do conjunto de dados "[Music Dataset 1950 to 2019](https://openml.org/search?type=data&status=active&id=43845)". . Para estabelecer um guia da exploração levantamos hipóteses iniciais no intuito de validá-las ou refutá-las conforme o comportamento dos dados.

Dentre os questionamentos estabelecidos, temos:

1. Há dados que não contribuem em nenhum aspecto nas análises?
2. Há dados faltantes no dataset? Qual é a melhor forma de tratá-los no contexto atual?
3. Os gêneros musicais formam classes que estão balanceadas ou desbalanceadas? Qual a porcentagem de cada um?
4. Existem dados que não são essenciais, ou seja, que são derivados de outros dados?
5. O número de observações (músicas) no dataset é uniforme no decorrer dos anos?
6. Qual é a distribuição das features desse dataset?
7. Como os atributos evoluíram no tempo?
8. Qual a diferença da média dos atributos por gênero?
9. Qual gênero se sobressaiu em cada década?
10. Qual autor lançou mais músicas em cada década?
11. Quais foram as músicas mais obscenas por década e quem são os autores?
12. Quais autores possuem músicas com maior caráter violento seus respectivos gêneros?
13. Quais gêneros são mais dançáveis?
14. Não se faz mais música como antigamente?
15. Evolução dos atributos no tempo

Ademais, durante o processo realizamos algumas análises secundárias (como no atributo 'len', por exemplo) e realizamos o processo de feature engineer quando cabível, criando novas features (por exemplo para análise conforme a década).


## Visualizações
Os gráficos das análises estão contidos no arquivo .ipynb presente em tal repositório. 

## Conclusão
Ao longo das décadas, observamos mudanças significativas nos gêneros musicais trabalhados aqui. Após nossas análises, fomos capazes de responder às nossas hipóteses e questionamentos iniciais, além de identificar insights interessantes.

Sobre as hipóteses e questionamentos iniciais:
- Qual gênero se sobressaiu em cada década?
  - Pop foi o gênero predominante ao longo de quase todas as décadas, com exceção apenas da década de 1950, onde o Jazz foi o gênero mais predominante.

- Qual autor lançou mais músicas em cada década?
  - 1950: Hank Mobley - Jazz;
  - 1960: Lorne Greene - Country;
  - 1970: Frank Zappa - Jazz;
  - 1980: The Replacements - Country;
  - 1990: Project Pat - Pop;
  - 2000: (hed) p. e. - Rock;
  - 2010: Rihanna - Pop.

- Idosos costumam comentar que não se faz música como antigamente. O quanto isto é verdade?
  - Apesar de “qualidade musical” ser subjetivo, se tomarmos como métrica a frequência de músicas com letras agressivas e obscenas, ao lado do uso de músicos reais em vez de instrumentos sintetizados, é possível afirmar que, de fato, não se faz música como antigamente.

- Quais foram os gêneros musicais mais obscenos?
  - Hip hop foi, disparado, o gênero musical com mais letras obscenas apesar de representar apenas aproximadamente 3% de todas as músicas analisadas.

- E quais foram os mais violentos?
  - Rock é o gênero musical mais violento, com reggae em segundo lugar, e blues em terceiro. O que é interessante, já que reggae é um estilo musical que se originou no movimento hippie, que pregava paz e amor.

- Músicas acústicas costumam ser mais amorosas?
  - De fato, as músicas mais acústicas apresentaram, também, uma taxa maior de romantismo.

- Pop é o gênero musical mais dançante?
  - Não! Hip hop e Reggae são os gêneros mais dançantes. Pop está em quarto lugar na lista, atrás de Country.

### Sobre os insights:
- Tanto o Rock quanto o Jazz e Country tiveram seu período de maior expressividade, sendo coerente com a cultura geral da época. Apesar disso, ainda sim o gênero Pop sempre foi mais popular, com exceção de Jazz na década de 50;
- O número de palavras nas letras das músicas aumentou, enquanto os trechos instrumentais diminuíram ao passar dos anos;
- Violência e Obscenidade são aspectos de letras de músicas que vêm aumentando com o passar do tempo. Estariam as pessoas se tornando mais violentas e obscenas, talvez? Enquanto isso, o romantismo teve uma queda brusca com o tempo.
- De forma contraintuitiva, observamos que as músicas com tópicos de violência tinham palavras relacionadas à família e espiritualidade. Pode ser um indicativo de que estes sejam os principais objetos da violência das letras destas músicas.
- Á medida em que as músicas foram deixando de serem tocadas por músicos reais, o uso de efeitos sintetizados aumentou junto da dançabilidade, energia e loudness. Tal constatação é totalmente condizente com o nosso período cultural atual: tecnologia substituindo seres humanos, pressa, busca incessante por dopamina em redes sociais, etc.

Esses insights fornecem uma compreensão mais profunda sobre a evolução da música ao longo das décadas, as preferências do público e os aspectos culturais e sociais refletidos nas músicas. No entanto, é importante destacar que a análise foi baseada em um conjunto de dados específico e pode não representar a totalidade da música ao longo do tempo. Em suma, esta análise de dados nos permite reconhecer como a música é uma expressão cultural dinâmica e influenciada por diversos fatores.

Por fim, é importante ressaltar que tais análises foram feitas utilizando dados já classificado conforme o gênero. Assim, é possível que haja eventuais ruídos tal como expresso na análise dos dados faltantes, onde o gênero rotulado (hip hop) não condizia com o real gênero da música.
