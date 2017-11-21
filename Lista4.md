# BancoII
Vê

CREATE TABLE DADOS_MULTIMIDIA(
CODIGO INT PRIMARY KEY,
NOME VARCHAR(30),
TIPO VARCHAR(20),
DADOS LONGBLOB
);

SELECT*FROM DADOS_MULTIMIDIA;


INSERT INTO DADOS_MULTIMIDiA(codigo,nome,tipo,dados) VALUES(1,'Imagem','oid',load_file("C:\\Users\\100296el\\Downloads\\Deserto.jpg"));
INSERT INTO DADOS_MULTIMIDiA(codigo,nome,tipo,dados) VALUES(2,'Imagem','OID',load_file("C:\\Users\\100296el\\Downloads\\oi.jpeg"));
INSERT INTO DADOS_MULTIMIDiA(codigo,nome,tipo,dados) VALUES(3,'Imagem','OID',load_file("C:\\Users\\100296el\\Downloads\\doid.jpeg"));

SELECT*FROM DADOS_MULTIMIDIA;

select dados into dumpfile'C:\\Users\\100296el\\Pictures\\06-04-2014\\oi.jpeg' from dados_multimidia where codigo = 1;
select dados into dumpfile'C:\\Users\\100296el\\Pictures\\06-04-2014\\oii.jpeg' from dados_multimidia where codigo = 2;
select dados into dumpfile'C:\\Users\\100296el\\Pictures\\06-04-2014\\oiii.jpeg' from dados_multimidia where codigo = 3;





