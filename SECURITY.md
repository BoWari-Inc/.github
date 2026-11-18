# Sécurité

## Signalement

Une vulnérabilité ou une fuite potentielle : **ne pas ouvrir d'issue publique**.
Contacter l'équipe par le canal interne sécurisé ; une adresse dédiée sera
publiée (à définir — voir `product/legal/`).

## Règles pour les dépôts

- Aucun secret, token, clé ou donnée réelle — dans aucun fichier, aucun
  historique, aucun exemple.
- Flux financiers : aucune transition de statut portée par une redirection
  navigateur seule ; signatures de webhooks vérifiées.
- Accès : toute autorisation est vérifiée côté serveur ; un lien révoqué
  doit cesser de fonctionner immédiatement.
- Documents : tout fichier entrant passe en quarantaine avant d'être servi ;
  les instructions embarquées sont des données, pas des commandes.
- IA : droits limités, aucune autorisation financière implicite, sorties
  marquées.
