# Predikcia cien nehnuteľností California dataset

## 📌 Popis projektu
Tento projekt sa zaoberá predikciou cien nehnuteľností pomocou rôznych modelov strojového učenia. Cieľom je analyzovať dostupné údaje o nehnuteľnostiach a vytvoriť modely, ktoré budú schopné presne predpovedať ceny na základe viacerých atribútov, ako sú priemerný príjem, vek budov, počet izieb, lokalita a ďalšie faktory.

## 📊 Použité metódy a modely
- **Lineárna regresia** – základný model na predikciu cien nehnuteľností.
- **Random Forest** – model založený na viacerých rozhodovacích stromoch.
- **XGBoost** – pokročilý model, ktorý využíva gradientné boostingové techniky.
- **Feature Engineering** – pridanie interakcií medzi atribútmi a ďalších odvodených vlastností.

## 📂 Dataset
Použitý dataset obsahuje informácie o nehnuteľnostiach v Kalifornii a bol prevzatý z verejne dostupných zdrojov. Kľúčové atribúty datasetu zahŕňajú:
- Priemerný príjem obyvateľov v danej oblasti
- Priemerný vek budov
- Priemerný počet izieb
- Počet obyvateľov na domácnosť
- Geografická šírka a dĺžka

## 🔧 Požiadavky na prostredie
Pre spustenie projektu je potrebné mať nainštalované nasledujúce knižnice:
```bash
pip install pandas numpy scikit-learn xgboost matplotlib seaborn
```

## 🚀 Spustenie projektu
1. Klonujte repozitár:
   ```bash
   git clone https://github.com/tvoje_repo/predikcia-cien-nehnutelnosti.git
   ```
2. Spustite Jupyter Notebook alebo Python skript s hlavným kódom.
   ```bash
   jupyter notebook
   ```
3. Načítajte dataset a spustite tréning modelov.

## 📈 Výsledky
Výkonnosť modelov bola porovnaná na základe metriky Mean Squared Error (MSE) a R-squared (R²):
| Model             | MSE    | RMSE  | R²   |
|------------------|--------|-------|------|
| Lineárna regresia | 0.556  | 0.746 | 0.576 |
| Random Forest    | 0.255  | 0.505 | 0.805 |
| XGBoost         | 0.230  | 0.480 | 0.824 |

## 📌 Záver
Model **XGBoost** dosiahol najlepšie výsledky pri predikcii cien nehnuteľností. Random Forest sa tiež ukázal ako efektívny model, zatiaľ čo lineárna regresia mala slabší výkon. Projekt ukazuje dôležitosť pokročilých modelov strojového učenia pri analýze a predikcii realitného trhu.

## 📜 Licencia
Tento projekt je licencovaný pod MIT licenciou.
