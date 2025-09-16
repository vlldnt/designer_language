# Spotify User Flow - Flow Diagram

```mermaid
flowchart TD
    A([Open Spotify Desktop]) --> B{Already logged in?}
    B -- No --> C[Enter credentials] --> D[Profile selection screen]
    B -- Yes --> D[Profile selection screen]

    D --> E{Who's listening?}
    E -- Michelle adult --> F[Adult home]
    E -- Child e.g. Leon --> K[Spotify Kids home]
    E -- No child profile --> J[Create child profile - name, avatar, age] --> K

    %% --- Adult flow Michelle ---
    F --> F1[Search bar / navigation]
    F1 --> F2[Tab or playlist: French songs]
    F2 --> F3[View recommendations]
    F3 --> F4{Add a track?}
    F4 -- Yes --> F5[Add to playlist / Liked songs]
    F4 -- No --> F6[Play a track]
    F5 --> F6
    F6 --> F7{Continue listening?}
    F7 -- Yes --> F2
    F7 -- No --> H[Switch profile / Quit]

    %% --- Child flow Kids ---
    K --> K1[Visual categories: Songs, Nursery Rhymes, Discovery, Heroes]
    K1 --> K2[Choose a card / playlist]
    K2 --> K3[Play a track - big Play button]
    K3 --> K4{Add / Child Like?}
    K4 -- Yes --> K5[Add to My Favorites - child space]
    K4 -- No --> K6[Next / Surprise - Magic button]
    K5 --> K6
    K6 --> K7{End session?}
    K7 -- Yes --> H[Switch profile / Quit]
    K7 -- No --> K1

    %% --- Quick changes ---
    F -. profile menu .-> D
    K -. profile button .-> D
```