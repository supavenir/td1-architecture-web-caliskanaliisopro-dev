**GET : récupérer une ressource**



**POST : envoyer/créer des données**



**PUT : remplacer une ressource**



**PATCH : modifier partiellement**



**DELETE : supprimer**



**HEAD : obtenir seulement les en-têtes**



**OPTIONS : connaître les méthodes supportées**



**En exemple :**



**curl -X GET http://localhost/**

**curl -X POST http://localhost/ -d "nom=Ali"**

**curl -X PUT http://localhost/ressource/1 -d "valeur=42"**

**curl -X DELETE http://localhost/ressource/1**



**## Exemple concret : GET**

**\*\*Contexte\*\* : récupération d’une page d’accueil.**  

**\*\*URL\*\* : `http://dev.local/?search=livre`**  

**\*\*Requête\*\* :**

**- Méthode : GET**

**- Headers : `Accept: text/html`**

**- Corps : vide**  

**\*\*Réponse\*\* :**

**- Status : `200 OK`**

**- Headers : `Content-Type: text/html`**

**- Extrait du corps :**

**```html**

**<html><body>Résultats pour "livre"</body></html>**



**Exemple concret : POST**



**Contexte : envoi d’un formulaire d’inscription.**

**URL : http://dev.local/register**

**Requête :**



**Méthode : POST**



**Headers : Content-Type: application/x-www-form-urlencoded**



**Corps : username=ali\&password=1234**

**Réponse :**



**Status : 201 Created**



**Headers : Content-Type: application/json**



**Extrait du corps :**



**{"message": "Utilisateur créé"}**

