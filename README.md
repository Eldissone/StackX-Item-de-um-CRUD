# StackX-Item-de-um-CRUD

CREATE TABLE Post
(
	id_post int PRIMARY KEY NOT NULL,
  id_user int NOT NULL,
	post varchar(355) NOT NULL,
	data_post datetime NOT NULL,
	
);
ALTER TABLE post
	ADD CONSTRAINT fk_post FOREIGN KEY (id_user_post) REFERENCES Alunos(id_user);

# CRUD
1- CREATE
INSERT INTO Post (id_post, id_user, post, data_pos ) 
VALUES (1, 10, 'Olá mundo esse é meu primeiro post', '2024-11-20 11:20:00'), </br>
       (2, 1, 'Olá mundo esse é meu primeiro post 2', '2024-11-21 18:20:00'),
       (3, 3, 'Olá mundo esse é meu primeiro post 3', '2024-11-21 20:30:00');

2- READ
SELECT * FROM Post;

3- Update
UPDATE Post SET id_user = 12, post = 'Olá mundo esse é meu post atualizado', WHERE id_post = 2;

4- DELETE
DELETE FROM Post WHERE id_post = 2;
