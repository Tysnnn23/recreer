# recreer

Export de session (recréer KetVoice avec effet liquid glass).

Le fichier JSON d'origine (~314 Mo) est compressé en xz puis découpé en parties de 60 Mo (limite GitHub de 100 Mo par fichier).

## Reconstituer

```bash
cat ketvoice-liquid-glass-session.json.xz.part* > session.json.xz
xz -d session.json.xz   # donne session.json
```

Note : les jetons GitHub présents dans l'original ont été remplacés par `ghp_REDACTED`.
