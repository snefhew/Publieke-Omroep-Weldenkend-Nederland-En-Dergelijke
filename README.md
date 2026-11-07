# PowNed Redactie Agent

Schoolproject: concept en demo van een AI-agent die lokaal nieuws met landelijke potentie klaarzet voor de redactie. [Demo](https://snefhew.github.io/Publieke-Omroep-Weldenkend-Nederland-En-Dergelijke/)

## Stack

- n8n (self-hosted)
- RSS, sitemaps en API's, Trafilatura
- LLM voor samenvatten en scoren
- PostgreSQL

## Pipeline

```
30+ bronnen -> tekst ophalen -> dedupliceren (hash) -> PostgreSQL
            -> samenvatten en scoren -> feed van 50 items voor 08:30
```

De AI stelt voor, de redactie beslist. Elk item krijgt een uitleg waarom het is geselecteerd.
