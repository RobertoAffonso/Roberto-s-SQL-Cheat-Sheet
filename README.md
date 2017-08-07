# Roberto-s-SQL-Cheat-Sheet
This is a cheat sheet that i wrote in order to help me with SQL Commands, nothing really special about it
*************************************************************************************************************
*                                                                                                           *
*                                                   Roberto's SQL Cheat Sheet                               *
*************************************************************************************************************
/* ORDEM DE CRIAÇÃO DE BANCO DE DADOS*/

1 -> Modelo Conceitual

2 -> Modelo Lógico

3 -> Modelo Físico

/*ALGUNS TIPOS DE ATRIBUTOS*/

CHAR -> 1 BYTE
	Sempre utilizar quando não for necessário
	variar um dado, pois ele possui uma maior
	velocidade.

	EXEMPLO: DF, MG, RAM, M, F.....

VARCHAR -> 1 BYTE(VARIAVEL)
	Utilizar quando for inserir dados de tamanho
	variável no número de caracteres

	EXEMPLO: JOAO, MARIA, MADEIRA, COMPUTADOR, JOGO......

ENUM ->
	Utilizar quando for necessário enumerar vários
	dados, ele serve como se fosse uma combobox.

INT ->
	Utilizar quando for necessário armazenar
	números inteiros, ele possui um máximo de
	11 dígitos.

FLOAT ->
	Utilizar quando for necessário armazenar
	números reais.

	FLOAT(10,3)
		10 = total de números
		3 = posição da vírgula

	EXEMPLO: 10,3 3,141519

/* CRIAR BANCO DE DADOS */

CREATE DATABASE db_projeto;

/* UTILIZAR O BANCO */

USE db_projeto;

/* CRIAR TABELA */

CREATE TABLE tb_cliente
(
	nme_nome VARCHAR(30),
	nme_genero CHAR(1),
	nme_email VARCHAR(30),
	num_cpf INT(11),
	num_telefone VARCHAR(30),
	nme_endereco VARCHAR(100)
);

/* VERIFICAR AS TABELAS */

SHOW TABLES;

/*DESCREVER TABELAS*/

DESC tb_cliente;

/*INSERIR DADOS*/

INSERT INTO tb_cliente VALUES(x,x,x,x,x);

