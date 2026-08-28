# NPS Group — Site Vitrine

Site vitrine de **NPS Group**, entreprise de construction, pavage et menuiserie aluminium basée à Abomey-Calavi, Bénin.

🌐 **Production :** [https://npsgroup.bj](https://npsgroup.bj)

---

## Stack technique

- **Framework :** [Astro 5](https://astro.build) — génération statique (SSG)
- **Styles :** CSS pur avec variables CSS (sans Tailwind)
- **Typo :** Montserrat (Google Fonts)
- **Intégrations :** `@astrojs/sitemap`
- **Déploiement :** build statique (`dist/`)

---

## Structure du projet

```
src/
├── components/
│   ├── Header.astro        # Navigation principale
│   └── Footer.astro        # Pied de page (3 colonnes)
├── layouts/
│   └── BaseLayout.astro    # Layout global (SEO, meta, JSON-LD)
├── pages/
│   ├── index.astro         # Accueil (hero, services, BIM, CTA)
│   ├── expertises.astro    # Nos expertises (bento grid)
│   ├── realisations.astro  # Portfolio (bento filtrable)
│   ├── contact.astro       # Contact & devis (formulaire WhatsApp)
│   ├── mentions-legales.astro
│   └── confidentialite.astro
└── styles/
    ├── global.css          # Variables, typographie, composants de base
    └── polish.css          # Overrides visuels par section
public/
├── images/                 # Images hébergées localement
└── robots.txt
```

---

## Pages

| Route | Description |
|---|---|
| `/` | Accueil — hero, cœurs de métier, processus, BIM, CTA |
| `/expertises/` | Bento grid 4 expertises (Bâtiment, Pavage, Alu, BIM) |
| `/realisations/` | Portfolio filtrable par catégorie |
| `/contact/` | Formulaire de devis envoyé via WhatsApp |
| `/mentions-legales/` | Mentions légales |
| `/confidentialite/` | Politique de confidentialité |

---

## Développement

```bash
# Installer les dépendances
npm install

# Lancer le serveur de développement
npm run dev

# Build de production
npx astro build

# Prévisualiser le build
npx astro preview
```

---

## SEO

- Balises `title` et `meta description` par page
- Open Graph complet (titre, description, image, url, site_name)
- Twitter Card `summary_large_image`
- JSON-LD `LocalBusiness` + `GeneralContractor`
- `sitemap-index.xml` généré automatiquement
- `robots.txt` configuré
- URLs canoniques

---

## Contact NPS Group

- **Téléphone :** +229 01 44 59 84 47
- **E-mail :** npsgroupcontact@gmail.com
- **Adresse :** Togoudo, Abomey-Calavi, République du Bénin
- **WhatsApp :** [wa.me/2290144598447](https://wa.me/2290144598447)
