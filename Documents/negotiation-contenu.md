Explique la négociation du contenu en tête



exemple en curl :



curl -H "Accept: text/html" http://localhost/api

curl -H "Accept: application/json" http://localhost/api



Réponses possibles :



Content-Type: text/html → renvoie du HTML



Content-Type: application/json → renvoie du JSON



\# Négociation de contenu



\## Principe

Le client précise ses préférences dans les en-têtes :

\- `Accept`: format (`text/html`, `application/json`)

\- `Accept-Language`: langue (`fr-FR`, `en-US`)

\- `Accept-Encoding`: compression (`gzip`, `br`)

\- `Content-Type`: type du corps envoyé

\- `Vary`: indique sur quels en-têtes la réponse varie



\## Exemple

Requête JSON :

```bash

curl -i http://dev.local/api -H "Accept: application/json"

