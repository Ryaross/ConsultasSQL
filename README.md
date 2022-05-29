# ConsultasSQL

Usuário | ... |
:--------- | :------: | 
INSERT INTO usuario (nome, email, senha) VALUES ('Gamon Gabriel', 'jsboy@gamon.com', '4545'); | Se Cadastrar |
SELECT * FROM usuario WHERE (email='jsboy@gamon.com' and senha = '4545'); | Login | 
(SELECT COUNT(*) FROM usuario WHERE email = 'jsboy@gamon.com' > 0); | Verificar Email | 
UPDATE usuario SET senha = "1304" WHERE cd=1; | Trocar Senha |
DELETE FROM usuario WHERE cd=1; | Excluir Conta |

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

<br>

Pergunta | ... |
:--------- | :------: | 
INSERT INTO jogo (nome, id_usuario, id_categoria) VALUES("gamongame", 1, 2); | Cadastrar Perguntar |
SELECT * FROM jogo WHERE id_usuario = 1; | Listar Perguntas do Jogo |
SELECT * FROM jogo WHERE id_categoria = 2; | Listar Jogo da Categoria |
UPDATE jogo SET nome = "Jogo do Gamon" WHERE cd=1; | Editar Pergunta |
DELETE FROM pergunta WHERE cd=1; | Excluir Pergunta |

<br>

Alternativa | ... |
:--------- | :------: | 
INSERT INTO alternativa (texto, resposta, id_pergunta) VALUES("Não", false, 1); | Cadastrar Alternativa |
INSERT INTO alternativa (texto, resposta, id_pergunta) VALUES("Claro", true, 1); | Cadastrar Alternativa |
SELECT * FROM alternativa WHERE id_pergunta = 1; | Listar Alternativas da Pergunta |
UPDATE alternativa SET texto = "Nunca" WHERE cd=1; | Editar Alternativa |
DELETE FROM alternativa WHERE cd=1; | Excluir Alternativa |

<br>

Pontos | ... |
:--------- | :------: | 
INSERT INTO ponto (id_usuario, id_jogo, total) VALUES (x,x, 10); | Cadastrar Pontos |
SELECT id_usuario FROM ponto WHERE total>0; | Listar Usuários que Jogaram um Jogo |
SELECT id_usuario FROM ponto WHERE Max(total);  | Listar Usuário com mais Pontos |
(SELECT COUNT(*) FROM ponto WHERE total>0);  | Listar Jogadores que já Jogaram |

<hr> 

<div align="center">Feito por <a href="https://github.com/devgamon" target="_blank">Gabriel Gamon</a> &#129398;</div>
	
