# ❓ FAQ – Fer à souder DIY tige de panini

## 🔹 Généralités

### Pourquoi utiliser une tige de panini ?
C’est une résistance chauffante bon marché, facile à trouver, mécaniquement robuste et facile à usiner.

### Puis-je utiliser une autre longueur ?
Oui, mais la résistance change.  
- Plus longue → résistance plus élevée → courant plus faible → moins de puissance  
- Plus courte → résistance plus faible → courant plus élevé (risque pour l’alimentation)

### Quelle alimentation choisir ?
Une **12 V – 5 A (60 W)** est idéale.  
Une 19 V nécessite une limitation de courant (résistance série ou PWM).

---

## 🔹 Température et soudure

### Mon étain ne fond pas bien
Causes possibles :
- Alimentation 12 V mais étain sans plomb (nécessite 300 °C)
- Panne oxydée (nettoyer avec éponge humide)
- Mauvais contact thermique (panne mal façonnée)

### L’étain fume ou noircit
Température trop élevée (rare en 12 V).  
Solutions :
- Vérifier l’alimentation (tension réelle)
- Ajouter un module PWM pour réduire la puissance

### Quelle panne utiliser ?
Une panne plate (façonnée à la lime douce) offre un bon compromis pour la plupart des soudures.

---

## 🔹 Mesures électriques

### Je n’ai pas de multimètre, comment faire ?
Tu peux procéder par essais :
- Si l’étain fond bien → c’est bon
- Si l’alimentation s’arrête → surcharge (réduire la résistance en série)

### Pourquoi mes courants sont différents de la théorie ?
La résistance de la tige augmente légèrement avec la température (effet PTC).  
Une variation de ±5 % est normale.

---

## 🔹 Sécurité

### L’alimentation chauffe, est-ce normal ?
Une légère chaleur est normale (rendement ~80 %).  
Si elle devient brûlante → surcharge ou ventilation insuffisante.

### Puis-je laisser le fer branché longtemps ?
Déconseillé : usure de la panne, risque d’incendie, consommation inutile.  
Ajoute un interrupteur ou débranche après usage.

### La panne est-elle sous tension dangereuse ?
Non : 12 V DC est une **très basse tension** (SELV), aucun risque d’électrocution.  
Mais attention à la **brûlure** (température élevée).

---

## 🔹 Dépannage

| Problème | Cause probable | Solution |
|----------|----------------|----------|
| L’alimentation se coupe | Surcharge (trop de courant) | Ajouter résistance série ou utiliser 12 V |
| Panne qui bleuit / s’oxyde vite | Température trop élevée | Réduire tension ou ajouter PWM |
| Soudure terne / granuleuse | Manque de flux ou étain de qualité médiocre | Ajouter flux externe, changer d’étain |
| L’étain ne tient pas sur la panne | Panne non étamée | Nettoyer + déposer un peu d’étain neuf |

---

## 🔹 Évolutions

### Comment passer à l’étain sans plomb ?
Deux solutions :
1. Alimentation 19 V + résistance série 0,8 Ω / 20 W
2. Alimentation 19 V + module PWM (réglage manuel)

### Puis-je ajouter un contrôle de température ?
Oui : thermocouple + ampli MAX6675 + Arduino + afficheur LCD.

### Puis-je utiliser une batterie ?
Oui : batterie 12 V (voiture, outil, etc.) à condition qu’elle puisse fournir 3 A en continu.