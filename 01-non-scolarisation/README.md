# Non-scolarisation des filles (12–23 ans) en Mauritanie — Analyse statistique & économétrique

**Contexte.** Malgré les progrès d’accès à l’éducation, la non-scolarisation des adolescentes et jeunes femmes reste élevée, surtout en zones rurales.

## Données
- **Source** : Enquête Permanente sur les Conditions de Vie des ménages (**EPCV 2019–2020**)
- **Population étudiée** : filles âgées de **12 à 23 ans**
- **Variable cible** : *Non scolarisée* (1) vs *Scolarisée* (0)

> ⚠️ Les micro-données ne sont pas publiées (confidentialité). Voir `data/README.md`.

## Méthodes
1. **Descriptif** : distributions + tableaux croisés  
2. **Bivarié** : tests **χ²** + **V de Cramer**  
3. **Exploratoire multivarié** : **ACM**  
4. **Modélisation** : **régression logistique binaire** (interprétation via **Odds Ratios**)  

## Résultats clés (extraits du rapport)
- **57,5 %** des filles (12–23 ans) sont **non scolarisées**
- Raisons principales : **enseignement coranique/mahadra (20,1 %)**, **éloignement/manque d’école (16 %)**, **mariage/grossesse (13,6 %)**
- Régression logistique (OR) : **urbain vs rural 0,27** ; **accès difficile 2,51** ; **pauvreté 1,54** ; **mariée 5,22** ; **19–23 ans vs 12–15 ans 7,46**
- Qualité prédictive : **AUC = 0,84** ; **accuracy ≈ 75 %**

## Figures sélectionnées
### Raisons de non fréquentation scolaire
![Raisons](figures/reasons_non_frequentation.png)

### Situation scolaire
![Situation](figures/situation_scolaire.png)

### ACM (profils associés à la scolarisation vs non-scolarisation)
![ACM](figures/acm_plot.png)

### Courbe ROC (AUC = 0,84)
![ROC](figures/roc_curve_auc_0_84.png)

### Résultats logit (tableau)
![Logit 1](figures/logit_results_table.png)
![Logit 2](figures/logit_results_table_cont.png)

## Livrables
- `report_1page.pdf` : synthèse 1 page (portfolio)
- `full_report.pdf` : rapport complet

