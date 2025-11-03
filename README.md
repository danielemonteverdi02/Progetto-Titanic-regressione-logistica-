# Progetto-Titanic-regressione-logistica-

ANALISI E PREDIZIONE DELLA SOPRAVVIVENZA DEI PASSEGGERI DEL TITANIC

DESCRIZIONE DEL PROGETTO:

Questo progetto si propone di analizzare e predire la sopravvivenza dei passeggeri del Titanic utilizzando tecniche di machine learning. L’obiettivo principale è costruire un modello predittivo accurato basato sulle caratteristiche dei passeggeri e su nuove feature ottenute tramite feature engineering.

IL PROGETTO COMPRENDE LE SEGUENTI FASI:

Pulizia dei dati e gestione dei valori mancanti (imputazione singola e tramite MICE).

Feature engineering per estrarre informazioni aggiuntive dai dati originali.

Codifica delle variabili categoriche con one-hot encoding e scalatura delle variabili numeriche.

Addestramento di un modello di regressione logistica con cross-validation.

Valutazione delle performance su un validation set.

Predizione finale sul test set fornito da Kaggle.

DATASET

Il dataset utilizzato è quello ufficiale di Kaggle del Titanic, suddiviso in due gruppi principali:

Training set (train.csv): include le informazioni sui passeggeri e l’esito (survival), da utilizzare per addestrare il modello.

Test set (test.csv): contiene le caratteristiche dei passeggeri senza indicazione della sopravvivenza; serve per valutare le predizioni del modello.


VARIABILI:

survival	Sopravvivenza	0 = No, 1 = Sì
pclass	Classe del biglietto	1 = Prima, 2 = Seconda, 3 = Terza (proxy per lo status socioeconomico)
sex	Sesso	Maschio/Femmina
age	Età in anni	Se stimata, può essere frazionaria (es. 0.5)
sibsp	Numero di fratelli/coniugi a bordo	
parch	Numero di genitori/figli a bordo	Alcuni bambini viaggiavano solo con la tata
ticket	Numero del biglietto	
fare	Prezzo del biglietto	
cabin	Numero della cabina	
embarked	Porto di imbarco	C = Cherbourg, Q = Queenstown, S = Southampton

METODOLOGIA

Pulizia dei dati: gestione dei valori mancanti, correzione di anomalie e normalizzazione dei dati.

Imputazione dei valori mancanti: sia imputazione singola che tramite MICE (Multiple Imputation by Chained Equations).

Feature Engineering: creazione di nuove variabili utili per migliorare le performance del modello.

Codifica e scalatura: trasformazione delle variabili categoriche in dummy variables e scalatura dei dati numerici.

Modello predittivo: regressione logistica con 10-fold cross-validation per ottimizzare i parametri e valutare le performance.

Valutazione: metriche utilizzate includono accuracy, precision, recall, F1-score e ROC AUC.

Predizione finale: applicazione del modello addestrato sul test set per generare il file di submission.

RISULTATI

Accuracy media in cross-validation: 0.81 ± 0.04

Precision media: 0.75 ± 0.07

Recall media: 0.78 ± 0.03

F1-score: 0.76 ± 0.04

ROC AUC: 0.86 ± 0.03

Sul validation set, il modello ottiene un’accuracy del 0.79, confermando la buona capacità predittiva del modello anche su dati non visti durante l’addestramento.

CONCLUSIONI

Il modello mostra buone performance sia nella cross-validation che sul validation set, riuscendo a catturare in modo efficace i passeggeri sopravvissuti pur mantenendo un buon equilibrio tra precision e recall. Eventuali miglioramenti futuri potrebbero includere l’uso di modelli più complessi, tecniche di bilanciamento delle classi o ulteriori strategie di feature engineering.
