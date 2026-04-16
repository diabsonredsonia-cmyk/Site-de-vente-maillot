# 📚 GUIDE UTILISATION - MAILLOTS VINTAGE

## 📁 Structure des fichiers

Tu as **2 fichiers distincts**:

```
projet/
├── index.html      (← le squelette / contenu)
└── styles.css      (← les couleurs / mise en page)
```

---

## 🎯 Qu'est-ce que c'est?

### **index.html**
C'est le fichier **HTML pur** = juste la structure, les textes et les images
- Les textes: "Maillots Vintage", "Chelsea 2005", etc.
- Les boutons et les images
- **Pas de couleurs, pas de design**

### **styles.css**
C'est le fichier **CSS** = les couleurs, les espacements et la mise en page
- Les couleurs: or (#C9A84C), noir (#06080f), etc.
- La taille des textes (font-size)
- L'espacement (padding, gap)
- **Les animations et les transitions**

---

## 🚀 Comment utiliser?

### **Étape 1: Télécharge les 2 fichiers**
- `index.html`
- `styles.css`

### **Étape 2: Mets-les dans le même dossier**
```
mon-projet/
├── index.html
└── styles.css   ← même dossier!
```

### **Étape 3: Ouvre index.html dans le navigateur**
Double-clique sur `index.html` → ça s'ouvre dans le navigateur!

---

## ✏️ Comment MODIFIER?

### **Tu veux changer le texte?**
→ Modifie `index.html`

Exemple: Changer "Chelsea 2005" en "PSG 1996"
```html
<!-- AVANT -->
<h3 class="maillot-title">Chelsea 2005</h3>

<!-- APRÈS -->
<h3 class="maillot-title">PSG 1996</h3>
```

### **Tu veux changer les couleurs?**
→ Modifie `styles.css`

Exemple: Changer la couleur or en bleu
```css
/* Cherche #C9A84C et remplace par ta couleur */
.hero-label {
    color: #C9A84C;  ← Couleur or
}

/* Devient */
.hero-label {
    color: #3A9FE8;  ← Couleur bleu
}
```

### **Tu veux changer la taille du titre?**
→ Modifie `styles.css`

```css
.hero-title {
    font-size: 3.2rem;  ← Grande taille
}

/* Réduis à */
.hero-title {
    font-size: 2.5rem;  ← Taille moyenne
}
```

---

## 🎨 Les couleurs principales

Voici les couleurs utilisées. Tu peux les changer:

```css
#C9A84C   = Or (Logo, CTA, accents)
#06080F   = Noir profond (Fond)
#E8E4DF   = Beige (Textes principaux)
#6B6A70   = Gris (Textes secondaires)
#0F1419   = Bleu très foncé (Gradients)
#1A2433   = Bleu foncé (Gradients)
```

---

## 📝 MODIFICATIONS COURANTES

### Ajouter une image à la place du emoji 👕

**Dans `index.html`, remplace:**
```html
<!-- ❌ AVANT (emoji) -->
<div class="maillot-image" style="background: linear-gradient(135deg, #1A2C4E, #0F1419); color: #C9A84C;">👕</div>

<!-- ✅ APRÈS (image réelle) -->
<img src="images/chelsea-2005.jpg" alt="Chelsea 2005" class="maillot-image-img">
```

**Puis dans `styles.css`, ajoute:**
```css
.maillot-image-img {
    width: 100%;
    height: 300px;
    object-fit: cover;
    border-radius: 4px;
}
```

---

### Ajouter un prix

**Dans `index.html`, ajoute une ligne:**
```html
<h3 class="maillot-title">Chelsea 2005</h3>
<p class="maillot-price">25 000 FCFA</p>  ← Ajoute ça
<p class="maillot-subtitle">Edition rare • Disponible</p>
```

**Dans `styles.css`, ajoute:**
```css
.maillot-price {
    color: #C9A84C;
    font-size: 16px;
    font-weight: 500;
    margin: 0;
}
```

---

## 🔗 Mettre à jour les liens des boutons

**Dans `index.html`:**
```html
<!-- Avant -->
<button class="btn-primary">Découvrir la collection</button>

<!-- Après (avec lien) -->
<a href="collection.html" class="btn-primary">Découvrir la collection</a>
```

---

## 🎯 RÉSUMÉ RAPIDE

| Besoin | Où modifier | Exemple |
|--------|------------|---------|
| Changer texte | `index.html` | "Maillots Vintage" → "Collection Rare" |
| Changer couleur | `styles.css` | #C9A84C → #E84040 |
| Changer taille texte | `styles.css` | font-size: 3.2rem → 2rem |
| Ajouter image | `index.html` | Remplacer emoji par `<img>` |
| Ajouter prix | `index.html` | Ajouter une nouvelle `<p>` |
| Changer bouton | `index.html` | Modifier le texte ou le lien |

---

## ❓ Questions courantes

### Q: Je change quelque chose mais ça ne s'affiche pas?
**R:** Appuie sur **Ctrl+Shift+R** (ou Cmd+Shift+R sur Mac) pour vider le cache du navigateur.

### Q: Comment voir les changements en direct?
**R:** Installe une extension comme **Live Server** sur VS Code. Ça reload automatiquement!

### Q: Je veux changer le layout (organisation)?
**R:** C'est dans `styles.css`:
- `display: grid` = grille
- `gap: 1rem` = espacement entre éléments
- `grid-template-columns: 1fr 1fr` = 2 colonnes

---

## 🚀 Prochaines étapes

1. **Remplace les emoji 👕** par des vrais images
2. **Change les noms des maillots** par tes vrais produits
3. **Ajoute les prix**
4. **Change les couleurs** si tu veux un autre style
5. **Ajoute tes vrais liens** aux boutons

Besoin d'aide? Dis-moi ce que tu veux changer! 💪
