# UniPlanner — download e aggiornamenti

**Per installare l'app: <https://lordmarte-a669.github.io/uniplanner-releases/>** (è la pagina del QR code).

Questo repo contiene solo ciò che la CI del repo dei sorgenti (privato) pubblica a ogni versione.
Non si modifica niente a mano, tranne la pagina di download (`index.html`, `qr.png`, `qr.svg`, `icon.svg`).

- **APK**: `uniplanner-X.Y.Z.apk` e la stessa col nome fisso `uniplanner.apk`, così
  `releases/latest/download/uniplanner.apk` porta sempre all'ultima.
- **Aggiornamenti automatici**: la parte web dell'app (`www/`) zippata, cifrata e firmata, più
  `manifest.json`. L'app installata li scarica da sola e scarta qualsiasi file non firmato dalla CI.
- `releases/latest/download/manifest.json` descrive l'ultima versione: numero, APK minima
  richiesta, URL dello zip e dell'APK, checksum firmato, chiave di sessione, novità.
