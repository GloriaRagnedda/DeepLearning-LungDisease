# LungDiseaseNet

**LungDiseaseNet** è un progetto di deep learning per la classificazione automatica di malattie polmonari a partire da immagini radiografiche. L'obiettivo è sviluppare un sistema diagnostico intelligente in grado di distinguere tra tre diverse condizioni polmonari:

- **Normal**: pazienti sani
- **Viral Pneumonia**: casi di polmonite virale
- **Lung Opacity**: include condizioni patologiche con opacità nei polmoni (es. COVID-19)
---

## Dataset

Il dataset utilizzato è disponibile su Kaggle:  
- [Lung Disease Dataset - Kaggle](https://www.kaggle.com/datasets/fatemehmehrparvar/lung-disease)

---
## Installazione

### Requisiti:

- Account Kaggle
- Account Google (per Google Drive e Google Colab)

### Istruzioni:

1. Accedere a [kaggle.com](https://www.kaggle.com) e scaricare il file `kaggle.json` dalle impostazioni dell’account (impostazioni -> sezione API -> _Create_ _a_ _new_ _token_);
2. Scaricare i Notebook da GitHub (`cnn.ipynb`, `resnet.ipynb`, `vgg16.ipynb`) e caricarli in una cartella su Google Drive;
3. Aprire la cartella con i file caricati e inserire il file 'kaggle.json' scaricato nel punto 1;
4. Procedere con l’addestramento dei modelli e l’analisi dei risultati;

---

## Modelli Implementati

| Modello      | Descrizione                                                                           |
|--------------|----------------------------------------------------------------------------------------|
| CNN Semplice | Una rete convoluzionale costruita da zero per la classificazione delle immagini       |
| ResNet50     | Architettura ResNet50 con possibilità di fine-tuning e utilizzo dei pesi preaddestrati |
| VGG16        | Architettura VGG16 preaddestrata con livelli fully connected personalizzati            |

---

## Librerie Utilizzate

| Libreria              | Funzione                                                                          |
|-----------------------|------------------------------------------------------------------------------------|
| `Tensorflow/Keras`    | Costruzione e addestramento dei modelli                                            |
| `OpenDatasets`        | Download automatico del dataset da Kaggle                                          |
| `Numpy, Pandas`       | Analisi e manipolazione dei dati                                                   |
| `Matplotlib, Seaborn` | Visualizzazione dei dati e delle performance (grafici, confusion matrix)           |
| `cv2, PIL`            | Preprocessing e gestione delle immagini                                            |
| `scikit-learn`        | Creazione di matrici di confusione e valutazione con metriche                      |

---

## Riferimenti

- Dataset: [Lung Disease - Kaggle](https://www.kaggle.com/datasets/fatemehmehrparvar/lung-disease)
- Librerie: TensorFlow, Keras, OpenDatasets, Scikit-Learn, Matplotlib, Seaborn

---
