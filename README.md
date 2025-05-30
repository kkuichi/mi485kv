# Názov bakalárskej práce
**Identifikácia podvodov v poisťovníctve**

## Jednoduchý prehľad  
Tento projekt využíva modely strojového učenia na detekciu podvodných poistných udalostí. Obsahuje kompletný postup podľa metodológie CRISP-DM: pochopenie cieľa, pochopenie dát, predspracovanie dát, modelovanie, vyhodnotenie a nasadenie.

## Abstrakt  
Bakalárska práca sa zaoberá identifikáciou poistných podvodov s dôrazom na aplikáciu dátovej analytiky a strojového učenia. Cieľom je navrhnúť a porovnať klasifikačné modely na detekciu podov, využitím CRISP-DM. V teoretickej časti práca analyzuje aktuálny stav poznania v oblasti digitálnej detekcie podvodov, popisuje hlavné typy poistných podvodov a prehľad metód strojového učenia. V praktickej časti sa implementujú algoritmy Logistickej regresie, XGBoost, Gradient Boosting, RF a DT na verejne dostupných dátach. Kľúčovou súčasťou praktickej implementácie bolo riešenie problematiky nevyvážených dát pomocou techník SMOTE a ADASYN. Jednotlivé modely sú vyhodnocované vhodnými metrikami. Výsledky preukázali, že vyváženie dát signifikantne zlepšuje schopnosť modelov detegovať podvody. Ako najlepší model sa preukázala Logistická Regresia s úspešnosťou 85%. Práve preto je výsledkom tejto práce súbor získaných znalostí a komplexné porovnanie použitých metód a modelov, nadobudnutých počas vykonávania rozsiahlych experimentov na dostupnom dátovom súbore.

## Getting started 

### Inštalácia knižníc
Zoznam hlavných knižníc, ktoré sú potrebné aby boli nainštalované v najnovšej verzii:

- pandas
- numpy 
- scikit-learn
- xgboost
- imbalanced-learn
- shap
- matplotlib
- seaborn

### Dataset
Pre túto prácu bol použitý dataset dostupný na adrese: https://databricks-prod-cloudfront.cloud.databricks.com/public/4027ec902e239c93eaaa8714f173bcfc/4954928053318020/1058911316420443/167703932442645/latest.html , ktorý sme v našej práci použili ako vstupný daataset súbor `insurance_data.csv`. 

### Použité modely
Modely, ktoré boli trénované a testované:

- Logistic Regression
- Gradient Boosting
- Decision Tree
- Random Forest
- XGBoost
- VotingClassifier (kombinovaný model)

### Použité metriky na vyhodnotenie
Výber najlepšieho modelu prebiehal na základe metrík:
- úspešnosť (accuracy)
- presnosť (precision)
- návratnosť (recall)
- F1-skóre
- ROC AUC

### Interpretácia modelou
Pre interpretáciu bola použitá knižnica SHAP (SHapley Additive exPlanations), ktorá pomáha vizualizovať dôležitosť príznakov pre jednotlivé predikcie.

## Autori  
- **Miriam Ihnátová**  
  GitHub: [@MiriamIhnatova](https://github.com/MiriamIhnatova)  
  Školiteľ: Ing. Anna Biceková, PhD.
