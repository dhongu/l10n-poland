# l10n-poland

Localizare Odoo pentru Polonia (Terrabit).

## Module

- `l10n_pl_zip` — localitățile (Polish) cu codul poștal, legate de regiunile țării; completează localitatea
  și regiunea din codul poștal și leagă contactele existente de localitatea codului lor poștal: la
  instalare, direct pe o bază mică sau printr-o acțiune programată, pe loturi, pe una mare.

## Date

Lista de localități vine din [GeoNames](https://www.geonames.org) (licență Creative Commons
Attribution 4.0). Pentru reîmprospătare:

```bash
curl -sSfLO https://download.geonames.org/export/zip/PL.zip && unzip PL.zip PL.txt
python3 scripts/generate_city_data.py PL.txt
```
