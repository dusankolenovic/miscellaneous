# Kreditni kalkulator (stan F606)

Kalkulator za kupovinu stana: uplate investitoru do podizanja kredita, pa otplata kredita po pravim mesecima.

- `index.html`: ceo kalkulator (Parametri, Scenario otplate, Dnevnik po mesecima, grafikoni).
- `uplate-investitoru.html`: jednostavna tabela mesečnih uplata investitoru (okt 2026 do nov 2027).
- `data/kalkulator.json`: sačuvani scenario (cena, plata, troškovi, događaji, povrat PDV-a, faze).

Žive verzije:
- Kalkulator: https://claude.ai/artifact/CxBLCeiAGfJQkAZYY7mWKd
- Uplate investitoru: https://claude.ai/artifact/MP3sBoGx96T2HcvVu9ztx4

## Lokalno pokretanje

Stranica čita `data/kalkulator.json` preko `fetch`, pa je otvori preko lokalnog servera, ne duplim klikom:

```
cd kreditni-kalkulator
python3 -m http.server 8000
```

pa otvori http://localhost:8000. Čuvanje izmena i asistent rade samo u živoj verziji na claude.ai; lokalno se scenario menja, ali se ne čuva.
