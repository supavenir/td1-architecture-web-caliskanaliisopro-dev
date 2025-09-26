Permet d 'expliquer la structure d'une URL



schéma://utilisateur:motdepasse@hôte:port/chemin?requête#fragment



EXEMPLE : https://user:pass@exemple.com:8080/dossier/page?tri=date#section2



| Partie       | Exemple               | Rôle                                |

|--------------|-----------------------|-------------------------------------|

| Schéma       | https                 | Protocole utilisé                   |

| Identifiants | user:pass             | Authentification (optionnelle)      |

| Hôte         | dev.local             | Domaine ou adresse IP               |

| Port         | 443                   | Port du service (443 = HTTPS)       |

| Chemin       | /api/v1/resources     | Chemin de la ressource              |

| Requête      | q=abc\&page=2          | Paramètres de recherche             |

| Fragment     | section-3             | Ancre dans la ressource             |

