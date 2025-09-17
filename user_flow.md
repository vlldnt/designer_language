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

## Explanation of the User Flow

This user flow describes how Michelle interacts with Spotify on desktop, including both the adult experience and the child-friendly Spotify Kids experience.

### 1. Starting point
- The user opens the Spotify desktop app
- If already logged in, they go directly to the profile selection screen
- If not logged in, they must enter their credentials before reaching the profile selection screen

### 2. Profile selection
- The user chooses who is listening
- Michelle can select her adult profile to access the standard Spotify interface
- If a child, such as Léon, is using the app, they can select the Spotify Kids profile
- If no child profile exists, the parent can create one (by entering name, avatar, and age)

### 3. Adult flow (Michelle)
- From the home screen, Michelle can use the search bar or navigate through tabs
- She may open a playlist such as French songs
- From there, she can view recommendations and decide whether to add a track to her library (Liked Songs or playlists)
- Alternatively, she can play a track directly
- After listening, she decides whether to continue exploring or to quit/switch profile

### 4. Child flow (Spotify Kids)
- The Kids interface presents visual categories (Songs, Nursery Rhymes, Discovery, Heroes)
- The child selects a card or playlist
- Tracks can be played with a large, simple Play button
- Children may "like" songs with a dedicated child-friendly button, saving them into My Favorites
- They can also use the Magic button for a surprise song
- At the end of a session, they may quit or switch back to the profile selection screen

### 5. Quick profile switching
- At any time, both Michelle (adult flow) and a child (Kids flow) can return to the profile selection screen via the profile menu/button

⸻

👉 In summary, this flow highlights how Spotify can seamlessly support multi-profile use within a family context, giving Michelle access to her personalized adult experience while also providing a safe, playful, and simplified environment for children.