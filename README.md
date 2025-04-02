
---

# Predikcia Nehnuteľností - Predikcia Ceny Nehnuteľností

## Popis projektu

Tento projekt sa zameriava na predikciu cien nehnuteľností na základe rôznych faktorov, ako sú veľkosť nehnuteľnosti, počet izieb, poloha, vek budovy a ďalšie. Používame rôzne modely strojového učenia na predikciu ceny nehnuteľností a hodnotíme ich výkonnosť. Cieľom projektu je predpovedať ceny nehnuteľností v konkrétnych oblastiach na základe historických dát.

## Použité technológie

- **Python**: Programovací jazyk používaný pre analýzu a modelovanie.
- **Jupyter Notebook**: Na vykonávanie interaktívnych analýz a experimentov.
- **pandas**: Knižnica na manipuláciu s dátami.
- **numpy**: Knižnica na numerické operácie.
- **scikit-learn**: Knižnica pre strojové učenie.
- **matplotlib** a **seaborn**: Knižnice na vizualizáciu dát.

## Inštalácia

1. Skopírujte si tento repozitár do vášho lokálneho prostredia:
    ```bash
    git clone https://github.com/janastadtruckerova/real_est_prediction/.git
    cd real_est_prediction
    ```

2. Vytvorte a aktivujte virtuálne prostredie (voliteľné, ale odporúčané):
    ```bash
    python -m venv venv
    source venv/bin/activate  # Na Windows: venv\Scripts\activate
    ```

3. Nainštalujte požiadavky:
    ```bash
    pip install -r requirements.txt
    ```

4. Otvorte Jupyter Notebook:
    ```bash
    jupyter notebook
    ```

Po otvorení notebooku môžete prejsť cez jednotlivé kroky analýzy a modelovania.


## Modely použité v projekte

Tento projekt využíva rôzne modely strojového učenia na predikciu ceny nehnuteľností, medzi ktoré patrí:

### 1. **Lineárna regresia**
Lineárna regresia je základný model, ktorý predpovedá cenu nehnuteľnosti na základe jej vlastností ako je počet izieb, rozloha alebo poloha. Tento model sa osvedčil ako rýchly, ale môže mať obmedzenú výkonnosť v prípade nelineárnych vzorcov.

### 2. **Polynomiálna regresia**
Polynomiálna regresia rozširuje lineárnu regresiu pridaním polynomiálnych termínov, čo umožňuje modelu zachytiť nelineárne vzory medzi nezávislými a závislými premennými. Tento model je vhodný, keď dáta vykazujú nelineárny trend.

**Kľúčové vlastnosti:**
- Pridanie polynomiálnych termínov.
- Vhodné pre nelineárne vzory.
- Môže viesť k overfittingu pri príliš vysokej miere stupňa polynómu.

### 3. **Ridge regresia**
Ridge regresia je variant lineárnej regresie, ktorá využíva **L2 regularizáciu** na potlačenie veľkých koeficientov a zníženie overfittingu. Tento model je vhodný, keď máme veľký počet nezávislých premenných alebo keď chceme kontrolovať overfitting.

**Kľúčové vlastnosti:**
- Regularizuje koeficienty modelu.
- Pomáha pri overfittingu, zvlášť pri veľkých dátach.
- Menej citlivý na multikolineritu ako lineárna regresia.

### 4. **Random Forest**
Random Forest je ensemble model, ktorý vytvára množstvo rozhodovacích stromov a kombinuje ich predikcie. Tento model je veľmi silný pri zachytávaní zložitých nelineárnych vzorcov a dokáže lepšie zvládať aj nestruktúrované dáta.

## Výsledky

- **Lineárna regresia**: Tento model dosiahol R² skóre **0.5758** na testovacích dátach, čo naznačuje, že model dokáže relatívne presne predpovedať ceny, ale je tu ešte priestor na zlepšenie.
- **Polynomiálna regresia (degree=3)**: Tento model dosiahol **R² skóre -2.3318**, čo naznačuje, že model sa overfittoval, pretože nebol schopný generalizovať na testovacích dátach.
- **Ridge regresia**: Tento model dosiahol **R² skóre 0.5823**, čo je lepšie ako lineárna regresia. Regularizácia pomohla zlepšiť výkon modelu.
- **Random Forest**: Tento model dosiahol **R² skóre 0.8062**, čo naznačuje, že model dokáže predpovedať ceny s vysokou presnosťou.

## Predpoklady

- **Python 3.x**
- **pandas, numpy, scikit-learn, matplotlib, seaborn** (tieto knižnice sú uvedené v súbore `requirements.txt`)

## Prispievanie

1. Forknite tento repozitár.
2. Vytvorte novú vetvu (napr. `feature-addition`).
3. Vykonajte zmeny a pridajte nové funkcie.
4. Pošlite pull request.

## License

Tento projekt je licencovaný pod MIT License - pozrite si **LICENSE** súbor pre viac informácií.







-


