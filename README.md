# InvestExcelDio

Criação de planilha em Excel para simulação, previsão e controle básico de investimentos.

# Objetivo

Esta planilha de simulação subsidia o investidor com ou sem experiência a tomar decisões relevantes sobre suas aplicações financeiras, proporcionando uma visão clara de seu saldo de investimento passado, futuro ou em tempo real.

# Introdução

Seguindo o propósito desse trabalho se faz necessário buscar informações e dados financeiros em algum site ligado diretamente a atividade econômica, de preferência com dados financeiros oficiais diversificados de diversos segmentos. Investidor10.com é uma sugestão onde você terá acesso a uma infinidade de dados. ex: FIIs - MXRF11, etc...

# Desenvolvimento

Algumas questões são interessantes para nortear o desenvolvimento desse trabalho sendo elas:
* Quanto você deseja investir por mês? (aporte)
* Por quantos anos? (qtd_anos)
* Qual a taxa de rendimento mensal? (taxa_mensal)
* Patrimônio acumulado? (patrimonio)
* Dividendos mensais?

# Base

A base engloba um Banner principal com logo. <img width="1079" height="243" alt="Image" src="https://github.com/user-attachments/assets/009e29b9-a2d7-4b55-98c0-3594beb0ac30" />

Uma tabela com cabeçalho ( Investimento Mensal ) e todas as questões anteriores distribuidas em 5 linhas numa única coluna seguida de outra onde serão inseridos os dados principais, ou seja, uma tabela com 6 linhas sendo uma delas para cabeçalho e 2 colunas.
<img width="709" height="181" alt="Image" src="https://github.com/user-attachments/assets/121f4329-6aee-48d2-a4e3-419910e837ca" />

# Simulador de acúmulo de patrimônio

Fórmula utilizada para patrimônio acumulado: =VF(taxa_mensal;qtd_anos*12;aporte*-1);
Fórmula utilizada para dividendos mensais: =patrimonio*Rendimento Carteira.

# Simulador de cenários

Essa tabela terá cabeçalho (Cenários), 05 linhas e 3 colunas, onde cada linha da 1ª Coluna terá variação de tempo em anos( 2, 5, 10, 20 e 30) e a 3ª Coluna será de dividendos que é o resultado da VF (*)vezes o Rendimento Carteira da planila de configurações.
A fórmula utilizada para patrimônio acumulado será =VF(taxa_mensal;qtd_anos*12;aporte*-1), o "-1" no final da fórmula inverte o sinal negativo para positivo nmo resultado.
A tecla F4 é utilizada para congelar os valores das: Apertanto 1 vez congela linha/coluna, na segunda vez somente linha e na terceira vez somente coluna.
para facilitar a utilização da quantidade de anos na fórmula, insere na frente de cada linha o número de anos correspondente ( fonte em vermelho) e depois utilize a cor branca para torná-la invisível.
<img width="744" height="198" alt="image" src="https://github.com/user-attachments/assets/71071e64-e77a-4cfc-9efc-df0c0b2d5b4c" />


# Variáveis Globais

As variáveis globais são utilizadas para diversos fins, no nosso caso será uma tabela com 4 linhas sendo uma delas para cabeçalho (Configurações) e 2 colunas. Na primeira coluna teremos as inscrições: salário, rendimento em carteira e sugestão de investimento:
<img width="707" height="123" alt="Image" src="https://github.com/user-attachments/assets/80830bf5-33a4-4d04-a7c1-520c04a2b3f1" />

# Nomeando intervalos

No canto esquerdo superior da planilha existe uma caixa de nomes, que normalmente exibe a referência de posição da célula, é nessa caixa que você irá renomeá-la.
Para renomear uma referência de célula (Apelido) não esqueça dos detalhes principais, o nome não pode ter espaço e sim Underline, não pode ter acento e deverá ser todo em letra minúscula.
Se você apertar a tecla CTRL + F3 juntas abrirá a janela de "Gerenciador de nomes" e somente a tecla F3 abre a janela de "Colar nomes" para que após selecionado insira a referência na fórmula desejada.
A substituição da referência alfa-númerica da célula para nome facilita a identificação e localização da célula, independente de onde está sendo aplicada.
A tecla CTRL+ Shift é utilizada para ocultar colunas e deixar a área da planilha limpa e de fácil visualização.

# Criando uniformidade visual

A visualização colunar da planilha a torna mais agradável. 
Em documentos formais é recomendado utilizar o formato contábil para valores monetários, porém será utilizado nessa planilha o formato "Moeda".
Quanto ao alinhamento dos dados para texto é indicado todo a esquerda e para números centralizados.
Para selecionar áreas distintas ao mesmo tempo, utilize o mouse/cursor com a tecla CTRL apertada.
Mesclar células é um mecanismo bem utilizado para ajustar o conteúdo das linhas e colunas buscando maior uniformidade no alinhamento.
Nas células o ideal é utilizar cores claras e nos cabeçalhos cores fortes.
Geralmente as células preenchidas com a cor cinza claro indicam uma preferência em não alterá-las.
A fonte recomendada nesse trabalho é a Segoe UI.
Ocultar a barra de tarefas suaviza a visualização.
A borda das tabelas recomenda-se linhas um pouco mais espessas e as linhas internas o mais finas possível.

# Simulador de perfil

Os tipos de Perfil de investidores utilizados nessa planilha são:
  * a) AGRESSIVO;
  * b) MODERADO e
  * c) CONSERVADOR.

Para isso vamos construir uma tabela com 2 linhas e duas colunas. Na primeira linha e primeira coluna o título PERFIL deve ser preenchido com cor clara e na segunda linha o texto "Valor a ser investido por mês" em negrito.

