Modellizzare la struttura di un database per memorizzare tutti i dati riguardanti una università:
sono presenti diversi `Dipartimenti` (es.: Lettere e Filosofia, Matematica, Ingegneria ecc.);

ogni Dipartimento offre più `Corsi di Laurea` (es.: Civiltà e Letterature Classiche, Informatica, Ingegneria Elettronica ecc..)

ogni Corso di Laurea prevede diversi `Corsi` (es.: Letteratura Latina, Sistemi Operativi 1, Analisi Matematica 2 ecc.);
ogni Corso può essere tenuto da diversi `Insegnanti`;
ogni Corso prevede più `appelli d'Esame`;
ogni `Studente` è iscritto ad un solo Corso di Laurea;
ogni Studente può iscriversi a più appelli di Esame;
per ogni appello d'Esame a cui lo Studente ha partecipato, è necessario memorizzare il voto ottenuto, anche se non sufficiente. Pensiamo a quali entità (tabelle) creare per il nostro database e cerchiamo poi di stabilirne le relazioni. Infine, andiamo a definire le colonne e i tipi di dato di ogni tabella.

# Entità

- Dipartimenti ✔️
- Corsi di Laurea ✔️
- corsi ✔️
- Insegnanti ✔️
- appelli d'Esame
- Studente ✔️

# Tables

# departments

- id
- Humanities
- law
- math

## courses (corsi di laurea)

- id
- old literature
- languages
- computer_science

## classes (corsi)

- id
- literature
- operating_systems_1
- civil_law

## students

- id | sarà usata come matricola
- name
- lastname
- age

## Profs

- id | sarà usata come matricola
- name
- lastname
- matter

## exams

- id
- date
- year
- prof
- matter
