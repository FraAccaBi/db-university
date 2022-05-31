# DB University

## Universities

id:             PK NOTNULL UNIQUE INDEX AUTOINCREMENTAL
subject:
course_name:
durata:
student_nr:
?teachers?:
?student?:
?employes?:
?classes?:
?laboratories?:

## Teachers

id:             PK NOTNULL UNIQUE INDEX AUTOINCREMENTAL
name:
lastname:
age:
telephone:
adress:
pay:
hiring_date:
children:
chidren_nr:
special_condition:
full/part_time:
contract_type:

## Students

id/matricola:   PK NOTNULL UNIQUE INDEX AUTOINCREMENTAL
name:
lastname:
age:
telephone:
adress:
iscription_year:
due_graduation:
graduated:

## Tuition Fees

id:             PK NOTNULL UNIQUE INDEX AUTOINCREMENTAL
name:
range:

## Tuition Support Entity

id:             PK NOTNULL UNIQUE INDEX AUTOINCREMENTAL
name: 
?student?:
student_nr:


## Faculties

id:             PK NOTNULL UNIQUE INDEX AUTOINCREMENTAL
name:
?university?:

## Employes

id:             PK NOTNULL UNIQUE INDEX AUTOINCREMENTAL
name:
lastname:
age:
telephone:
adress:
pay:
hiring_date:
contract_type:
children:
chidren_nr:
special_condition:
full/part_time:

## Classes (Location)

id:             PK NOTNULL UNIQUE INDEX AUTOINCREMENTAL
name:
?building?:

## Laboratories

id:             PK NOTNULL UNIQUE INDEX AUTOINCREMENTAL
name:
?building?:

## Buildings

id:             PK NOTNULL UNIQUE INDEX AUTOINCREMENTAL
name:
adress:

## Exams

id:             PK NOTNULL UNIQUE INDEX AUTOINCREMENTAL
date:
subject:
?biundings?:
?class?

## Results

id:             PK NOTNULL UNIQUE INDEX AUTOINCREMENTAL
?student?
mark:
pass:
