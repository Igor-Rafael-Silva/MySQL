# MySQL - Comandos Básicos

##  Criar banco de dados

```sql
CREATE DATABASE escola;
```

Cria um novo banco de dados.

```sql
USE escola;
```

Seleciona o banco que será utilizado.

## Criar tabela

```sql
CREATE TABLE alunos (
    id INT PRIMARY KEY AUTO_INCREMENT,
    nome VARCHAR(100),
    curso VARCHAR(50)
);
```

Cria a tabela `alunos`.

* `INT` → número inteiro.
* `PRIMARY KEY` → identifica cada registro.
* `AUTO_INCREMENT` → gera o ID automaticamente.
* `VARCHAR` → armazena textos.

##  Inserir dados

```sql
INSERT INTO alunos (nome, curso)
VALUES ('Ana Souza', 'ADS');
```

Adiciona um novo aluno na tabela.

## Consultar dados

```sql
SELECT * FROM alunos;
```

Mostra todas as colunas e registros da tabela.

Também podemos filtrar:

```sql
SELECT nome FROM alunos
WHERE curso = 'ADS';
```

Mostra apenas o nome dos alunos que fazem ADS.

## Atualizar dados

```sql
UPDATE alunos
SET curso = 'Redes'
WHERE nome = 'Ana Souza';
```

Altera o curso da Ana.


## Excluir dados

```sql
DELETE FROM alunos
WHERE nome = 'Carla Reis';
```

Remove o registro da Carla.


## Resumo

| Comando         | Função             |
| --------------- | ------------------ |
| CREATE DATABASE | Cria um banco      |
| USE             | Seleciona um banco |
| CREATE TABLE    | Cria uma tabela    |
| INSERT          | Adiciona dados     |
| SELECT          | Consulta dados     |
| UPDATE          | Atualiza dados     |
| DELETE          | Remove dados       |




