# 📊 Diagrammes UML - Sprint 1 SmartTransport

## 📁 Fichiers fournis

Ce dossier contient tous les diagrammes UML nécessaires pour le **Chapitre 3** de votre rapport PFE :

### 1️⃣ **Diagramme de Classes** (`diagramme_classes_sprint1.drawio`)
- Classe Passager
- Classe Reclamation
- Classe Preuve
- Énumérations : TypeTransport, StatutReclamation, TypePreuve
- Relations et cardinalités

### 2️⃣ **Diagrammes de Séquence**

#### `sequence_inscription.drawio` - US1 : Inscription
- Flux complet d'inscription d'un passager
- Vérification email
- Hashage mot de passe
- Génération JWT

#### `sequence_authentification.drawio` - US2 : Authentification
- Connexion avec email/password
- Vérification des credentials
- Génération token
- Gestion des erreurs (alt frame)

#### `sequence_soumettre_reclamation.drawio` - US5, US6, US7
- Remplissage formulaire
- Upload de photo
- Compression image
- Sauvegarde en base de données
- Stockage fichier

---

## 🚀 Comment utiliser ces fichiers

### **Méthode 1 : Draw.io en ligne (RECOMMANDÉ)**

1. Allez sur **https://app.diagrams.net/**
2. Cliquez sur **"Open Existing Diagram"**
3. Sélectionnez le fichier `.drawio` que vous voulez ouvrir
4. Le diagramme s'affiche immédiatement ✅

### **Méthode 2 : Draw.io Desktop**

1. Téléchargez Draw.io Desktop : https://github.com/jgraph/drawio-desktop/releases
2. Installez l'application
3. Lancez Draw.io
4. **File → Open** → Sélectionnez le fichier `.drawio`

---

## 📸 Exporter en image (pour votre rapport LaTeX)

### **Export PNG (recommandé pour LaTeX)**

1. Ouvrez le diagramme dans Draw.io
2. **File → Export as → PNG...**
3. Paramètres recommandés :
   - ✅ **Zoom: 100%**
   - ✅ **Border Width: 5**
   - ✅ **Transparent Background: Non** (fond blanc)
   - ✅ **Include a copy of my diagram: Oui** (pour pouvoir le modifier plus tard)
4. Cliquez **Export**
5. Sauvegardez dans votre dossier `figures/` du projet LaTeX

### **Export PDF (alternative)**

1. **File → Export as → PDF...**
2. ✅ **Fit to: 1 page**
3. **Export**

---

## 📝 Intégration dans LaTeX

### **Code LaTeX pour insérer un diagramme :**

```latex
\begin{figure}[h]
\centering
\includegraphics[width=0.85\textwidth]{figures/diagramme_classes_sprint1.png}
\caption{Diagramme de classes - Sprint 1}
\label{fig:classes_sprint1}
\end{figure}
```

### **Pour les diagrammes de séquence (plus larges) :**

```latex
\begin{figure}[h]
\centering
\includegraphics[width=1.0\textwidth]{figures/sequence_inscription.png}
\caption{Diagramme de séquence - Inscription passager}
\label{fig:seq_inscription}
\end{figure}
```

---

## ✏️ Modifier les diagrammes

Les fichiers `.drawio` sont **complètement éditables** :

### **Pour modifier un élément :**
1. Double-cliquez sur l'élément (texte, forme, flèche)
2. Modifiez le contenu
3. Cliquez en dehors pour valider

### **Pour ajouter un élément :**
1. Utilisez la palette de gauche
2. Glissez-déposez la forme souhaitée
3. Connectez avec des flèches

### **Conseils d'édition :**
- **Ctrl + D** : Dupliquer un élément
- **Ctrl + Z** : Annuler
- **Ctrl + Shift + L** : Aligner automatiquement
- **Alt + Shift + Flèches** : Déplacer finement

---

## 🎨 Personnalisation

### **Changer les couleurs :**
1. Sélectionnez l'élément
2. Panneau de droite → **Style**
3. Choisissez **Fill** (remplissage) et **Line** (contour)

### **Changer la police :**
1. Sélectionnez le texte
2. Panneau de droite → **Text**
3. Modifiez **Font Family** et **Size**

---

## 📋 Diagrammes de séquence manquants (à créer vous-même)

Pour compléter votre Chapitre 3, vous devrez créer ces diagrammes supplémentaires :

### **À créer :**
- ✅ Réinitialisation mot de passe (US3)
- ✅ Modification profil (US4)
- ✅ Consulter historique (US8)
- ✅ Suivre état réclamation (US9)

### **Comment les créer rapidement :**
1. Ouvrez `sequence_authentification.drawio` (le plus simple)
2. **File → Save As** → Nouveau nom (ex: `sequence_modifier_profil.drawio`)
3. Modifiez le titre
4. Adaptez les messages selon la logique de l'US
5. Exportez en PNG

**Astuce** : Dupliquez et adaptez plutôt que de tout refaire !

---

## 🆘 Problèmes courants

### **Le fichier ne s'ouvre pas dans Draw.io**
→ Assurez-vous d'utiliser **app.diagrams.net** (et non une ancienne version)

### **Les flèches ne se connectent pas**
→ Zoomez à 100% et assurez-vous de bien viser les points de connexion (petits cercles bleus)

### **Export PNG trop petit/grand**
→ Modifiez le **Zoom** dans les options d'export (100% = taille normale)

### **Le texte est coupé dans l'export**
→ Augmentez **Border Width** à 10 ou 15

---

## 📚 Ressources utiles

- **Tutoriel Draw.io (vidéo)** : https://www.youtube.com/results?search_query=drawio+uml+tutorial
- **Documentation UML** : https://www.uml-diagrams.org/
- **Guide des diagrammes de séquence** : https://www.uml-diagrams.org/sequence-diagrams.html

---

## ✅ Checklist avant de rendre votre rapport

- [ ] Tous les diagrammes exportés en PNG haute qualité (300 DPI)
- [ ] Fichiers PNG dans le dossier `figures/` de LaTeX
- [ ] Légendes (\caption) claires et numérotées
- [ ] Labels (\label) pour pouvoir référencer (ex: "voir Figure \ref{fig:classes_sprint1}")
- [ ] Diagrammes cohérents avec le texte du rapport
- [ ] Orthographe et français corrects dans les diagrammes

---

## 💡 Conseils pour un rapport professionnel

1. **Alignez tout** : Utilisez Ctrl+Shift+L pour aligner automatiquement
2. **Couleurs cohérentes** : Utilisez les mêmes couleurs dans tous vos diagrammes
3. **Police lisible** : Arial ou Helvetica, taille 10-12
4. **Pas de chevauchement** : Espacez bien les éléments
5. **Notes explicatives** : Ajoutez des notes (forme "Note") pour clarifier

---

## 📧 Contact

Si vous avez des questions ou besoin d'aide pour créer les diagrammes manquants, n'hésitez pas à demander !

Bon courage pour votre PFE ! 🚀

---

**Auteur** : Diagrammes créés pour le projet SmartTransport
**Date** : Février 2026
**Sprint** : Sprint 1 - Authentification et Soumission de réclamations
