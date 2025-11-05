# Notas do Capítulo 1 
  
> Uma base de dados é nada mais do que uma coleção de dados relacionados.  
  
## Sistemas de Base de Dados não Relacionais  
  
Inicialmente, os dados eram armazenados e representados aos usuários em diferentes maneiras:  
- Sistema de Base de Dados Hierárquico;
- Sistema de Base de Dados de Rede.
  
## O Modelo Relacional  
  
Esse modelo propõe a representação de dados como um conjunto de tabelas conectadas por dados redundantes.  
  
Em uma tabela relacional está inclusa uma informação que unicamente identifica uma linha (row) na tabela. Essa informação é chamada de **chave primária**.  
  
> A chave primária pode ser nomeada de chave composta se consistir em duas ou mais colunas. Por exemplo, uma tabela com uma coluna para nome e outra coluna para sobrenome. Se a chave primária é composta por dados cujo contéudo é independente da realidade de máquina, como nomes de pessoas, temos então uma **chave natural**. POrém, considerando que podemos ter duas ou mais pessoas com os mesmos nomes e sobrenomes e adicionarmos uma coluna para alocar IDs aleatórios, temos então uma **chave substituta**.  
  
> Ainda considerando a chave substituta, a exemplo, e tomarmos uma outra tabela que aloca os dados de compras dos clientes, a presença da chave substituta nessa outra tabela visa conectar a tabela de compras com a tabela de cleintes, de modo a indentificar a qual cliente pertence cada compra. Nesse cenário, a chave substituta, quando parte da tabela conectada, é chamada de **chave estrangeira**.  
  
Uma das vantagens do modelo relacional é a possibilidade de, na necessidade de alteração de dados, ser possível alterar o dado somente um local. Assim, em uma base de dados de 50 tabelas, se eu precisar alterar o dado do meu cliente, vou fazê-lo somente na tabela de clientes, de forma que a chave estrangeira permanecerá a mesma nas demais tabelas.  
  
> O processo de refinar a base de dados para assegurar que cada tipo e conteúdo de dado está no local correto é chamado de **normalização**.
  
## Termos e Definições  
  
* Entidade: algo do interesse para a comunidade de usuários da base de dados. Por exemplo, clientes, localizações, etc.  
* Coluna: um pedaço individual de dados armazenados em uma tabela.  
* Linha: um conjunto de colunas que juntos descrevem completamente uma entidade ou alguma ação da entidade. Também é chamada de gravação.  
* Tabela: uma coleção de linhas, mantida na memória (não persistente) ou armazenada permanentemente (persistente).  
* Result set: outro nome para uma tabela não persistente, geralmente resultado de uma consulta SQL.  
  
## O que é SQL?  
  
SQL, pronunciando __sequel__, é uma linguagem para manipular dadsos em bancos de dados relacionais.  
  
## Classes de Instruções SQL  
  
* Instruções de esquema SQL: usados para definir as estruturas de dados armazenados na base de dados;  
* Instruções de dados SQL: usados para manipular estruturas de dados previamente definidas pelas instruções de esquema SQL;  
* Instruções de transação SQL: usados para começar, terminar e reverter transações.  
  
## SQL: uma linguagem não-procedural  
  
Uma linguagem não-procedural define os resultados desejados, mas não os procesos pelos os quais os resultados foram  gerados, que são deixados fora do alcance do agente externo.  
  
