# Analisi del Mercato delle Auto Usate e Fattori di Svalutazione

## Panoramica del Progetto
Questo progetto analizza un dataset di oltre 2.800 auto usate per identificare i principali fattori che influenzano il prezzo di vendita e comprendere le dinamiche di svalutazione dei veicoli sul mercato.

L'obiettivo è fornire indicazioni utili a concessionarie o acquirenti per valutare correttamente un veicolo usato in base a marca, età, chilometraggio e alimentazione.

---

## Principali Risultati (Business Insights)
- Svalutazione Globale: Il valore delle auto subisce il calo più netto nei primi 5-6 anni di vita, per poi stabilizzarsi gradualmente.
- Cambio Automatico vs Manuale: Le auto con cambio automatico mantengono in media un valore di mercato significativamente più alto rispetto a quelle con cambio manuale.
- Impatto dell'Alimentazione: I veicoli elettrici e diesel mostrano prezzi mediani più elevati rispetto ai veicoli a benzina o CNG.

---

## Tecnologie Utilizzate
- Linguaggio: Python
- Librerie per l'Analisi: Pandas, NumPy
- Librerie per la Visualizzazione: Matplotlib, Seaborn

---

## Visualizzazioni Chiave
![Distribuzione dei Prezzi e Svalutazione](assets/grafici_auto.png)

---

## Fasi di Pulizia e Preparazione dei Dati (Data Cleaning)
1. Trattamento dei dati mancanti: Rimozione della colonna `reg_year` a causa di oltre il 70% di valori nulli; imputazione della mediana per la cilindrata (`engine_capacity(CC)`) raggruppata per marca.
2. Feature Engineering: Creazione delle variabili `car_age` (età del veicolo) e `km_per_year` (chilometri medi percorsi all'anno).
3. Conversione dei Tipi di Dato: Trattamento di anni e cilindrate come numeri interi (`int`) per ottimizzare la leggibilità e l'analisi.

---
