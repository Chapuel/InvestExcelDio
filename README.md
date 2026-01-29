# InvestExcelDio

Criação de planilha em Excel para simulação, previsão e controle básico de investimentos.

# Objetivo

Esta planilha de simulação subsidia o investidor com ou sem experiência a tomar decisões relevantes sobre suas aplicações financeiras, proporcionando uma visão clara de seu saldo de investimento passado, futuro ou em tempo real.

# Introdução

Seguindo o propósito desse trabalho se faz necessário buscar informações e dados financeiros em algum site ligado diretamente a atividade econômica, de preferência com dados financeiros oficiais diversificados de diversos segmentos. Investidor10.com é uma sugestão onde você terá acesso a uma infinidade de dados. ex: FIIs - MXRF11.

# Desenvolvimento

Algumas questões são interessantes para nortear o desenvolvimento desse trabalho por exemplo:
Quanto você deseja investir por mês?
Por quantos anos?
Qual a taxa de rendimento mensal?
Patrimônio acumulado?
Dividendos mensais?

# Base

A base engloba uma tabela ( Simulador de Patrimônio ) com cabeçalho e todas as questões anteriores distribuidas em 5 linhas numa única coluna seguida de outra onde serão inseridos os dados principais ou seja, uma tabela cabeçalho, 5 linhas e duas colunas.

# Simulador de acumulo de patrimônio

Formulas utilizadas para patrimônio acumulado =VF(taxa_mensal;qtd_anos*12;aporte*-1); Dividendos mensais =patrimonio*rendimento_carteira.

# Simulador de cenários

Essa tabela terá cabeçalho, 05 linhas e 2 colunas, onde cada linha da 1ª Coluna terá variação de tempo em anos( 2, 5, 10, 120, e 30).
A fórmula utiliza será =VF(taxa_mensal;qtd_anos*12;aporte*-1), o "-1" no final da fórmula inverte o sinal negativo do resultado para positivo.
A tecla F4 é utilizada para congelar os valores.
para facilitar a utilização da quantidade de anos na fórmula, insere na frente de cada linha o número de anos correspondente e depois utiliza a fonte branca para tornar invisível.













