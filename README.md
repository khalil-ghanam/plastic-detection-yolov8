#  Détection de plastique avec YOLOv8

##  Description

Ce projet utilise YOLOv8 pour détecter des déchets plastiques dans des images.

---

##  Structure du projet

* `data/` : dataset (train, validation, test)
* `notebooks/` : notebook d'entraînement
* `results/` : résultats de détection

---

##  Notebook

Le pipeline complet (prétraitement, entraînement, évaluation) est disponible ici :
 `src/train_yolo.ipynb`
 `src/train_yolo.py`

---

##  Résultats

*  Precision (P): 0.666 
*  Recall (R): 0.714
*  mAP50: 0.802 
*  mAP50-95: 0.669  

---

##  Exemples

`results/`

---

##  Dataset

Dataset utilisé :
https://universe.roboflow.com/yolo-lnkrj/plastic-detection-pywxk

---

##  Installation

```bash
pip install -r requirements.txt
```

---

## Technologies

* Python
* YOLOv8 (Ultralytics)
* OpenCV
