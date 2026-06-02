# Guide d'ajout des photos - SO COIF'

## 📸 Comment ajouter vos photos à la galerie

### Étape 1 : Préparez vos images
1. Prenez ou sélectionnez vos photos
2. Redimensionnez-les à une taille web standard (ex: 800x800px)
3. Optimisez-les pour le web (JPG ou PNG)

### Étape 2 : Nommez vos images
Nommez vos photos comme ceci dans le dossier `/images` :
- `photo1.jpg` - Photo principale du salon (grande, 2x2)
- `photo2.jpg` - Coupe avant/après
- `photo3.jpg` - Coloration
- `photo4.jpg` - Mise en forme boucles (large, 2 colonnes)
- `photo5.jpg` - Soin profond
- `photo6.jpg` - Blond spécial

### Étape 3 : Placez-les dans le dossier images
```
so-coif/
├── images/
│   ├── photo1.jpg
│   ├── photo2.jpg
│   ├── photo3.jpg
│   ├── photo4.jpg
│   ├── photo5.jpg
│   └── photo6.jpg
├── index.html
└── ...
```

### Étape 4 : Vérifiez le résultat
Allez sur `https://socoif.com` (ou `.fr`) et vérifiez que les photos s'affichent dans la galerie !

---

## 🎨 Recommandations pour les photos

- **Format** : JPG (photos) ou PNG (si transparence)
- **Taille** : 800x800px minimum, 1200x1200px optimal
- **Poids** : < 500KB par image (pour une charge rapide)
- **Qualité** : 85-90% pour JPG

### Outils gratuits pour optimiser les images :
- [TinyPNG](https://tinypng.com) - Compression
- [Pixlr](https://pixlr.com) - Redimensionnement
- [Imgbot](https://www.imgbot.ai) - Auto-optimisation

---

## 🔄 Modifier la galerie dans le code

Si vous voulez changer l'ordre ou ajouter/retirer des photos, éditez le fichier `index.html` :

Cherchez la section "GALERIE PHOTOS" dans le JavaScript et modifiez le tableau `photos` :

```javascript
const photos = [
  { src: 'images/photo1.jpg', title: 'Votre titre', span: 2, row: 2 },
  { src: 'images/photo2.jpg', title: 'Votre titre', span: 1 },
  // Ajoutez/modifiez selon vos besoins
];
```

- `src` : Chemin vers l'image
- `title` : Titre de la photo (visible au survol)
- `span` : 1 = normal, 2 = large (2 colonnes)
- `row` : 1 = normal, 2 = haut (2 rangées) - seulement pour photo1

---

## ✅ Vous êtes prêt !

Une fois les images placées, le site affichera votre galerie automatiquement ! 🎉

Pour d'autres questions, consultez la documentation de Vercel ou relancez le développement.
