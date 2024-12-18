### 1. Selezionare tutti gli studenti nati nel 1990 (160)

```SQL
SELECT * 
FROM `students`
WHERE `date_of_birth` LIKE '1990%';
```

### 2. Selezionare tutti i corsi che valgono più di 10 crediti (479)

```SQL
SELECT * 
FROM `courses`
where `cfu` > 10
```

### 3. Selezionare tutti gli studenti che hanno più di 30 anni

```SQL
SELECT *
FROM students
WHERE `date_of_birth` < CURDATE() - INTERVAL 30 YEAR;
```


### 4. Selezionare tutti i corsi del primo semestre del primo anno di un qualsiasi corso di laurea (286)

```SQL
select *
from `courses`
where `period` = 'I semestre' and `year` = 1
```

### 5. Selezionare tutti gli appelli d'esame che avvengono nel pomeriggio (dopo le 14) del 20/06/2020 (21)

```SQL
select *
from `exams`
where hour(`hour`) >= '14:00' and `date` ="2020-06-20"
```

 
### 6  Selezionare tutti i corsi di laurea magistrale (38)
```SQL
select *
from `degrees`
where `level` = 'magistrale'
```


### 7 Da quanti dipartimenti è composta l'università? (12)
```SQL
select *
from `departments`

```



### 8 Quanti sono gli insegnanti che non hanno un numero di telefono? (50)
```SQL
select *
from `teachers`
where `phone` is null

```



### 9 Inserire nella tabella degli studenti un nuovo record con i propri dati (per il campo degree_id, inserire un valore casuale)

```SQL
INSERT INTO `students`(degree_id, name, surname, date_of_birth, fiscal_code, enrolment_date, registration_number, email)
VALUES (18, 'Damiano', 'Mariscoli', '1972-08-31' , 'DADSADASDASD1231', '2019-04-16', 672344, 'daibnib@gmail.com' );
```



### 10. Cambiare il numero dell’ufficio del professor Pietro Rizzo in 126

```SQL
update `teachers`
set `office_number` = 126
where `name` ='Pietro' and `surname` = 'Rizzo'
```


### 11 Eliminare dalla tabella studenti il record creato precedentemente al punto 9

```SQL
-- SELECT id from students
-- where name = 'damiano' and surname = 'mariscoli' 

delete from `students`
where `name` = 'Damiano' and `surname` = 'Mariscoli'
```




