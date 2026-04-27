# 🚀 TP Java Jenkins Pipeline

## 🎯 Objectif
Mettre en place un pipeline CI avec Jenkins pour un projet Java Maven.

---

## 🛠️ Outils utilisés
- Java
- Maven
- Jenkins
- Docker
- GitHub

---

## ⚙️ Pipeline Jenkins

Le pipeline contient :

- Clone du dépôt GitHub  
- Build avec Maven  
- Tests  

---

## 🔄 Déclenchement automatique

✔️ Poll SCM utilisé :

H/1 * * * *


📌 Jenkins vérifie les changements chaque minute.

📌 Webhook non utilisé car Jenkins en localhost.

---

## 📸 Captures

### ✅ Jenkins Success
![Jenkins](captures/jenkins-success.png)

---

### 🖥️ Console Output
![Console](captures/console.png)

---

### ⚙️ Trigger (Poll SCM)
![Trigger](captures/trigger.png)

---

### 🌐 GitHub Repo
![GitHub](captures/github.png)

---

### 🐳 Docker Jenkins
![Docker](captures/docker.png)

---

## ✅ Résultat

✔️ Pipeline fonctionne correctement  
✔️ Build automatique après modification  
✔️ Tests exécutés avec succès  

---

## 👩‍💻 Auteur
IMANE FAIAD