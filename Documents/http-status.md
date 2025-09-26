Ce fichier explique les codes de status avec catégories

1xx : information



2xx : succès (200 OK, 201 Created)



3xx : redirection (301, 302)



4xx : erreur client (400, 404)



5xx : erreur serveur (500, 503)



exemple curl -i http://localhost/ressource-inexistante



| Famille | Signification           | Exemple | Cas d’usage typique                |

|---------|-------------------------|---------|------------------------------------|

| 1xx     | Information             | 100     | Le serveur continue le traitement  |

| 2xx     | Succès                  | 200     | Requête réussie                    |

| 3xx     | Redirection             | 302     | Rediriger vers une autre URL       |

| 4xx     | Erreur côté client      | 404     | Ressource introuvable              |

| 5xx     | Erreur côté serveur     | 500     | Problème interne du serveur        |

