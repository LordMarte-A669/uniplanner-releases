# UniPlanner — aggiornamenti

Qui ci sono solo gli aggiornamenti "over the air" dell'app UniPlanner: la parte web (`www/`)
zippata, cifrata e firmata, più un `manifest.json` per versione. Li pubblica in automatico la CI
del repo dei sorgenti, che è privato. Non si modifica niente a mano.

- **Non ci sono APK né sorgenti.** L'app installata scarica da qui solo il bundle più recente.
- **Ogni bundle è firmato.** L'app lo verifica con la chiave pubblica che ha dentro e scarta
  qualsiasi file non firmato dalla CI, anche se arrivasse da questo repo.
- `releases/latest/download/manifest.json` descrive l'ultima versione: numero, versione minima
  dell'APK che serve, URL dello zip, checksum firmato, chiave di sessione.
