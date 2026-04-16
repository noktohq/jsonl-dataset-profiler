# JSONL Datasett-profiler

CLI-verktoy for profilering av JSONL-datasett for bruk i LLM-trening og testmiljoer.

## Funksjoner

- Analyserer alle felter i JSONL-filer
- Teller feltfrekvenser og null-rater
- Estimerer datatyper per felt
- Statistikk (min/maks/gjennomsnitt for tallfelt)
- Oppdager anomalier og tomme verdier

## Installasjon

```bash
pip install -r requirements.txt
```

## Bruk

```bash
python jsonl_profiler.py datasett.jsonl
python jsonl_profiler.py datasett.jsonl --output rapport.json
python jsonl_profiler.py datasett.jsonl --top 20
```

## Eksempelutdata

```
Felt              Type     Antall    Null%
id                int      10000     0.0%
tekst             str      10000     0.2%
etikett           str       9980     0.2%
score             float    10000     1.1%
```

## Ansvarsfraskrivelse

Verktoy laget for analyse av egne eller lisensierte datasett. Brukeren er ansvarlig for etterlevelse av GDPR og gjeldende personvernregler.

## Eier

[Nokto](https://nokto.no) — edin@nokto.no
