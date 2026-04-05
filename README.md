# 🌊 Détection de déchets plastiques avec YOLOv8

![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python)
![YOLOv8](https://img.shields.io/badge/YOLOv8-Ultralytics-purple)
![mAP50](https://img.shields.io/badge/mAP50-80.2%25-brightgreen)
![Precision](https://img.shields.io/badge/Precision-66.6%25-yellow)
![Recall](https://img.shields.io/badge/Recall-71.4%25-yellow)
![License](https://img.shields.io/badge/License-MIT-green)

Détection automatique de déchets plastiques dans des images réelles à l'aide de **YOLOv8**, avec application à la surveillance environnementale (milieux naturels, zones marines, espaces verts).

---

## 🎯 Exemples de détection

### Détection en milieu marin

![Détection sac plastique sous-marin](images/detection_turtle.jpg)

> Détection d'un sac plastique avec une confiance de **0.91** en milieu sous-marin — cas critique pour la faune marine.

### Détection en milieu naturel terrestre

![Résultats de détection sur terrain](images/detection_results.png)

> Le modèle détecte plusieurs types de déchets (sacs, bouteilles, emballages) dans des environnements naturels variés avec bounding boxes.

---

## 📊 Résultats

| Métrique | Valeur |
|----------|--------|
| Precision (P) | **0.666** |
| Recall (R) | **0.714** |
| mAP50 | **0.802** |
| mAP50-95 | **0.669** |

> Un mAP50 de **0.802** indique que le modèle localise correctement les déchets dans plus de 80% des cas à un seuil IoU de 0.5.

---

## 📁 Structure du projet

```
plastic-detection-yolov8/
│
├── notebook/
│   └── train_yolo.ipynb        # Pipeline complet d'entraînement
├── data/
│   ├── train/
│   ├── valid/
│   └── test/
├── results/                    # Prédictions et métriques
├── images/                     # Exemples de détection
│   ├── detection_turtle.jpg
│   └── detection_results.png
├── architecture.jpg            # Architecture YOLOv8
├── requirements.txt
└── README.md
```

---

## ⚙️ Pipeline

```
Dataset Roboflow → Prétraitement → Entraînement YOLOv8 → Évaluation → Inférence
```

1. **Chargement du dataset** — images annotées depuis Roboflow
2. **Entraînement** — fine-tuning YOLOv8 sur les classes de déchets plastiques
3. **Évaluation** — calcul des métriques (P, R, mAP50, mAP50-95)
4. **Inférence** — détection sur nouvelles images

---

## 🗃️ Dataset

Dataset annoté disponible sur Roboflow :
[plastic-detection-pywxk](https://universe.roboflow.com/yolo-lnkrj/plastic-detection-pywxk)

---

## 🚀 Installation & Utilisation

```bash
# Cloner le dépôt
git clone https://github.com/khalil-ghanam/plastic-detection-yolov8.git
cd plastic-detection-yolov8

# Installer les dépendances
pip install -r requirements.txt

# Lancer le notebook
jupyter notebook notebook/train_yolo.ipynb
```

---

## 🛠️ Technologies

![Python](https://img.shields.io/badge/-Python-3776AB?logo=python&logoColor=white)
![YOLOv8](https://img.shields.io/badge/-YOLOv8-purple)
![OpenCV](https://img.shields.io/badge/-OpenCV-5C3EE8?logo=opencv&logoColor=white)
![Jupyter](https://img.shields.io/badge/-Jupyter-F37626?logo=jupyter&logoColor=white)

- **YOLOv8 (Ultralytics)** — modèle de détection d'objets en temps réel
- **OpenCV** — traitement et visualisation des images
- **Python / Jupyter Notebook** — pipeline d'entraînement et d'évaluation

---

## 👤 Auteur

**Khalil Ghanam**  
🎓 Étudiant en Intelligence Artificielle & Facteurs Humains — Université de Caen Normandie  
💼 Futur Data Scientist / ML Engineer  
📧 [ghanamkhalil8@gmail.com](mailto:ghanamkhalil8@gmail.com)  
🔗 [LinkedIn](https://www.linkedin.com/in/ghanamkhalil/)

---

## 📜 Licence

Projet sous licence MIT.
