# ConsultasSQL

Usuário | ... |
:--------- | :------: | 
INSERT INTO usuario (nome, email, senha) VALUES ('Gamon Gabriel', 'jsboy@gamon.com', '4545'); | Se Cadastrar |
SELECT * FROM usuario WHERE (email='jsboy@gamon.com' and senha = '4545'); | Login | 
(SELECT COUNT(*) FROM usuario WHERE email = 'jsboy@gamon.com' > 0); | Verificar Email | 
UPDATE usuario SET senha = "1304" WHERE cd=1; | Trocar Senha |

<br>

Categoria | ... |
:--------- | :------: | 
SELECT * FROM categoria; | Listar Categorias |

<br>

Jogo | ... |
:--------- | :------: | 
INSERT INTO jogo (nome, id_usuario, id_categoria) VALUES("gamongame", 1, 2); | Cadastrar Jogo |
SELECT * FROM jogo WHERE id_usuario = 1; | Listar Jogo do Usuário |
SELECT * FROM jogo WHERE id_categoria = 2; | Listar Jogo da Categoria |
UPDATE jogo SET nome = "Jogo do Gamon" WHERE cd=1; | Editar Jogo |
