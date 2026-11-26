# DOCUMENTAZIONE progettoFloresNavarroRobertoClasse


il programma deve gestire una Classe alla quale vengono aggregati N Studenti, ogni classe ha i propri attributi e metodi, la Classe deve saper calcolare la media totale di tutti gli studenti che ne fanno parte, deve saper
riferire le medie insufficienti, deve saper estrarre un alunno per un eventuale verifica orale, e deve saper caricare tutti gli studenti che ne fanno parte, mentre la classe Studente deve saper aggiungere un nuovo voto e 
calcolare la media del singolo alunno.

============================================================================
### classe Studente:
============================================================================

attributi:
-----------------------------------------------------------
-nome: String| serve per inserire il dato del nome dello studente

-cognome: String| serve per inserire il cognome dello studente

-numMaterie: int| serve per indicare il numero totale delle materie 

-votiFinali: int[]| array che serve per aggiungere tutti i voti finali dell'alunno

-matricola: int| il numero della matricola dell'alunno

metodi:
-----------------------------------------------------------
+Studente(String,String,int,int)| serve per istanziare l'oggetto Studente

+gNome():String| metodo get serve per leggere e ottenere il valore dell'attributo privato nome

+sNome(String):void| metodo set serve per modificare l'attributo privato nome

+toString():String| metodo toString serve per indicare una descrizione e tutti i voti finali dello studente

+caricaVoto(int):boolean| metodo per caricare un nuovo voto

+calcolaMedia():double| metodo per calcolare la media totale dell'alunno


============================================================================
### classe Classe:
============================================================================

attributi:
-----------------------------------------------------------

-anno: int| serve per inserire l'anno dove si trovano attualmente gli studenti (1,2,3,4 o 5)

-sezione: String| serve per inserire la sezione attuale della classe

-indirizzo: String| serve per indicare l'indirizzo scolastico preso dagli studenti

-studenti: Studente[]| array che serve per aggiungere tutti gli studenti di una Classe

-numStudenti: int| il numero degli studenti totali che fanno parte della Classe


metodi:
-----------------------------------------------------------

+Classe(int,String,String,int)| serve per istanziare l'oggetto Classe

+gAnno():int| metodo get serve per leggere e ottenere il valore dell'attributo privato Anno

+sAnno(int):void| metodo set serve per modificare l'attributo privato anno

+toString():String| metodo toString serve per indicare e mostrare tutte le medie degli alunni sia sufficienti che insufficienti

+mediaClasse():double| metodo per calcolare la media totale di tutta la classe

+mediaInsufficienti():int| metodo che serve per capire quante medie insufficienti ci sono all'interno della Classe

+estraiStudenti(int):Studente[]| metodo che serve per estrarre uno studente casuale per un eventuale interrogazione

+caricaStudente(Studente):boolean| metodo in grado di caricare un nuovo studente



============================================================================

COLLEGAMENTI FATTI CON UML:
ho usato una relazione di aggregazione(queesto legame indica una relazione meno forte) se l'oggetto Classe viene eliminato l'oggetto Studente e' 
indipendente e non subisce cambiamenti inoltre l'oggetto "Studente" viene creato prima della Classe inoltre uno Studente ha solo una Classe, 
mentre la Classe può avere piu studenti quindi un array di studenti.




