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

### 3.

```SQL
select *
from students
where year(`date_of_birth`) <  '1994'
```


### 4.
```SQL
select *
from `courses`
where `period` = 'I semestre' and `year` = 1
```

### 5.
```SQL
select *
from `exams`
where hour(`hour`) >= '14:00' and `date` ="2020-06-20"
```


### 6
```SQL
select *
from `degrees`
where `level` = 'magistrale'
```


### 7
```SQL
select *
from `departments`

```




```SQL
SELECT * 
FROM `courses`
where `cfu` > 10
```





```SQL
SELECT * 
FROM `courses`
where `cfu` > 10
```





```SQL
SELECT * 
FROM `courses`
where `cfu` > 10
```



```SQL
SELECT * 
FROM `courses`
where `cfu` > 10
```



```SQL
SELECT * 
FROM `courses`
where `cfu` > 10
```