<img width="719" height="64" alt="Image" src="https://github.com/user-attachments/assets/a75ea2e2-8a4c-478b-8c2e-cfdb0bf60f26" />


Na primeira linha da segunda coluna inserir uma caixa de listagem.

<img width="714" height="83" alt="image" src="https://github.com/user-attachments/assets/5ee7939b-669a-4225-9ff0-725a05bd0c1d" />

A segunda tabela logo abaixo terá 8 linhas e 3 colunas, a primeira linha terá o título de cada coluna sendo a primeira TIPO DE FII, a segunda coluna PERCENTUAL SUGERIDO e a terceira coluna VALORES.
 * Tipos de FII: Papel, Tijolo, Híbridos, FOFs, Desenvolvimento e Hotelarias. 
 * Percentual Sugerido para o perfil conservador: 30%, 50%, 10%, 10%, 0% e 0%.
 * Valores: É o resultado do Percentual Sugerido.

<img width="712" height="191" alt="image" src="https://github.com/user-attachments/assets/563ee991-74d8-4c71-8387-2dd8a38a6567" />


# Tabela de Apoio

A tabela de apoio fica oculta numa segunda planilha, nomeie e insira uma tabela.
<img width="477" height="60" alt="image" src="https://github.com/user-attachments/assets/578c90e9-c845-4e1e-a048-3b52aba22328" />

Inicie a nova tabela de apoio com apenas 7 linhas e 3 colunas. Na primeira coluna cole os valores do PERFIL , na segunda coluna os TIPO DE FIIs e na terceira coluna as porcentagens.

<img width="397" height="169" alt="image" src="https://github.com/user-attachments/assets/85585957-f87a-45b2-b39c-3f1513e51bb6" />

Para fazer os cálculos dinâmicamente utilize uma CHAVE COMPOSTA. Na tabela já existente insira uma nova coluna do lado ESQUERDO da coluna PERFIL, essa nova coluna terá o título CHAVE. Portanto, a Tabela estará exibindo os valores do perfil conservador e seus padrões.

<img width="663" height="209" alt="Image" src="https://github.com/user-attachments/assets/691b007b-1cde-46e7-93b3-090ffd9fd1b9" />

Feito isso, copiar as 6 linhas com todo seu conteúdo até a última coluna e em seguida colar abaixo na sequência lógica e no mesmo alinhamento mudando o perfil de conservador para moderado. Repita o mesmo procedimento para o PERFIL Agressivo. 
Dica para a coluna de PERFIL com textos iguais ( para colar os valores a partir da primeira linha preenchida selecione todas as desejadas, aperte e solte a tecla F2, escreva o texto e aperte CTRL + enter).
Na sequência e na quarta coluna deverão ser preenchidos os campos de acordo com o perfil expresso na linha.
No final a tabela ficará com 19 linhas sendo a primeira para os titulos das colunas e 18 linhas em 3 blocos de perfil.
Percentual Sugerido para o perfil conservador: 30%, 50%, 10%, 10%, 0% e 0%.
Percentual Sugerido para o perfil moderado: 32%, 40%, 8%, 10%, 10% e 10%.
Percentual Sugerido para o perfil agressivo: 50%, 10%, 5%, 5%, 20% e 10%.

<img width="625" height="434" alt="Image" src="https://github.com/user-attachments/assets/b59d080d-fd80-46fd-b6c3-5ba2f2dcaebc" />

# Construir a PROCV

Clique em um espaço aleatório próximo da tabela, selecione duas células uma ao lado da outra, vá em estilos no menu e clique em "Estilos de Célula" escolhendo um dos estilos que mais lhe agradar. Cole um texto de qualquer linha da coluna CHAVE ( Moderado-Tijolo) e cole na primeira célula.
O que difere um perfil do outro será a CHAVE única utilizada na fórmula/função PROCV = Procura Vertical. Para isso é necessário a combinação de dois campos específicos com o PROCV gerando dessa forma uma chave única, ou seja, o excel procura um valor determinado nas linhas de uma coluna e assim que localizado tras o valor desejado. Portanto na busca ele encontra primeiro a linha e na sequência a coluna indicada na fórmula.
Selecione a segunda célula do PROCV e insira a fórmula. PROCV(valor_procurado;matriz_tabela;núm_índice_coluna'[procurar_intervalo]).

<img width="973" height="484" alt="image" src="https://github.com/user-attachments/assets/691c29ba-5815-44d3-b5fb-bbb10c516c2c" />

# PROCV no Simulador

Retorne na tabela do SIMULADOR DE PERFIL e na coluna PERCENTUAL SUGERIDO insira na primeira linha o PROCV com tipo do perfil e o valor a ser inserido por mês (ex: moderado/papel). Na fórmula o FALSO é utilizado para correspondência exata na busca.
A tabela de apoio facilita caso tenham novos valores a serem declarados.

<img width="732" height="254" alt="image" src="https://github.com/user-attachments/assets/2a98b3b3-c23a-4be1-9a74-0ca43ca94ddd" />

# Inserindo Gráfico

Selecionar na tabela a área de Tipo de FII e Percentual Sugerido, ir em Inserir gráficos e escolher o modelo desejado (Pizza), formate o gráfico como desejar.
Mudando o perfil na caixa de listagem o gráfico irá exibir de acordo com a sua escolha.

<img width="551" height="257" alt="image" src="https://github.com/user-attachments/assets/fa7340cd-ca91-45c2-b09e-e4d2355f1f3e" />

Essas instruções por si não eximem a necessidade de assistir o vídeo do Professor Felipe Aguiar da DIO, porém subsidiam na facilidade e entendimento.

O que fizemos:
Banner, projeções com tabela de apoio, intervalos nomeados, uniformidade visual e gráficos.
















