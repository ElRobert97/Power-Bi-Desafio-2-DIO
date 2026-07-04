# Power-Bi-Desafio-2-DIO-
Aqui foquei em fazer as coisas dentro do power bi não utilizei SQL para fazer as mesclagem. 

Notas do Desafio 2 do Formação Power BI Analyst focado em ETL da Azure
Azure configurado, criado o banco de dados e integrado ao power bi

IMPORTANTE: Elimine as colunas desnecessárias, que não serão usadas no relatório de cada tabela

- Limpar a base de dados e verificar a existência de nulos
- Employee sem Super_ssn podem ser o gerente, verificar se existe algum colaborador assim
- Verificar se há algum departamento sem gerente e caso tenha preencher as lacunas com dados fictícios
- Verificar o número de horas dos projetos
- Separar colunas complexas

- Eliminar as colunas desnecessárias no processo

- Fazer a junção dos colaboradores e respectivos nomes dos gerentes

- Mesclar as colunas de nome e sobrenome para ter apenas uma coluna definindo os nomes dos colaboradores

- Mesclar consultas employee e departamento para criar uma tabela employee com o nome dos departamentos associados aos colaboradores. A mescla terá como base a tabela employee

- Mesclar os nomes de departamentos e localização, explicar por que, neste caso podemos apenas utilizar o mesclar e não o atribuir.
R: Quando mesclamos a consulta nós conseguimos selecionar o modo como queremos realizar a junção dos dados de acordo com a nossa necessidade, mas ao atribuirmos/acrescentarmos uma consulta, ele junta as duas tabelas de modo geral semelhante a um crossjoin trazendo vários valores nulos no processo ao tentar unir as tabelas, sendo assim para esse caso é melhor mesclar pela previsibilidade e por conseguirmos organizar as informações melhor
Super_ssn preenchido com o ssn 888665555 para fins de todos os colaboradores terem um Super

OK - Agrupar os dados a fim de saber quantos colaboradores existem por gerente

Formato o nome das tabelas para ficar mais amigável e o nome das consultas para ficar coerente com o contexto, como a importação da Azure trás os nomes das tabelas e das consultas junto ao nome do DB achei importante fazer ela limpeza para organizar os dados.
