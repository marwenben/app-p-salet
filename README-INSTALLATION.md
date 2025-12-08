# 🕌 APPLICATION HORAIRES DE PRIÈRE - VERSION FINALE

## ✅ FONCTIONNALITÉS COMPLÈTES

### 1. 🔔 **Notifications Automatiques**
- Notifications push pour chaque prière
- Adhan (appel à la prière) joue automatiquement
- Configuration individuelle pour chaque prière
- Volume ajustable

### 2. 📖 **Coran Bilingue**
- Texte arabe complet (114 sourates)
- Traduction française complète
- Affichage côte à côte ou séparé
- Navigation facile par sourate

### 3. 🌙 **Calendrier Ramadan avec Notes**
- Calendrier complet du mois de Ramadan
- Ajout de notes pour chaque jour
- Sauvegarde automatique des notes
- Notes persistantes (localStorage)

### 4. 🧭 **Direction Qibla**
- Boussole précise vers La Mecque
- Utilise la géolocalisation
- Affichage de la distance

### 5. 📿 **Tasbih Électronique**
- Compteur de dhikr
- Objectifs configurables (33, 99)
- Vibration au tap

### 6. 🌍 **Multi-villes**
- Plus de 25 villes disponibles
- Affichage simultané de 2 villes
- Horaires précis selon la méthode locale

### 7. 🌤️ **Méteo Temps Réel**
- Intégration Open-Meteo API
- Météo pour chaque prière
- Mise à jour automatique

### 8. 📱 **PWA Installable**
- Installation sur mobile/desktop
- Fonctionne hors ligne
- Icônes HD 192px et 512px

---

## 📥 INSTALLATION SUR GITHUB PAGES

### ÉTAPE 1: Préparer les fichiers

```
1. Téléchargez TOUS les fichiers du dossier "app-salat-final"
2. Décompressez si nécessaire
```

### ÉTAPE 2: Upload sur GitHub

```
1. GitHub → Votre repo "marwenben/app-Salet"
2. Supprimez TOUS les anciens fichiers
3. Uploadez TOUS les nouveaux fichiers:
   - index.html
   - script.js
   - style.css
   - manifest.json
   - service-worker.js
   - icon-192.png
   - icon-512.png
   - adhan1.mp3
   - fajr-bg.jpg
   - dhuhr-bg.jpg
   - asr-bg.jpg
   - maghrib-bg.jpg
   - isha-bg.jpg
   - ramadan.gif
   - ramadan.mp4
```

### ÉTAPE 3: Vérifier le déploiement

```
1. Attendez 3-5 minutes
2. GitHub Actions doit être en succès
3. Allez sur: https://marwenben.github.io/app-Salet/
4. Ctrl+Shift+Delete → Vider TOUT le cache
5. Rechargez la page
```

---

## ✅ TEST DES FONCTIONNALITÉS

### 1. Tester les Notifications

```
1. Cliquez sur 🔔 Notifications (en haut)
2. Cliquez "Autoriser les notifications du navigateur"
3. Acceptez dans le popup du navigateur
4. Cochez les prières désirées (Fajr, Dhuhr, etc.)
5. Cliquez "🔊 Tester l'Adhan"
6. Vous devez entendre l'adhan !
```

### 2. Tester le Coran Bilingue

```
1. Cliquez sur 📖 Coran
2. Sélectionnez une sourate
3. Choisissez "Arabe seul", "Français seul", ou "Arabe + Français"
4. Cliquez "Charger"
5. Les versets apparaissent avec traduction !
```

### 3. Tester les Notes Ramadan

```
1. Cliquez sur le compte à rebours Ramadan
2. Cliquez sur un jour du calendrier
3. Tapez une note (ex: "Jeûne terminé 18h30")
4. La note est sauvegardée automatiquement
5. Rechargez la page → La note est toujours là !
```

### 4. Installation PWA

```
Android Chrome:
- Bouton "📱 Installer l'Application" apparaît après 5-10 secondes
- OU Menu ⋮ → "Installer l'application"

iOS Safari:
- Bouton Partage 📤
- "Sur l'écran d'accueil"
```

---

## 🔧 PARAMÈTRES GITHUB (IMPORTANT)

### Vérifiez ces paramètres:

```
Settings → Actions → General → Workflow permissions
→ Sélectionnez "Read and write permissions"
→ Cliquez "Save"
```

### GitHub Pages:

```
Settings → Pages
→ Source: "Deploy from a branch"
→ Branch: "main" (ou "master")
→ Folder: "/ (root)"
→ Save
```

