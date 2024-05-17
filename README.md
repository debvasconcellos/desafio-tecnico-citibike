# DESAFIO TÉCNICO - FICHA TÉCNICA

# Ficha Técnica: Desafio Técnico

## Título do Projeto: Cicloviajes

---

## Objetivo

Realizar uma análise exploratória de um conjunto de dados do programa de compartilhamento de bicicletas. Observando medidas gerais para compreensão da dinâmica do programa na cidade de Nova Iorque. 

---

## Equipe

Débora Vasconcellos

---

## Ferramentas e Tecnologias

Google Big Query e Looker Studio

---

## Processamento e Análises

---

### Limpeza dos dados e Criação de Variáveis

***Tabela “citibike_trips_explore”***:
Amostra com 50.000 casos (base original com 58.937.715). 

Transformei “stoptime” de variável TIMESTAMP para DATE criando a variável “stopdate”. 

Transformei a métrica de “timeduration” de segundos para minutos criando a variável “timedurationminutes”

Transformei a variável “birth_year” em idade criando a variável “age”.

Transformei a variável “age” em “age_group” criando as faixas etárias: 22-30; 31-40, 41-50, 51-60, 60+

---

---

## Resultados e Conclusões

O Programa de compartilhamento de bicicletas do Citi Bank foi lançado em 2013 na cidade de Nova Iorque. Com duas modalidades para os usuários, o programa possui o plano Anual (Subscriber) e planos de curto prazo (Customer) que podem ser passes de 24 horas ou para 3 dias.

Na amostra observada, podemos analisar o comportamento das viagens referentes ao intervalo de anos 2015-2018. 

Com uma média de 53 viagens por dia, o programa apresentou uma tendência de crescimento ao longo do período analisado, havendo uma queda nas viagens de 2018. 87,9% dos usuários são do plano anual (Subscriber)

67,9% dos usuários se identificaram como Homens, 

20,5% são Mulheres e os demais não se identificaram no aplicativo. 

A faixa etária com mais usuários é a de 31-40 anos (36,19%), seguida por 41-50 anos (25,25%). A faixa etária com menos usuários foi a de 22-30 anos. 

O tempo médio das viagens é de 16 minutos, entretanto há uma grande variância nos dados. Já que o tempo mínimo foi de 1 minuto, enquanto o máximo de 55 mil minutos. O desvio padrão de 256 minutos aponta que há muita dispersão. 

De modo geral, podemos perceber que o público de homens adultos é preponderante no programa. Há uma dispersão significativa na duração das viagens, o que denota uma multiplicidade de usos. Apesar da média girar em torno de 16 minutos, o desvio padrão nos indica que há casos que se distanciam muito dessa média. Dessa forma, podemos inferir que os usos tanto podem ser para situações pontuais e rápidas, como usuários inscritos no plano anual que ficam com as bicicletas por muito mais tempo.  
Complementando a análise com outros estudos realizados sobre o programa, podemos inferir que a presença preponderante do público masculino necessita de ser interpretado a partir de aspectos socioculturais. As mulheres apresentam uma maior vulnerabilidade para violências e acabam por ter mais receio em se locomoverem de bicicleta pelos centros urbanos. Segundo Kaufman et al. (2015), as mulheres optam por estações do programa com maior segurança em seu entorno e preferem utilizar os serviços em dias com clima mais estável e ameno. Além disso, os usos do serviço por homens e mulheres se diferencia pelas suas atividades. As mulheres procuram mais o serviço para transporte de crianças para escolas, realizar atividades pontuais ao redor de sua residência. Enquanto os homens, teriam uma maior inserção da bicicleta para múltiplas atividades como trabalho, passear pelo parque, encontrar com colegas, etc. (Kaufman, et.al, 2015).

---

## Limitações/Próximos Passos

Para uma análise mais robusta certos pontos poderiam ser melhor investigados com a adição de mais dados:

- A queda de viagens em 2018: os dados trabalhos não possui informações de todos os meses de 2018 o que pode ter impactado no menor número de casos. Dessa forma, não há como afirmar se houve uma queda de viagens nesse ano e quais motivos poderiam ter acarretado.
- Gênero: Seria interessante realizar uma pesquisa com as usuárias do serviço entender como as mulheres que fazem o uso do programa pensam sobre ele e entender como tornar o uso de bicicletas por mulheres uma possibilidade mais segura em grandes centros urbanos.

O banco original possui 58.937.715 viagens registradas, o tamanho robusto dos dados tornou-se um empecilho para realizar a análise de forma gratuita no BigQuery. Dessa form,a optamos por usar uma amostra. De toda forma, com mais dedicação e conhecimento sobre o setor de transporte urbano poderíamos trazer mais inferências para esse pequeno estudo exploratório. 

---

## Links de interesse

**Fonte**:

[NYC Citi Bike Trips – Marketplace – Console do Google Cloud](https://console.cloud.google.com/marketplace/product/city-of-new-york/nyc-citi-bike?project=data-sandbox-319716)

Kaufman, et.al. Citi Bike: The First Two Years. Rudin Center for Transportation, 2015 : [Citi Bike Formatted (nyu.edu)](https://wagner.nyu.edu/files/faculty/publications/Citi_Bike_First_Two_Years_RudinCenter.pdf)

[Citi Bike System Data | Citi Bike NYC | Citi Bike NYC](https://citibikenyc.com/system-data)

**Dashboard**: https://lookerstudio.google.com/reporting/602b6e53-073e-40db-be8e-4db5d31bfbfe


---

---
