# 🔧 Fer à souder DIY à partir d’une tige de panini

**Auteur** : Projet personnel  
**Version** : 1.0  
**Date** : Mai 2026  
**Licence** : CC BY-NC 4.0  

---
# 🔧 Fer à souder DIY – Tige de panini 12V

> **Un fer à souder basse tension, simple, sûr et économique, fabriqué à partir d’une résistance de panini (4,5Ω) et d’une alimentation 12V – 60W.**
<img width="1200" height="1600" alt="image" src="https://github.com/user-attachments/assets/3ade0e19-2ee6-4a1a-820a-7a2c09e67899" />

## 📖 Résumé

Ce document décrit la réalisation d’un **fer à souder électronique basse tension** à partir d’une **résistance chauffante de 4,5 Ω** (portion de tige de panini), alimentée par un convertisseur **12 V – 60 W**.

L’ensemble permet des soudures propres sur fils cuivre, circuits époxy et bakélite, avec un étain **60/40 – flux 2 %**.  
Aucun composant électronique complexe n’est nécessaire : la solution est simple, économique et reproductible.

---

## 🎯 Objectifs

- Construire un fer à souder fonctionnel avec des moyens limités
- Utiliser une alimentation secteur-basse tension standard (SELV)
- Atteindre une température de panne comprise entre 230 °C et 280 °C
- Assurer la sécurité électrique et thermique

---

## 🧱 Matériel utilisé

| Composant | Référence / Caractéristiques |
|-----------|-------------------------------|
| Résistance chauffante | Portion de tige de panini : **4,5 Ω**, **6 cm** |
| Alimentation | Sloaled – 12 V – 5 A – 60 W – Classe II – SELV |
| Étain | Alliage **60/40 (Sn60Pb40)** – diamètre **0,8 mm** – flux **2 %** |
| Panne | Plaquée / façonnée depuis la tige |
| Manche | Récupéré d’un ancien fer à souder hors service |
| Multimètre | Contrôle des tensions et courants |

---

## ⚡ Caractéristiques électriques

### Résistance mesurée à froid
- Tige seule : **4,5 Ω** (vérifié au multimètre)

### Régime permanent (après stabilisation thermique)
- Tension d’alimentation : **12 V DC**
- Courant consommé : **2,63 A**
- Puissance dissipée : **≈ 31,6 W**

### Calculs théoriques (loi d’Ohm)
I = U / R = 12 / 4,5 ≈ 2,67 A

P = U × I = 12 × 2,67 ≈ 32 W

Les mesures réelles sont cohérentes avec la théorie.

---

## 🌡️ Température de panne (estimée sans thermomètre)

| Méthode d’estimation | Résultat |
|----------------------|----------|
| Comportement de l’étain (60/40) | Brillant, coule bien sans brûler |
| Test papier | Brunit sans flamber |
| Fusion de l’étain plombé | Rapide et fluide |

➡️ **Température estimée : 230 °C – 280 °C**  
Plage idéale pour l’étain 60/40.

---

## 🔌 Schéma électrique simplifié
Secteur 230V AC
│
▼
┌──────────────┐
│ Convertisseur               │
│ 12V DC / 5A │ (Sloaled)
└──────┬───────┘
│
├────────────┐
│                                   │
▼                                  ▼
+12V                          GND
│                                   │
│   ┌──────────┘
│   │
▼ ▼
┌───┴───┴───┐
│ Tige                       │
│ 4,5 Ω                      │
│ (panne)                 │
└───────────┘

> Aucune résistance série ni composant actif n’est nécessaire.

---
## ✅ Résultats pratiques

| Type de soudure | Résultat |
|----------------|----------|
| Fils multibrins (cuivre) | Bonne pénétration, brillance correcte |
| Plaques époxy simple face | Très bonne adhérence |
| Plaques bakélite | Soudures propres |
| Petits composants CMS | Facile, pas d’excès de chaleur |
| Gros plans de masse / câbles épais | Limite (manque d’inertie thermique) |

---

## ⚠️ Sécurité et bonnes pratiques

- La panne atteint **plus de 200 °C** → support isolant indispensable
- L’alimentation SELV est **sécurisée** (pas de risque d’électrocution)
- Laisser refroidir avant rangement
- Ne pas laisser chauffer sans surveillance prolongée
- Nettoyer la panne avec éponge humide avant chaque soudure
- Ne jamais limer la panne (risque de détruire le revêtement)

---

## 🧪 Évolutions possibles (optionnel)

| Modification | Bénéfice |
|--------------|----------|
| Ajout d’un interrupteur pied | Sécurité / économie d’énergie |
| Module PWM entre 12V et tige | Réglage fin de la température |
| Ajout d’un thermocouple + afficheur | Contrôle précis (pour perfectionnistes) |
| Alimentation 19 V + résistance série (0,8 Ω / 20 W) | Permet l’étain sans plomb |

---

## 📚 Références utiles

- Loi d’Ohm : \( U = R \times I \)
- Étain 60/40 : fusion 183 → 190 °C, usage électronique standard
- Sécurité SELV : Très Basse Tension de Sécurité (< 60 V)

---

## 🙏 Remerciements

Projet réalisé par étapes : mesures, essais, ajustements.  
Ce document est publié pour aider d’autres bricoleurs à reproduire ou adapter cette solution.

---
