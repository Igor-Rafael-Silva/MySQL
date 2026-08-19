# MySQL
Alguns códigos aprendidos de MySQL


# Banco de Dados - Escola

## Comandos utilizados

### 1. Entrar no MySQL

```sql
mysql -u root
```

Entra no MySQL usando o usuário `root`.

### 2. Criar o banco

```sql
CREATE DATABASE escola_db;
```

Cria o banco de dados chamado `escola_db`.

### 3. Mostrar os bancos

```sql
SHOW DATABASES;
```

Mostra todos os bancos de dados existentes.

### 4. Selecionar o banco

```sql
USE escola_db;
```

Seleciona o banco `escola_db` para trabalhar nele.

### 5. Criar a tabela

```sql
CREATE TABLE aluno (
    matricula INT,
    nome VARCHAR(50),
    cpf VARCHAR(11)
);
```

Cria a tabela `aluno` com matrícula, nome e CPF.

### 6. Mostrar as tabelas

```sql
SHOW TABLES;
```

Mostra as tabelas existentes no banco selecionado.

### 7. Ver a estrutura da tabela

```sql
DESCRIBE aluno;
```

Mostra as colunas, tipos de dados e outras informações da tabela.

### 8. Inserir um aluno

```sql
INSERT INTO aluno
(matricula, nome, cpf)
VALUES
(1, 'Valdir Pouca Telha', '12345678970');
```

Adiciona um aluno na tabela.

### 9. Consultar os alunos

```sql
SELECT * FROM aluno;
```

Mostra todos os dados cadastrados na tabela.


