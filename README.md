# fieldshift-nasa-space-apps
# 🌱 FieldShift — Cultiver demain, une saison d'avance

> **L’observation de la Terre au service de vos décisions agricoles.**  
> *NASA Space Apps Challenge 2026*

---

## 📋 Aperçu du projet (Overview)

**FieldShift** est une plateforme web d’aide à la décision agricole propulsée par les données d’observation de la Terre de la **NASA** et l’intelligence artificielle générative (**Google Gemini**). 

Conçu pour les exploitants agricoles confrontés au stress hydrique et aux aléas climatiques, FieldShift transforme des données satellites brutes (humidité du sol, indice de végétation NDVI, précipitations et anomalies thermiques) en recommandations agronomiques claires, exploitables parcelle par parcelle.

### 🎥 Démonstration (Demo)
* 📄 **Présentation (Slides PDF) :** [Voir la présentation FieldShift](./FieldShift_Demo.pdf) 
* 🎬 **Vidéo de démonstration
* 

---

## ✨ Fonctionnalités principales

* **🗺️ Vue d’ensemble & Carte interactive des parcelles :** Suivi en temps réel de la surface exploitée, de l’humidité du sol (`%`), de la température moyenne et de l’indice de santé végétale (`NDVI`).
* **🔄 Planificateur intelligent de rotations culturales :** Recommandations pluriannuelles (ex. alternance *Blé dur → Pois chiche → Orge*) permettant de réduire jusqu’à **18 % des besoins en eau** tout en enrichissant naturellement les sols en azote.
* **📊 Simulateur climatique & hydrique :** Modélisation interactive de scénarios de sécheresse (déficit pluviométrique et hausse des températures) pour anticiper les besoins en irrigation et les rendements.
* **🛰️ Intégration des données satellites NASA :**
  * **NASA POWER :** Données agro-climatiques (températures, précipitations, évapotranspiration $ET_0$).
  * **NASA SMAP :** Humidité superficielle du sol.
  * **NASA MODIS :** Indice de végétation normalisé (`NDVI`).
* **🤖 Assistant FieldShift (IA contextuelle) :** Chatbot agronomique connecté au contexte de la parcelle sélectionnée et aux analyses météo locales, propulsé par **Laravel** et l’**API Gemini**.

---

## 🛠️ Architecture technique

* **Frontend :** HTML5, CSS3 (Design System sur mesure), JavaScript Vanilla, Cartographie vectorielle SVG interactive.
* **Backend :** PHP / **Laravel** (API RESTful, gestion du contexte parcellaire et sécurisation des appels IA).
* **Data & Traitement météo :** **Python** (`analyse.py`) pour l'extraction et la structuration des séries temporelles de pluie et de température au format JSON (`insights_chatbot.json`).
* **Intelligence Artificielle :** **Google Gemini API** (`gemini-2.5-flash`).

---

## 🚀 Installation et démarrage rapide

### Prérequis
* PHP >= 8.1 & Composer
* Python >= 3.9
* Une clé API gratuite [Google AI Studio (Gemini)](https://aistudio.google.com/)


