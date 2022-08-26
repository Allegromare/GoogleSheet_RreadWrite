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

-
