# Here starts the journey with Cinescope
Binome :
- Shreya AHLUWALIA
- Paul LECOMTE

## First install your project
- you can copy the repo locally using `git clone`
- go to the root of the directory and run `npm i`
- run the project with `npm run dev`

## Constats
- Les pastilles de couleur (vertes ou rouges) ne sont pas explicites : rien n'indique ce qu'elles représentent, et l'information repose uniquement sur la couleur
- On suppose que l'étoile représente les favoris, mais ce n'est pas explicite
- On ne s'y retrouve pas avec la navigation au clavier : aucun focus n'est visible, on ne sait pas quel composant est sélectionné
- La navigation au clavier permet de mettre un film en favori, mais pas de sélectionner un film
- Après une recherche, la carte restante s'étire sur toute la largeur de la page au lieu de garder une taille normale

## Impacts avant et après l'accessibilité

| Impact | Avant | Après |
| --- | --- | --- |
| **Disponibilité des places** | L'information repose uniquement sur une pastille verte ou rouge : illisible pour une personne daltonienne, absente pour un lecteur d'écran et incompréhensible sans légende. | La pastille et son libellé ne forment plus qu'un seul badge, placé sur l'affiche : "Places disponibles" ou "Places indisponibles", lisible par tous. |
| **Favoris** | Le bouton n'affiche qu'une étoile "☆" ou "★" : on doit deviner qu'il s'agit des favoris. | Le bouton affiche explicitement "Favoris ☆" / "Favoris ★". |
| **Recherche** | Quand un seul film correspond, sa carte occupe toute la largeur de la page. | Les cartes gardent la même taille, quel que soit le nombre de résultats. |

## Reste à faire
- Rendre les cartes atteignables et activables au clavier pour pouvoir sélectionner un film
- Rendre le focus visible sur la recherche, les liens, les cartes et le bouton favori
- Ajouter un texte alternatif aux affiches et un libellé à la barre de recherche
