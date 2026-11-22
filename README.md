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

## Band IELTS automatica, facoltativa

Con una risorsa **Azure OpenAI** l'app stima da sola la band IELTS sui quattro criteri, con correzioni e una versione migliorata della risposta. Senza questa parte puoi usare il tasto Copia per Claude e incollare il risultato in una chat.

1. Nel portale cerca **Azure OpenAI**, crea la risorsa nello stesso gruppo con piano Standard. Si paga a consumo dai crediti e ogni valutazione costa pochissimo.
2. Dalla risorsa apri il portale Foundry, vai su Distribuzioni e distribuisci un modello piccolo, ad esempio `gpt-5-mini` o `gpt-4.1-mini`, con tipo Global Standard.
3. In Chiavi ed endpoint copia endpoint e Key 1, poi inseriscili nelle Impostazioni dell'app insieme al nome della distribuzione.

## Esame completo

La modalità Esame completo simula lo Speaking vero, con 4 domande di Part 1, una cue card di Part 2 con un minuto di preparazione e 4 domande di Part 3 sullo stesso tema. La valutazione arriva alla fine, sull'insieme delle risposte, come all'esame.

## Sul telefono

Apri la pagina in Chrome e tocca **Installa** in alto, oppure dal menu scegli "Installa app" o "Aggiungi a schermata Home". Al primo uso consenti l'accesso al microfono.

## Note

- I punteggi di Azure vanno da 0 a 100 e non sono una band IELTS.
- Lo storico delle risposte resta solo nel browser del dispositivo che usi.
