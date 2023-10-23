# BASE_DE_DADOS_ESPB
                                      Trabalho de base de dados
Modelo relacional

Os futuros usuários de grandes bancos de dados devem ser protegidos contra ter que saber como os dados são organizados na máquina . Um serviço de alerta que fornece essas informações não são uma solução satisfatória. Atividades de usuários nos terminais e a maioria dos programas de aplicativos deve permanecer não afetado quando a representação interna dos dados é alterada e mesmo quando alguns aspectos da representação externa

A visão relacional dos dados descritos em

Seção 1 parece ser superior em vários aspectos ao gráfico ou modelo de rede atualmente em voga para sistemas inferenciais. Ele fornece um meio de descrever dados com sua estrutura natural apenas - isto é, sem superimapresentando qualquer estrutura adicional para representação da máquina finalidades. Consequentemente, fornece uma base para um alto nível linguagem de dados que irá render a máxima independência ser entre os programas, por um lado, e a representação da máquina e organização de dados, por outro.

O modelo de rede, por outro lado, gerou um número de confusões, a menos das quais é o engano a derivação de conexões para a derivação de rela-são alterados. Mudanças na representação de dados serão frequentemente.
Finalmente, a visão relacional permite uma avaliação mais clara tráfego e crescimento natural dos tipos de informação armazenada.

Os sistemas de dados formatados não inferenciais existentes fornecem aos usuários sistemas de dados, e também os méritos relativos de representações concorrentes de dados dentro de um modelos dos dados. Na Seção 1, inadequações desses modelos sistema único. Exemplos dessa perspectiva mais clara são são discutidos. Um modelo baseado em relações n-árias, uma normal citado em várias partes deste artigo. Implementações de formulário para relações de banco de dados, e o conceito de um universal sistemas para apoiar o modelo relacional não são discutidos.
necessária como resultado de mudanças na consulta, atualização e relatório sublinguagem de dados são introduzidos. Na Seção 2, certas operações ações sobre as relações são discutidas e aplicado aos problemas de redundância e consistência no modelo do usuário.

DEPENDÊNCIAS DE DADOS NOS SISTEMAS ATUAIS

O fornecimento de tabelas de descrição de dados em recentemente desistemas de informação desenvolvidos representam um grande avanço em direção ao objetivo de independência de dados . Tais tabelas facilitar a mudança de certas características dos dados representados sentação armazenada em um banco de dados. No entanto, a variedade de características de representação de dados que podem ser alteradas sem prejudicar logicamente alguns programas de aplicativos é ainda bastante limitado. Além disso, o modelo de dados com o qual a interação dos usuários ainda está desordenada com propriedades representacionais direitos, particularmente no que diz respeito à representação de collições de dados . Três de os principais tipos de dependências de dados que ainda precisam a serem removidos são: dependência de ordenação, dependência de indexação e dependência do caminho de acesso. Em alguns sistemas, estes as dependências não são claramente separáveis umas das outras.
Dependência de pedidos. Elementos de dados em um banco de dados pode ser armazenado de várias maneiras, algumas envolvendo não se preocupando com o pedido, alguns permitindo que cada elemento para participar de apenas um pedido, outros permitindo cada elemento para participar em vários pedidos. Vamos considerar os sistemas existentes que requerem ou permitem dados elementos a serem armazenados em pelo menos uma ordem total que é intimamente associado ao pedido determinado por hardware de endereços. Por exemplo, os registros de um arquivo relativo as peças podem ser armazenadas em ordem crescente por série de peças número. Esses sistemas normalmente permitem a aplicação gramas para assumir que a ordem de apresentação dos registros de tal arquivo é idêntico ao pedidos armazenados. Esses programas de aplicação que levam vantagem da ordem armazenada de um arquivo provavelmente falhará operar corretamente se por algum motivo for necessário.

UMA VISÃO RELACIONAL DOS DADOS

O termo relação é usado aqui em sua matemática aceita sentido matemático. Conjuntos dados $ 1, $ 2, • • •, S ~ , mas possuem significados distintos em relação ao relação. A relação descrita é chamada de componente. É um um papel crítico no problema de explosão de peças.
Normalmente, um domínio é chamada de chave primária. No exemplo acima, o número da peça seria uma chave primária, enquanto a cor da peça não seria. Uma chave primária não é redundante se for um domínio simples ou uma combinação de modo que nenhum dos domínios simples participantes seja são ou mais domínios exigimos emfunção cada caso que dois o nome de domínio sejaidênticos, qualificado por uma distinta nome, que serve para identificar o papel desempenhado por aquele domínio na relação dada. Por exemplo, na relação componente da Figura 2, a primeira parte do domínio pode ser qualificado pelo nome da função sub e o segundo por super, então que os usuários podem lidar com o componente de relacionamento e seus domínios - , quantidade - sem consideração supérfluo na identificação única de cada elemento.
A relação pode possuir mais de um primário não redundante chave. Este seria o caso no exemplo se partes diferentes sempre receberam nomes distintos. Sempre que uma relação tem duas ou mais chaves primárias não redundantes, uma delas é selecionada arbitrariamente e chamada de chave primária daquele reção.
Um requisito comum é para elementos de uma relação com a qualquer ordem entre esses domínios.

