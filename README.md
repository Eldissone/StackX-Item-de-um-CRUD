# StackX-Item-de-um-CRUD

CREATE TABLE Post <br>
( <br>
	id_post int PRIMARY KEY NOT NULL, <br>
        id_user int NOT NULL, <br>
	post varchar(355) NOT NULL, <br>
	data_post datetime NOT NULL, <br>
	
); <br>
ALTER TABLE post <br>
	ADD CONSTRAINT fk_post FOREIGN KEY (id_user_post) REFERENCES Alunos(id_user); <br>

# CRUD
1- CREATE <br>
INSERT INTO Post (id_post, id_user, post, data_pos )  <br>
VALUES (1, 10, 'Olá mundo esse é meu primeiro post', '2024-11-20 11:20:00'), <br>
       (2, 1, 'Olá mundo esse é meu primeiro post 2', '2024-11-21 18:20:00'), <br>
       (3, 3, 'Olá mundo esse é meu primeiro post 3', '2024-11-21 20:30:00'); <br>

2- READ <br>
SELECT * FROM Post; <br>

3- Update <br>
UPDATE Post SET id_user = 12, post = 'Olá mundo esse é meu post atualizado', WHERE id_post = 2; <br>

4- DELETE <br>
DELETE FROM Post WHERE id_post = 2; <br>
