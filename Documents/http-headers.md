Permet d expliquer les en-têtes de rerquête et de réponse



Requête : Accept, Authorization, User-Agent

Réponse : Content-Type, Set-Cookie, Location

exemple de curl :

curl -I http://localhost/

curl -H "Accept: application/json" http://localhost/api



\# Extensibilité de HTTP



HTTP est extensible car :

\- On peut définir de \*\*nouvelles méthodes\*\* (ex: WebDAV → PROPFIND, MKCOL).

\- On peut ajouter de \*\*nouveaux en-têtes\*\* (ex: `X-Request-ID`, `Authorization`).

\- De nouveaux \*\*codes de statut\*\* apparaissent (ex: `418 I'm a teapot`, `429 Too Many Requests`).

\- Les \*\*versions évoluent\*\* (HTTP/1.1 → HTTP/2 → HTTP/3).

\- Négociation de contenu : formats (`Accept`), langues (`Accept-Language`), encodage (`Accept-Encoding`).



\## Exemple OPTIONS

```bash

curl -X OPTIONS http://dev.local/ -i

