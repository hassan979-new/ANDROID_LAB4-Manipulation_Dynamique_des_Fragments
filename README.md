# Android Java – Gestion des Fragments

## 📖 Description
Ce projet Android Java illustre l’utilisation des **Fragments** pour créer une interface dynamique et réutilisable.  
L’application permet de basculer entre deux fragments :
- **FragmentOne** : affiche un texte et un bouton pour interagir.
- **FragmentTwo** : contient une barre de progression (`SeekBar`) et conserve son état lors des changements.

---

## 📂 Structure du projet
```
app/
└── src/
└── main/
├── java/com/example/fragmentslab/
│   ├── MainActivity.java
│   ├── FragmentOne.java
│   └── FragmentTwo.java
└── res/
    └── layout/
        ├── activity_main.xml
        ├── fragment_one.xml
        └── fragment_two.xml
```
---
## 📲 Installation de l’APK

Pour installer l’APK de ce projet Android :

1. **Compiler l’application**  
   - Ouvrir le projet dans **Android Studio**.  
   - Aller dans le menu **Build > Build Bundle(s) / APK(s) > Build APK(s)**.
   - <img width="960" height="540" alt="image" src="https://github.com/user-attachments/assets/f8013d07-8ca0-44f1-ba68-70147e031e22" />
   - Le fichier APK sera généré dans le dossier :  
     ```
     app/build/outputs/apk/debug/app-debug.apk
     ```
2. **Transférer l’APK sur votre appareil Android**  
   - Copier le fichier `app-debug.apk` sur votre smartphone (via câble USB, Bluetooth,...).  

3. **Autoriser les sources inconnues**  
   - Sur votre appareil Android, aller dans **Paramètres > Sécurité**.  
   - Activer l’option **Installer des applications depuis des sources inconnues**.  

4. **Installer l’APK**  
   - Ouvrir le fichier `app-debug.apk` sur votre smartphone.  
   - Suivre les instructions pour installer l’application.  

5. **Lancer l’application**  
   - Une fois installée, l’application sera disponible dans le menu des applications sous le nom **PizzaRecipes**.
  
  
---

## ⚙️ Fonctionnalités
- **MainActivity** :
  - Contient deux boutons pour charger les fragments.
  - Méthode `replaceFragment()` pour remplacer dynamiquement le fragment affiché.
  - Gestion du `BackStack` pour naviguer entre les fragments.

- **FragmentOne** :
  - Affiche un `TextView` et un bouton.
  - Lors du clic, le texte change en : *"Bonjour depuis Fragment 1 !"*.
  - Journalisation du cycle de vie (`onResume`, `onPause`).

- **FragmentTwo** :
  - Affiche un `SeekBar` et un `TextView` indiquant la valeur.
  - Sauvegarde et restauration de l’état (`onSaveInstanceState`).
  - Mise à jour dynamique du texte lors du déplacement du curseur.

---

## 🖥️ Exemple d’exécution


---

## 💡 Concepts pratiqués
- Utilisation des **Fragments** pour modulariser l’interface.
- Gestion du cycle de vie des fragments (`onResume`, `onPause`).
- Sauvegarde/restauration de l’état avec `Bundle`.
- Navigation dynamique avec `FragmentManager` et `FragmentTransaction`.
- Interaction utilisateur via `Button` et `SeekBar`.

---

## 🧑‍💻 Auteur
👤 **Agouram Hassan**  
📱 Développement Android Java  
🎓 Instructor : **Mr. LACHGAR**  
📅 14 Mars 2026
