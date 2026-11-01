# Padel Uren

PWA voor een padeltrainer: lessen en uren bijhouden (privé en groep), facturen als PDF maken en delen, omzet-dashboard, back-up.

- Geen server en geen account: alle gegevens staan in IndexedDB op de telefoon. Back-up via Instellingen.
- Statische bestanden, geen build. Lokaal draaien: `python3 -m http.server 8131`.
- PDF met jsPDF 2.5.1 (lokaal in `lib/`, MIT), werkt offline.
- Na een wijziging: `VERSIE` in `sw.js` ophogen, anders blijft de oude versie in de cache.

## Versie voor Marijn
Kopie van [daanbauman/padel-uren](https://github.com/daanbauman/padel-uren). Eigen database (`padel-uren-marijn`) en eigen cache, zodat deze app nooit gegevens deelt met die van Daan, ook niet als ze op hetzelfde domein draaien. Back-ups blijven uitwisselbaar. Marijn vult zijn naam, IBAN en tarieven in via Instellingen (tandwiel).
