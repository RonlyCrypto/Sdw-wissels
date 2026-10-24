# SDW Wissels

Teamapp voor jeugdvoetbal: agenda met aanwezigheid, eerlijk wisselschema (4 × 10 min, wissel elke 5 min, keeper per kwart), live wedstrijdklok en doelpunten.

- **Website:** https://sdw-wissels.vercel.app/
- **Android-app:** `SDW-Wissels.apk` bij [Releases](https://github.com/RonlyCrypto/Sdw-wissels/releases/latest). De app laadt altijd de nieuwste versie van de website.

## Aanmelden
1. Kies je team.
2. Vul je naam in en de teamcode:
   - `STAF-…` → coach (alles aanpassen). De teammanager kan rollen wijzigen en codes vernieuwen.
   - `OUDER-…` → ouder (alles bekijken, aanwezigheid van eigen kind doorgeven).
3. Op een tweede telefoon meld je je aan met dezelfde naam en code.

De gegevens staan in Supabase (project `sdw-wissels`, tabellen `app_*`). Alle toegang loopt via de functies `app_get` en `app_act`, die de rol van de ingelogde gebruiker controleren.
