# Machine frigorifique en coupe

Simulateur pédagogique pour comprendre le fonctionnement d'une machine frigorifique.

**Page en ligne :** https://oliviercalmels.github.io/machine-frigorifique/

## Contenu

- **Simulateur de cycles**
  - Mono-étagé sous-critique, bi-étagé à injection totale, bi-étagé à injection partielle (cascade intégrée à venir).
  - Schéma animé du circuit : température du fluide, pression (paroi), liquide et vapeur dans les tubes.
  - Diagramme log P-h synchronisé avec le schéma, diagramme de l'air humide, tableau des points du cycle.
  - Fluides : R134a, R1234yf, R32, R290, R600a, R717, R744.
- **Visite d'installations réelles en 3D**
  - Réfrigérateur (capillaire) et maison avec climatisation réversible (vanne 4 voies, modes climatisation et pompe à chaleur).
  - Explication étape par étape, caméra qui zoome sur l'élément concerné, point suivi à la fois en 3D et sur le diagramme log P-h.

## Technique

Une seule page HTML autonome (`index.html`). Les propriétés des fluides sont calculées à partir des équations d'état de référence en énergie de Helmholtz (coefficients publiés, tels qu'utilisés par CoolProp), puis tabulées dans la page. La vue 3D utilise three.js (r128) chargé depuis un CDN.

Pour l'ouvrir en local : ouvrir `index.html` dans un navigateur.