---

## 🚨 RÉSOLUTION DE PROBLÈMES

### Problème: "Failed to get ID Token"

```
Solution:
Settings → Actions → General → Workflow permissions
→ "Read and write permissions" → Save
Puis relancez le workflow
```

### Problème: PWA ne s'installe pas

```
1. Vérifiez que manifest.json est accessible:
   https://marwenben.github.io/app-Salet/manifest.json
   
2. Vérifiez les icônes:
   https://marwenben.github.io/app-Salet/icon-192.png
   https://marwenben.github.io/app-Salet/icon-512.png
   
3. Si erreur 404 → Chemins incorrects dans les fichiers
```

### Problème: Horaires ne s'affichent pas

```
1. F12 → Console → Vérifiez les erreurs
2. Si "Script error" → Videz le cache complètement
3. Essayez en navigation privée
4. Vérifiez que script.js est chargé
```

### Problème: Notifications ne marchent pas

```
1. Vérifiez que vous avez autorisé les notifications
2. Chrome → Paramètres → Confidentialité → Paramètres du site
   → Notifications → Vérifiez que le site est autorisé
3. Testez avec "🔊 Tester l'Adhan"
```

### Problème: Notes Ramadan ne se sauvegardent pas

```
1. Vérifiez que localStorage est activé
2. Mode navigation privée → localStorage ne fonctionne PAS
3. Essayez en mode normal
```

---

## 📊 STRUCTURE DES FICHIERS

```
app-Salet/
├── index.html              (Page principale)
├── script.js               (Logique complète)
├── style.css               (Styles)
├── manifest.json           (Configuration PWA)
├── service-worker.js       (Service Worker)
├── icon-192.png            (Icône 192x192)
├── icon-512.png            (Icône 512x512)
├── adhan1.mp3              (Audio adhan)
├── fajr-bg.jpg             (Image Fajr)
├── dhuhr-bg.jpg            (Image Dhuhr)
├── asr-bg.jpg              (Image Asr)
├── maghrib-bg.jpg          (Image Maghrib)
├── isha-bg.jpg             (Image Isha)
├── ramadan.gif             (Animation Ramadan)
└── ramadan.mp4             (Vidéo Ramadan)
```

---

## 🎯 LISTE DE VÉRIFICATION FINALE

Avant de déclarer que tout fonctionne, vérifiez:

- [ ] Site accessible sur https://marwenben.github.io/app-Salet/
- [ ] Horaires s'affichent pour Montréal et Tunis
- [ ] Heure locale fonctionne
- [ ] Météo s'affiche
- [ ] Notifications peuvent être activées
- [ ] Test adhan fonctionne
- [ ] Coran arabe charge
- [ ] Coran français charge
- [ ] Affichage bilingue fonctionne
- [ ] Calendrier Ramadan s'ouvre
- [ ] Notes peuvent être ajoutées
- [ ] Notes sont sauvegardées après rechargement
- [ ] Tasbih fonctionne
- [ ] Qibla détecte la position
- [ ] PWA peut être installée
- [ ] Icône d'installation apparaît

---

## 💡 CONSEILS D'UTILISATION

### Pour les notifications:

1. Activez les notifications dès la première visite
2. Cochez toutes les prières que vous voulez
3. Testez d'abord avec "🔊 Tester l'Adhan"
4. L'adhan joue automatiquement à l'heure de la prière

### Pour le Coran:

1. Commencez par Al-Fatiha (sourate 1)
2. Utilisez le mode bilingue pour apprendre
3. Faites défiler pour voir tous les versets
4. Changez de sourate avec le sélecteur en haut

### Pour les notes Ramadan:

1. Cliquez sur le compte à rebours Ramadan
2. Cliquez sur n'importe quel jour
3. Tapez votre note (iftar, tarawih, objectifs, etc.)
4. La note est sauvegardée instantanément
5. Les notes restent même après avoir fermé le navigateur

---

## 🆘 SUPPORT

Si vous rencontrez des problèmes:

1. Vérifiez cette documentation
2. Consultez F12 → Console pour les erreurs
3. Videz le cache complètement
4. Essayez en navigation privée
5. Vérifiez que tous les fichiers sont uploadés

---

## 🎉 FÉLICITATIONS !

Vous avez maintenant une application complète de prière avec :
- Notifications automatiques
- Coran bilingue
- Calendrier Ramadan personnalisé
- Et bien plus !

**بارك الله فيكم** 🤲

**Qu'Allah accepte vos prières** 🕌
