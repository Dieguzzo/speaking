# Speaking, allenamento IELTS

Una piccola web app per allenarsi allo Speaking IELTS. Rispondi a voce alle domande di Part 1, 2 e 3, Azure Speech valuta la pronuncia (suoni, scorrevolezza, ritmo e intonazione) e con un tasto copi il risultato per farti valutare il resto da un assistente AI.

Funziona nel browser e si può installare sul telefono come app.

## Cosa ti serve

Una risorsa **Azure Speech** tua. La chiave resta salvata solo nel tuo browser e non passa da nessun server oltre a quello di Microsoft.

1. Crea un account Azure. Se sei studente universitario puoi usare **Azure for Students** con la mail dell'università, senza carta di credito.
2. Nel portale Azure cerca **Speech** (in italiano può comparire come **Voce**, nel Marketplace) e crea la risorsa con piano **Free F0**, che include 5 ore di audio gratis al mese.
3. Se la creazione fallisce con un errore di policy sulla regione, l'abbonamento studenti non permette quella regione. Prova Italy North, Sweden Central, France Central o Germany West Central.
4. Nella risorsa apri **Chiavi ed endpoint** e copia la Key 1 e la regione, scritta come in Posizione/Area (ad esempio `italynorth`).
5. Apri l'app, vai in Impostazioni e incolla chiave e regione.

## Sul telefono

Apri la pagina in Chrome e tocca **Installa** in alto, oppure dal menu scegli "Installa app" o "Aggiungi a schermata Home". Al primo uso consenti l'accesso al microfono.

## Note

- I punteggi di Azure vanno da 0 a 100 e non sono una band IELTS.
- Lo storico delle risposte resta solo nel browser del dispositivo che usi.
