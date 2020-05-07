# NOTA

## Astuces

Lancement d'une image docker pour tester en local le résultât

```bash
docker run -it --rm -v "$PWD":/usr/src/app -p "4000:4000" starefossen/github-pages
```
