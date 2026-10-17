# SmartHomeAI — Flows Node-RED

Système domotique intelligent : supervision temps réel de l'habitat, alertes automatiques
avec persistance cloud (Firebase) et assistant IA conversationnel — développé avec
**Node-RED** dans le cadre d'un projet d'équipe EMSI (2025/2026).

## Ma contribution

Conception et développement de **l'ensemble des 6 flows Node-RED**, le cœur logique du système :

| Flux | Rôle |
|------|------|
| F1 — Température & alertes | Acquisition simulée (toutes les 2 s), jauge + graphe temps réel, détection du seuil critique (> 35 °C) avec triple notification (popup UI, compteur, push Firebase) |
| F2 — Énergie | Simulation de la consommation (0–1000 W) et jauge Power Usage |
| F3 — Horloge | Heure système actualisée chaque seconde |
| F4 — Météo simulée | Rotation de 4 états météo toutes les 5 s |
| F5 — Authentification & sécurité UI | Login Firebase, verrouillage/déverrouillage dynamique des 6 pages du dashboard |
| F6 — Assistant IA | Parsing de 7 commandes en langage naturel, 3 sorties (réponse textuelle, pilotage lumière, pilotage porte) |

## Résultats

- 20 scénarios de test validés — **100 % de réussite** (fonctionnel, performance, sécurité)
- 38 alertes critiques générées, affichées et persistées en temps réel
- Latence d'affichage < 2 s, redéploiement des flows < 3 s

## Stack

Node-RED v4.1.9 · node-red-dashboard v3.6.6 · Firebase Realtime Database · Firebase Auth ·
JavaScript ES6+ · HTTP/REST · CSS3

## Fichiers

- `flows.json` — export complet des flows *(à ajouter : Node-RED → menu → Export → Clipboard → coller dans ce fichier)*
- `docs/` — captures d'écran du dashboard et de la console Firebase *(optionnel)*

## Équipe

Projet réalisé en équipe de 4 : Ahmed Edoublali, Ayoub Benaissa, Mohammed Darir, **Ilias Alame**
(ma partie : les flows Node-RED décrits ci-dessus). Encadré par Mr. Ali Hamidi — EMSI, 2025/2026.
