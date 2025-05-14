#### Desafio Azure criação de banco de dados

## Objetivo 

Mostrar aprendizado sobre o que foi aprendido na aula.

#Tutorial 

1. Entre na sua conta Azure.

2.  Clique em adicionar recurso > SQL Database

3.  Definir nome do servidor, servidor, localidade e performance .

4.  Criar um servidor SQL com nome e senha.

5.  Configurar o firewall para permitir conexões externas.

6.  Conectar via SQL Server Management Studio ou Azure Data Studio.

7.  Realizar conexões de testes e criação de tabelas.


##### TESTANDO BANCO DE DADOS

1. Acesse via sqlcmd o banco de dados com: sqlcmd -S nomedoservidor.database.windows.net -U nomedousuario@nomedoservidor -P 'senha' -d nomedobancodedados

2. Crie uma tabela: 

CREATE TABLE Clientes (
    ID INT PRIMARY KEY IDENTITY(1,1),
    Nome NVARCHAR(100) NOT NULL,
    Email NVARCHAR(100) NOT NULL,
    DataCadastro DATETIME DEFAULT GETDATE()
);
GO

3. Teste a tabela com: SELECT * FROM Clientes depois digite GO

4. Pronto, banco de dados funcionando ! =)
