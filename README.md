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

A base engloba um Banner principal com logo, uma tabela com cabeçalho ( Investimento Mensal ) e todas as questões anteriores distribuidas em 5 linhas numa única coluna seguida de outra onde serão inseridos os dados principais ou seja, uma tabela com 6 linhas sendo uma delas para cabeçalho e 2 colunas.

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
A tecla CTRL+ Shift é utilizada para ocultar colunas e deixar a área da planilha limpa e de fácil visualização.

# Criando uniformidade visual

A visualização colunar da planilha a torna mais agradável. 
Em documentos formais é recomendado utilizar o formato contábil para valores monetários, porém será utilizado nessa planilha o formato "Moeda".
Quanto ao alinhamento dos dados para texto é indicado todo a esquerda e para números centralizados.
Para selecionar áreas distintas ao mesmo tempo utilize o mouse/cursor com a tecla CTRL apertada.
Mesclar é um mecanismo bem utilizado para ajustar as linhas e colunas buscando maior uniformidade no alinhamento.
Nas células o ideal é utilizar cores claras e cabeçalhos as cores mais fortes.
Geralmente as células preenchidas com a cor cinza claro indicam uma preferência em não alterá-las.
A fonte recomendada nesse trabalho é a Segoe UI.
Ocultar a barra de tarefas suaviza a visualização.
A borda das tabelas sempre com uma linha um pouco mais grossa e as linhas internas mais finas.

# Simulador de perfil

Os tipos de Perfil de investidores utilizados nessa planilha são:
  a) AGRESSIVO;
  b) MODERADO e
  c) CONSERVADOR.

Para isso vamos construir uma tabela com 2 linhas e duas colunas. Na primeira linha e primeira coluna o título PERFIL deve ser preenchido com cor clara e na segunda linha o texto "Valor a ser investido por mês" em negrito.
Na primeira linha da segunda coluna inserir uma caixa de listagem.

A segunda tabela logo abaixo terá 8 linhas e 3 colunas, a primeira linha terá o título de cada coluna sendo a primeira TIPO DE FII, a segunda coluna PERCENTUAL SUGERIDO e a terceira coluna VALORES.
 * Tipos de FII: Papel, Tijolo, Híbridos, FOFs, Desenvolvimento e Hotelarias. 
 * Percentual Sugerido para o perfil conservador: 30%, 50%, 10%, 10%, 0% e 0%.
 * Valores: É o resultado do Percentual Sugerido.

# Tabela de Apoio

A tabela de apoio fica oculta na aba de uma nova planilha. Nessa aba insira uma tabela com 7 linha e 3 colunas. Na primeira coluna cole os valores do PERFIL , na segunda coluna os TIPO DE FII e na terceira coluna as porcentagens.

Para fazer os cálculos dinamicamente utilize a CHAVE COMPOSTA. Na tabela já existente insira uma nova coluna Do lado ESQUERDO da coluna PERFIL, essa nova coluna terá o título CHAVE. Portanto, a Tabela estará exibindo os valores do perfil conservador e seus valores. Feito isso, copiar as 6 linhas de valores e colar embaixo na sequência, porém mudando o perfil para moderado ( para colar os valores a partir da primeira linha preenchida selecione todas as desejadas, aperte a tecla F2 escreva o texto aperte CTRL+enter). Na sequência o percentual na quarta coluna deverá ser preenchida de acordo com o perfil expresso na linha.
No final a tabela ficará com 19 linhas sendo a prim eira para os titulos das colunas e 18 linhas em 3 blocos de perfil.
Percentual Sugerido para o perfil moderado: 32%, 40%, 8%, 10%, 10% e 10%.
Percentual Sugerido para o perfil agressivo: 50%, 10%, 5%, 5%, 20% e 10%.

# Construir a PROCV

Clique em um espaço aleatório próximo da tabela, selecione duas células uma ao lado da outra, vá em estilos e clique em Estilos de célula escolhendo um dos estilos existentes. Cole um texto de qualquer linha da coluna CHAVE ( Moderado-Tijolo) e cole na primeira célula.

O que difere um perfil do outro será a CHAVE única necessária para a formula/função PROCV (Procura Vertical). Para que eu consiga pegar uma combinação de dois campos específicos com o PROCV eu preciso de uma chave única, ou seja, ele procura um valor na coluna e assim que localizado a linha ele tras o valor da coluna especificada na mesma linha. Portanto encontra a linha e depois a coluna.
Selecione a segunda célula do PROCV e insira a fórmula. PROCV(valor_procurado;matriz_tabela;núm_índice_coluna'[procurar_intervalo]).

Retorne a tabela do simulador de perfil e na coluna PERCENTUAL SUGERIDO insira na primeira linha o PROCV com tipo do perfil e o valor a ser inserido por mês (ex: moderado/papel). na fórmula o FALSO será utilizado para correspondência exata.

A tabela de apoio facilita caso tenham novos valores a serem declarados.

# Inserindo Gráfico

Selecionar na tabela a área de Tipo de FII e Percentual Sugerido, ir em Inserir gráficos e escolher o modelo desejado (Pizza), formate o gráfico como desejar.
mudando o perfil o gráfico irá exibir de acordo com a escolha.

Essas instruções por si não eximem a necessidade de ver o vídeo do Professor Felipe Aguiar da DIO, porém subsidiam a clareza algumas necessidades. 
https://web.dio.me/lab/criando-uma-ferramenta-de-controle-de-investimentos-com-excel/learning/1f9861d5-d23d-42d7-9ed0-efa937cb0087?back=/track/santander-excel-com-inteligencia-artificial. 

O que fizemos:
Banner, projeções com tabela de apoio, intervalos nomeados, uniformidade visual e gráficos.

https://web.dio.me/lab/criando-uma-ferramenta-de-controle-de-investimentos-com-excel

















