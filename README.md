# mySql

mySql comandos via cmd

cd C:\Program Files\MySQL\MySQL Server 8.0\bin

mysql -u root -p

show databases;

create database portal_noticias;

use portal_noticias;

show tables;
 
create table noticias(
	id_noticias int not null primary key auto_increment,
	titulo varchar(100),
	noticia text,
	data_criacao timestamp default current_timestamp
);

select * from noticias;

insert into noticias(titulo, noticia) 
value('titulo da noticia','conteudo da noticia');
