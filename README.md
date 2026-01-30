# InvestExcelDio

Criação de planilha em Excel para simulação, previsão e controle básico de investimentos.

# Objetivo

Esta planilha de simulação subsidia o investidor com ou sem experiência a tomar decisões relevantes sobre suas aplicações financeiras, proporcionando uma visão clara de seu saldo de investimento passado, futuro ou em tempo real.

# Introdução

Seguindo o propósito desse trabalho se faz necessário buscar informações e dados financeiros em algum site ligado diretamente a atividade econômica, de preferência com dados financeiros oficiais diversificados de diversos segmentos. Investidor10.com é uma sugestão onde você terá acesso a uma infinidade de dados. ex: FIIs - MXRF11.

# Desenvolvimento

Algumas questões são interessantes para nortear o desenvolvimento desse trabalho e no nosso caso serão:
Quanto você deseja investir por mês? (aporte)
Por quantos anos? (qtd_anos)
Qual a taxa de rendimento mensal? (taxa_mensal)
Patrimônio acumulado? (patrimonio)
Dividendos mensais?

# Base

A base engloba uma tabela com cabeçalho ( Investimento Mensal ) e todas as questões anteriores distribuidas em 5 linhas numa única coluna seguida de outra onde serão inseridos os dados principais ou seja, uma tabela com 6 linhas sendo uma delas para cabeçalho e 2 colunas.

# Simulador de acumulo de patrimônio

Fórmulas utilizadas para patrimônio acumulado =VF(taxa_mensal;qtd_anos*12;aporte*-1); Dividendos mensais =patrimonio*Rendimento Carteira.

# Simulador de cenários

Essa tabela terá cabeçalho (Cenários), 05 linhas e 3 colunas, onde cada linha da 1ª Coluna terá variação de tempo em anos( 2, 5, 10, 20 e 30) e a 3ª Coluna será de dividendos que é o resultado da VF vezes o Rendimento Carteira da planila de configurações.
A fórmula utilizada será =VF(taxa_mensal;qtd_anos*12;aporte*-1), o "-1" no final da fórmula inverte o sinal negativo do resultado para positivo.
A tecla F4 é utilizada para congelar os valores.
para facilitar a utilização da quantidade de anos na fórmula, insere na frente de cada linha o número de anos correspondente e depois utiliza a fonte branca para tornar invisível.

# Variáveis Globais

As variáveis globais são utilizadas para diversos fins, no nosso caso será uma tabela com 4 linhas sendo uma delas para cabeçalho (Configurações) e 2 colunas. Na primeira coluna teremos as inscrições: salário, rendimento em carteira e sugestão de investimento.

# Nomeando intervalos
No canto esquerdo superior da planilha existe uma caixa de nomes, que normalmente exibe a referência de posição da célula, é nessa caixa que você irá renomeá-la.
Para renomear uma referência de célula (Apelido) não esqueça dos detalhe principais, o nome não pode ter espaço e sim Underline, não pode ter acento e deverá ser todo em letra minúscula.
Se você apertar a tecla CTRL + F3 juntas abrirá a janela de "Gerenciador de nomes" e somente a tecla F3 abre a janela de "Colar nomes" para que após selecionado insira a referência na fórmula desejada.
A substituição da referência alfa-númerica da célula para nome, facilita a identificação e localização da célula independente de onde está sendo aplicada.








