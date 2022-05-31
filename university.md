# DB University

## Faculties

id:             PK NOTNULL UNIQUE INDEX AUTOINCREMENTAL 
name:           VARCHAR(50) NOTNULL INDEX
student_nr:     MEDIUMINT NULL

## Degree_courses

id:             PK NOTNULL UNIQUE INDEX AUTOINCREMENTAL
name:           VARCHAR(50) NOTNULL INDEX
subject:        VARCHAR(60 NOTNULL)
student_nr:     MEDIUMINT NULL     


## Courses

id:             PK NOTNULL UNIQUE INDEX AUTOINCREMENTAL
name:           VARCHAR(60) NOTNULL INDEX
subject:        VARCHAR(60 NOTNULL)
CFU:            TINYINT NULL DEFAULT(120)
length:         TINYINT NULL DEFAULT(2)


## Teachers

id:                     PK NOTNULL UNIQUE INDEX AUTOINCREMENTAL
name:                   VARCHAR(50) NOTNULL
lastname:               VARCHAR(50) NOTNULL
birth_date:             DATE NULL      
telephone:              VARCHAR(15) NULL
adress:                 VARCHAR(50) NOTNULL
subject:                VARCHAR(60) NOTNULL

## Students

id/matricola:       PK NOTNULL UNIQUE INDEX AUTOINCREMENTAL
name:               VARCHAR(50) NOTNULL
lastname:           VARCHAR(50) NOTNULL
birth_date:         DATE NULL      
telephone:          VARCHAR(15) NULL
adress:             VARCHAR(50) NOTNULL
registration_year:    YEAR NULL
due_graduation:     YEAR NULL
graduated:          CHAR(1)

## Exams

id:                 PK NOTNULL UNIQUE INDEX AUTOINCREMENTAL
date:               DATETIME NOTNULL
subject:            VARCHAR(60 NOTNULL)
enrolled_students:  SMALLINT NULL






