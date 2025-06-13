# 📋 Mini-application ToDo List (Vue 3 + FastAPI)

Projet réalisé dans le cadre du test technique "Alternant Master Dev Informatique".

## 🎯 Objectif

Développer une mini-application web de gestion de tâches (ToDo List) en fullstack :

✅ Backend en Python / FastAPI  
✅ Frontend en Vue.js 3  

## ⚙️ Fonctionnalités

- Création de tâche
- Liste des tâches
- Filtre par catégorie
- Filtre par priorité
- Affichage des tâches urgentes (< 2 jours) en rouge
- Suppression de tâche
- Feedback utilisateur

## 🏗️ Architecture

### Backend (FastAPI)

- API RESTful
- Validation avec Pydantic
- CORS activé pour le Frontend
- Routes :
  - `GET /tasks`
  - `POST /tasks`
  - `GET /tasks/{id}`
  - `PUT /tasks/{id}`
  - `DELETE /tasks/{id}`
  - `GET /categories`

### Frontend (Vue 3 + Axios)

- Composants :
  - `TaskForm.vue` → création de tâche
  - `TaskList.vue` → affichage & suppression
- Communication avec l'API via Axios
- Filtres dynamiques
- UX fluide avec feedback utilisateur

## 🚀 Lancement du projet

### Prérequis

- Node.js + npm
- Python 3 + FastAPI

### Démarrer le backend

```bash
cd backend
python -m venv venv
# Activation venv Windows :
.\venv\Scripts\Activate
pip install -r requirements.txt (ou installer manuellement fastapi uvicorn pydantic)
uvicorn main:app --reload
