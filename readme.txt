Comdandi git

//init crea la repository nella cartella in cui è invocata
git init
//clona una reppsitory gia esistente
git clone <repository remota> o <locale>
//Aggiunge un file al repository locale (permettendone la condivisione)
git add <file o insieme di file da aggiungere>
//Committa i cambiamenti apportati alla copia locale (e aggiunti nella cosiddetta area di staging)
git commit -m <messaggio>
//Committa con -a ( aggiunge senza fare l'add) -m(immetti subito il messaggio)
git commit -a -m <messaggio>
//Aggiorna i branch locali con le eventuali modifiche presenti sul repository remoto
git pull
//Carica i cambiamenti locali committati sul repository remoto.
//se qualcun altro ha apportato delle modifiche al repository remoto dopo il nostro ultimo aggiornamento (pull), allora, prima
//di poter effettuare il caricamento (push) siamo costretti a effettuare un ulteriore pull il quale unir`a le modifiche locali con
git push
// Permette di fondere due branch 
git merge <branch>
// Permette di spostarci su un altro branch o ad uno specifico commit. Pu`o anche essere utilizzato per creare un nuovo branch e
//spostarci con l’opzione -b.
git checkout -b <newBranch> //Si sposta creando un nuovo branch
git checkout <nomeBranch> // si sposta sul branch desiderato
//Tramite opportune opzioni pu`o essere utilizzato per sapere quali sono i branch, aggiungerne di nuovi o cancellarne qualcuno
git branch <nomeBranch> //add
git branch -d <nomeBranch> //remove
//Ci informa sullo stato del repository locale: quali file abbiamo aggiunto, modificato, quali commit sono stati effettuati, su quale
//branch ci troviamo...
git status
// ci da il resoconto di tutte le modifiche fatte a tutti i file
git log
//Permette di vedere tutte le modifche sono state fatte su quel file
git diff <nomefile>
// compara i file aggiunti con HEAD; altrimenti compara i file non ancora aggiunti.
git diff --cached
