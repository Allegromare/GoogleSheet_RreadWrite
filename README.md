# GoogleSheet_RreadWrite

Aprire il foglio google che si vuole utilizzare:

<img width="1325" alt="Schermata 2022-08-26 alle 22 52 44" src="https://user-images.githubusercontent.com/66548449/186989072-cc8d6164-052f-4710-9703-bbaa62aded0d.png">

Premere il pulsante Condividi in alto a sinistra e verrà visualizzata la seguente schermata:

<img width="494" alt="Schermata 2022-08-26 alle 22 46 11" src="https://user-images.githubusercontent.com/66548449/186988283-d0e1bf3c-7784-46b1-8366-a84154024bba.png">

NB: nel mio caso ho messo le opzioni più ampie, capire se è possibile limitare l'accesso.

Premere il pulsante Copia Link per ottenere il link del foglio che nel mio caso è https://docs.google.com/spreadsheets/d/1ofJ5rMHBuHiDOZYHs7p2ECbd2beJNBqX0kix4xI2RJQ/edit?usp=sharing

Dal link si ottiene l'ID del foglio che nel mio caso è: 1ofJ5rMHBuHiDOZYHs7p2ECbd2beJNBqX0kix4xI2RJQ

Se non fatto in precedenza abilitare le Google Sheets API (trovate le indicazioni al seguente link: https://developers.google.com/sheets/api/quickstart/python

Se non già presenti nel sistema (o se avete creato un ambiente virtuale), istallate i moduli necessari attraverso i seguenti comendi

pip install google_spreadsheet
pip install google-auth-oauthlib
pip install pandas

Creare un progetto in Google Cloud Platform ed abilitare le API

- Aprire la Google CLoud Platform https://console.cloud.google.com/

Se è la prima volta che lo si fa, accettare le condizioni

<img width="541" alt="Schermata 2022-08-26 alle 23 26 37" src="https://user-images.githubusercontent.com/66548449/186993102-f3a063c5-e13f-4e87-855f-00ad418abd03.png">

- Poi Menu > IAM e Amministrazione > Crea un progetto
- Dare un nome al progetto e premere CREA

<img width="596" alt="Schermata 2022-08-26 alle 23 32 20" src="https://user-images.githubusercontent.com/66548449/186993681-8fa2bdac-07aa-41df-b15d-0b84fa6707d4.png">

- Abilitare le Google Workspace API per il progetto

Menu > API e Servizi > Libreria (per la versione inglese Menu > APIs & Services > Library)

Nel campo ricerca scrivere "sheet" in modo da cercare la corrispondete API fra le molte messe a disposizione:

<img width="1033" alt="Schermata 2022-08-26 alle 23 37 32" src="https://user-images.githubusercontent.com/66548449/186994263-fe3f8941-393a-4b88-87ea-34c93fbd38a2.png">

Cliccare sulla scheda Google Sheets API e si aprirà la seguente schermata:

<img width="696" alt="Schermata 2022-08-26 alle 23 39 35" src="https://user-images.githubusercontent.com/66548449/186994560-b8dbb764-51c2-477f-a4ce-3adfd36a170f.png">

Premere ABILITA
NB: è presente anche al documentazione e Tutorial sull'utilizzo dell'API

Ci verrà segnalata la necesità di creare delle credenziali per utilizzare l'API

<img width="1310" alt="Schermata 2022-08-26 alle 23 43 35" src="https://user-images.githubusercontent.com/66548449/186995015-fbb8f454-5a66-4c7d-af77-07bd54344177.png">

Premendo il pulsante CREA CREDENZIALI verrà mostrata la schermata che segue

<img width="812" alt="Schermata 2022-08-26 alle 23 48 19" src="https://user-images.githubusercontent.com/66548449/186995292-6bc8e319-6271-4c54-bb54-a7ae5b3fb819.png">

Scegliere "Dati applicazione", poi "No, non le sto usando e premere il pulsante AVANTI (attenzione che è un po' nascosto, mentre è molto evidente il tasto FINE che se premuto però vi porterà solamente alla schermata precedente)

Inserire il nome dell'account di servizio (io ho scelto gsrw), il sistema creerà ul ID account di servizio, e premere CREA E CONTINUA

<img width="812" alt="Schermata 2022-08-26 alle 23 48 19" src="https://user-images.githubusercontent.com/66548449/186995948-772fe233-d128-4bcb-93a8-f451e2361f6f.png">

Come ruolo scegliere Amministratore account di servizio e premere CONTINUA


<img width="706" alt="Schermata 2022-08-27 alle 00 04 16" src="https://user-images.githubusercontent.com/66548449/186996690-dcf90c3b-0d28-4a2b-9f64-a995c35aadfb.png">

Premere fine

<img width="731" alt="Schermata 2022-08-27 alle 00 06 06" src="https://user-images.githubusercontent.com/66548449/186996787-58ebbbd0-c75a-4cb1-82bc-0ba9d1b93486.png">





