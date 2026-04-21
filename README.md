# AGE — App Maraîcher

Prototype d'interface mobile pour les agriculteurs clients du kit solaire AGE en Angola.

---

## C'est quoi AGE ?

AGE propose des kits solaires agricoles aux petits maraîchers d'Angola, principalement dans la région de Huambo. Le kit comprend des panneaux solaires, une pompe à eau et une chambre de conservation — le tout accessible via un contrat de leasing mensuel (modèle Pay-As-You-Go), sans apport initial.

L'idée centrale : transformer la dépense diesel hebdomadaire (~40 000–50 000 AOA/mois) en un investissement durable à 8 500 AOA/mois, remboursable petit à petit.

---

## Ce que fait cette page HTML

C'est une **simulation d'application mobile** — une seule page HTML, sans backend, qui tourne dans n'importe quel navigateur. Elle est conçue pour ressembler à une vraie app sur smartphone (coque téléphone incluse).

Elle s'adresse au persona **Pedro Kissanga**, 25 ans, maraîcher à Caála (Huambo), qui n'a pas d'ordinateur et utilise uniquement son téléphone.

### 4 écrans navigables

**Accueil**
- Résumé des économies du mois vs dépense diesel
- Stats rapides : litres d'eau pompés, énergie solaire produite, jours avant prochain paiement
- Alertes : état de la pompe, stress thermique (risque brûlures cultures), sécurité du kit, rappel de paiement

**Leasing**
- Explication du modèle Pay-As-You-Go
- Anneau de progression du remboursement (40% remboursé)
- Historique des mensualités (payé / en cours / à venir)
- Modal de paiement avec choix entre **Unitel Money** et **BAI Directo**

**Parcelle**
- Liste des cultures en cours (choux, tomates, oignons) avec surface et stade
- Formulaire pour ajouter une nouvelle culture
- Suivi des récoltes vendues au marché local avec formulaire d'enregistrement

**Compte**
- Fiche profil du client
- Détail des composants du kit (panneau solaire 600 Wc, pompe 0,75 kW, chambre de conservation)
- Cumul des économies réalisées depuis l'installation
- Historique financier (économies diesel + paiements leasing)
- Témoignage d'un voisin (levier de preuve sociale, facteur déclencheur d'achat identifié dans le persona)
- Boutons de contact AGE (WhatsApp + appel technicien)

---

## Contexte projet

Ce prototype a été construit dans le cadre du **Track Entrepreneurial de l'ESSEC Business School** (Séance 3 Coaching). Il s'appuie sur :

- Un **Value Proposition Canvas** qui identifie les douleurs clés des maraîchers (coût diesel, stress thermique, pannes, vol du matériel) et les gains apportés par le kit AGE
- Un **persona terrain** construit à partir d'entretiens avec des agriculteurs de Huambo
- Un **benchmark concurrentiel** face à GenRent, SunCulture et les PME solaires locales (ENF Solar Angola)
- Une **matrice ERRC** (Éliminer / Réduire / Renforcer / Créer) qui positionne AGE sur l'agrivoltaïsme accessible

---

## Stack technique

Rien à installer. C'est du HTML/CSS/JS pur dans un seul fichier.

```
age-app/
└── index.html   # tout est là
```

Ouvrir `index.html` dans un navigateur suffit.

---

## Points de design

- Interface pensée pour un écran 390px (iPhone standard) — mobile-first
- Palette terre/eau/feuille cohérente avec l'univers agricole
- Textes en français, contexte angolais (AOA, Unitel Money, BAI Directo, noms locaux)
- Pas de dépendance externe (pas de librairie, pas de framework)
