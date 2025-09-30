# 🛰️ DeepPrez – Détection d’objets en télédétection avec Mask R-CNN

## 📌 Description

  projet de **deep learning** visant à développer une méthode rapide et précise de **détection d’objets dans des images de télédétection**. L’objectif est d’exploiter les images satellites haute résolution pour identifier et segmenter différents objets (avions, bateaux, véhicules, terrains sportifs, etc.), avec des applications en **sécurité, surveillance, robotique, diagnostic médical** et **cartographie environnementale**.

## 🗂️ Données

* **Dataset utilisé :** [NWPU VHR-10](https://github.com/chaozhong2010/NWPU-VHR-10-dataset)
* **Images positives :** 650 (contenant au moins un objet d’intérêt)
* **Images négatives :** 150
* **Classes cibles :** 10 (avion, bateau, réservoir, terrain de sport, port, pont, véhicule, etc.)
* **Prétraitement :** redimensionnement à 1024x1024, ajustement des bounding boxes, data augmentation (rotation, flip, contraste, bruit, etc.).

## 🤖 Méthodes

Plusieurs architectures ont été comparées :

* **YOLOv5 & YOLOv8** (Ultralytics, PyTorch) – détection rapide et optimisée pour l’inférence en temps réel.
* **Faster R-CNN** (ResNet-50 backbone, torchvision) – approche basée sur Region Proposal Network.
* **Mask R-CNN** – extension de Faster R-CNN permettant la **segmentation d’instances** pour une détection plus fine des objets.

## ⚙️ Entraînement

* Optimisateurs : **SGD / Adam**
* Batch size : 8–10
* Learning rate : 0.005–0.01 (avec scheduler)
* Epochs : 10–50
* Frameworks : **PyTorch, Torchvision, Ultralytics**

## 📈 Résultats

* Comparaison des performances (précision, rappel, mAP) entre YOLOv5, YOLOv8, Faster R-CNN et Mask R-CNN.
* Mask R-CNN offre la **meilleure segmentation et précision**, tandis que YOLOv8 se distingue par sa **rapidité** et son optimisation pour le temps réel.

## 🚀 Déploiement





