# Contribuer à BoWari

## Principes

- **Contrat d'abord** : aucun endpoint ni événement n'est implémenté sans son
  contrat publié dans `contracts` (revue consommateurs incluse).
- **États honnêtes** : jamais un état non vérifié affiché comme confirmé —
  vocabulaire partagé `design-system/docs/etats.md`.
- **Invariants non négociables** : `product/business-rules/invariants.md`
  (montants en chaîne d'unités mineures, registre append-only, révocation
  immédiate, IA sans effet métier, quarantaine documentaire).
- **Aucun secret dans un dépôt** — variables d'environnement et gestionnaire
  de secrets uniquement.

## Flux

1. Branche depuis `main`, commits atomiques, messages en français type
   `feat:`, `fix:`, `docs:`.
2. PR : contexte, scénarios CA couverts, captures si UI.
3. Revue : un développeur + le propriétaire du domaine pour les contrats.
4. CI verte obligatoire (build, tests, lint, et sur `contracts` : rupture oasdiff).

## Données

Jamais de données réelles, de secrets ou d'identités dans le code, les tests,
les exemples ou la documentation. Fixtures synthétiques uniquement.
