# Parcours Utilisateur Spotify - Diagramme de Flux

```mermaid
flowchart TD
    A([Ouvrir Spotify Desktop]) --> B{Déjà connecté ?}
    B -- Non --> C[Entrer identifiants] --> D[Écran de sélection de profil]
    B -- Oui --> D[Écran de sélection de profil]

    D --> E{Qui écoute ?}
    E -- Michelle (adulte) --> F[Accueil adulte]
    E -- Enfant (ex : Léon) --> K[Accueil Spotify Kids]
    E -- Aucun profil enfant --> J[Créer profil enfant - nom, avatar, âge] --> K

    %% --- Parcours adulte (Michelle) ---
    F --> F1[Barre de recherche / navigation]
    F1 --> F2[Onglet ou playlist : « Françaises »]
    F2 --> F3[Voir recommandations]
    F3 --> F4{Ajouter un titre ?}
    F4 -- Oui --> F5[Ajouter à playlist / Titres likés]
    F4 -- Non --> F6[Lire un titre]
    F5 --> F6
    F6 --> F7{Continuer l'écoute ?}
    F7 -- Oui --> F2
    F7 -- Non --> H[Changer de profil / Quitter]

    %% --- Parcours enfant (Kids) ---
    K --> K1[Catégories visuelles : Chansons, Comptines, Découverte, Héros]
    K1 --> K2[Choisir une carte / playlist]
    K2 --> K3[Lire un titre (gros bouton Play)]
    K3 --> K4{Ajouter / Like enfantin ?}
    K4 -- Oui --> K5[Ajout dans « Mes Favoris » (espace enfant)]
    K4 -- Non --> K6[Suivant / Surprise (bouton Magie)]
    K5 --> K6
    K6 --> K7{Fin de session ?}
    K7 -- Oui --> H[Changer de profil / Quitter]
    K7 -- Non --> K1

    %% --- Changements rapides ---
    F -. menu profil .-> D
    K -. bouton profil .-> D
```