# ATV_04_SINTAXE_SQL

### Código SQL:
```sql
-- Criar a tabela 'musicasFavoritas'
CREATE TABLE musicasFavoritas (
    id INT PRIMARY KEY AUTO_INCREMENT,
    musica VARCHAR(50),
    artista VARCHAR(50),
    idioma VARCHAR(50),
    duracaoMin TIME
);

-- Inserir dados na tabela 'musicasFavoritas'
INSERT INTO musicasFavoritas (musica, artista, idioma, duracaoMin) VALUES
    ('Summertime Sadness', 'Lana del Rey', 'EN', '00:04:25'),
    ('Poker Face', 'Lady Gaga', 'EN', '00:03:32'),
    ('Habits of My Heart', 'Jaymes Young', 'EN', '00:03:30'),
    ('Habits (Stay High)', 'Tove Lo', 'EN', '00:03:24'),
    ('Pontos de Exclamação', 'Jovem Dionisio', 'PT-BR', '00:03:01'),
    ('Games', 'Tessa Violet', 'Inglês', '00:03:29'),
    ('Nada Contra (ciúme)', 'Clarissa', 'PT-BR', '00:02:21'),
    ('Save Your Tears', 'The Weeknd', 'EN', '00:03:36'),
    ('Imaturo', 'Jão', 'PT-BR', '00:03:00'),
    ('Algum Ritmo', 'Jovem Dionisio', 'PT-BR', '00:03:35'),
    ('Lapada Dela', 'Grupo Menos é Mais', 'PT-BR', '00:02:39'),
    ('The Real Folk Blues', 'Mig Music', 'PT-BR', '00:06:11'),
    ('Deja vu', 'Olivia Rodrigo', 'Inglês', '00:03:35'),
    ('Amiga da Minha Mulher', 'Seu Jorge', 'PT-BR', '00:04:08'),
    ('Jovem', 'Julio Secchin', 'PT-BR', '00:02:48'),
    ('O Amor do Mundo Inteiro', 'Chapéu de Palha', 'PT-BR', '00:02:59'),
    ('Bem', 'Chapéu de Palha', 'PT-BR', '00:04:30'),
    ('Oitavo Andar', 'Clarice Falcão', 'PT-BR', '00:02:15'),
    ('Onde Anda Você', 'Tiago Nacarato', 'PT-BR', '00:02:51'),
    ('João e Maria', 'Chico Buarque', 'PT-BR', '00:03:00'),
    ('Quando Bate Aquela Saudade', 'Rubel', 'PT-BR', '00:06:35');
    
-- Mostrar os dados inseridos
SELECT * FROM musicasFavoritas;
```

### Para listar as músicas em ordem alfabética, executamos o código:
```sql
-- Ordem crescente
SELECT * 
FROM musicasFavoritas 
ORDER BY musica;

-- Ordem decrescente
SELECT * 
FROM musicasFavoritas 
ORDER BY musica DESC;
```

### Para listar as músicas de acordo com a duração, executamos o código:
```sql
-- Ordem crescente
SELECT * 
FROM musicasFavoritas 
ORDER BY duracaomin;

-- Ordem decrescente
SELECT * 
FROM musicasFavoritas 
ORDER BY duracaomin DESC;
```
