

Modellizzare la struttura di un database per memorizzare tutti i dati riguardanti una università:
sono presenti diversi Dipartimenti (es.: Lettere e Filosofia, Matematica, Ingegneria ecc.);
ogni Dipartimento offre più Corsi di Laurea (es.: Civiltà e Letterature Classiche, Informatica, Ingegneria Elettronica ecc..)
ogni Corso di Laurea prevede diversi Corsi (es.: Letteratura Latina, Sistemi Operativi 1, Analisi Matematica 2 ecc.);
ogni Corso può essere tenuto da diversi Insegnanti;
ogni Corso prevede più appelli d'Esame;
ogni Studente è iscritto ad un solo Corso di Laurea;
ogni Studente può iscriversi a più appelli di Esame;
per ogni appello d'Esame a cui lo Studente ha partecipato, è necessario memorizzare il voto ottenuto, anche se non sufficiente. Pensiamo a quali entità (tabelle) creare per il nostro database e cerchiamo poi di stabilirne le relazioni. Infine, andiamo a definire le colonne e i tipi di dato di ogni tabella.
Utilizzare https://www.drawio.com/ per la creazione dello schema.
Esportare quindi il diagramma in png, caricarlo nella repo in un file index.html  nel quale inserite l'immagine come visto in classe.


# Table name: *dipartimenti*
- id
- nome_dipartimento


# Table name: *corsi_di_laurea*
- id
- id_dipartimento
- nome_laurea

# Table name: *corsi*
- id
- id_corso_di_laurea
- nome_corso

# Table name: *insegnanti*
- id
- nome_insegnante
- cognome_insegnante

# Table name: *appelli*
- id
- id_corso
- numero_appelli


# Table name: *studente*
- id
- id_appello
- nome_studente
- cognome_studente

# Table name: *risultati*
- id
- id_appello
- voto_studente

