# MySQL

Oinarrizko komandoak MySQLn:

CREATE DATABASE Adibidea; --> adibidea izeneko datu basea sortu dugu
SHOW DATABASES; --> dauden datu baseak ikusteko
USE Adibidea; --> adibidea datu basea erabiliko dela adierazi

CREATE TABLE Jokalariak(izena varchar(20),abizena varchar(20) adina int, nan varchar(10)); --> jokalariak taula sortuta daturik gabe
SHOW TABLES; --> taulen informazioa ikusi 

INSERT INTO Jokalariak VALUES ('Iker', 'Martinez-Ayo', 22, 12345678A); --> pertsona baten datuak sartu
INSERT INTO Jokalariak VALUES ('Cristiano', 'Ronaldo', 34, 12345679B); --> pertsona baten datuak sartu
INSERT INTO Jokalariak VALUES ('Gabriel', 'Barbosa', 30, 12345688K); --> pertsona baten datuak sartu

SELECT * FROM Jokalariak; --> Jokalari guztiak ikusi
SELECT COUNT(*) FROM Jokalariak; --> jokalari kopurua ikusi
SELECT * FROM Jokalariak WHERE izena = 'Iker';

UPDATE Jokalariak SET adina=35 WHERE (izena='Cristiano' & abizena='Ronaldo');

