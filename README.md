# KAOS SPACE INVADERS, RS - 2025

## FUNZIONALITÀ PRINCIPALI
### 1. Sistema AI con Sottotitoli Sincronizzati
  - Inizio gioco
  - Arrivo UFO nemico
  - Ondate in arrivo
  - Colpi ai giocatori
  - Allarmi scudi critici
  - Nemici rimanenti
  - Vittoria e Game Over
  - Combo e punteggi record
  - Potenziamenti attivati
  - Boss wave in arrivo

### 2. Effetti Grafici 3D Pseudo-Perspective
- **Parallax Starfield** a 3 livelli con velocità differenziate
- **Scaling prospettico**: gli alieni più vicini appaiono più grandi
- **Effetto wobble**: movimento oscillante degli alieni
- **Rotazione UFO**: astronave nemica che ruota su se stessa
- **Glow effects**: bagliori neon su player, UFO, proiettili
- **Scanlines CRT**: effetto schermo arcade vintage
- **Vignette**: angoli scuri per simulare monitor CRT
- **Trail luminosi** sui proiettili

### 3. Sistema Audio Dinamico
- **Heartbeat progressivo**: musica cardiaca che accelera con la tensione
- **Suoni arcade**: spari, esplosioni, hit, vittoria, game over
- **Toni di notifica** per annunci vocali
- **Sincronizzazione** con numero nemici rimanenti

### 4. Sistema Particellare Avanzato
- **Esplosioni** con 20-30 particelle fisiche
- **Gravità e fisica** realistica
- **Fade-out** alpha progressivo
- **Colori contestuali** (rosso per nemici, giallo per UFO)
- **Trail proiettili** con particelle

### 5. Sistema Classifica e Punteggi
- **Top 10 punteggi** salvati localmente (JSON)
- **Medaglie**: 🥇 1°, 🥈 2°, 🥉 3° posto
- **Evidenziazione** oro/argento/bronzo
- **Data e livello** di ogni record
- **Persistenza** tra sessioni di gioco

### 6. UFO Mystery Ship Bonus
- **Apparizioni casuali** ogni 10-20 secondi
- **Punteggio bonus variabile**: 50-300 punti
- **Movimento bidirezionale** (sinistra/destra)
- **Effetto rotazione** con glow magenta
- **Notifica visiva** al colpo

### 7. Interfaccia Completamente Italiana
- Menu, HUD, messaggi, annunci
- Comandi intuitivi
- Istruzioni chiare

-----------------------------------------------------------------------------

##  GAMEPLAY
### Obiettivo
Difendi la Terra dall'invasione aliena distruggendo tutte le ondate nemiche!

### Meccaniche
- **5 Ondate** di difficoltà crescente
- **3 Tipi di alieni** con punteggi diversi
- **Scudi protettivi** che si deteriorano
- **UFO bonus** per punteggi extra
- **Sistema vite**: 3 vite iniziali
- **Proiettili nemici** sempre più veloci

### Punteggi
- Alieno Tipo 1: 10 punti
- Alieno Tipo 2: 20 punti
- Alieno Tipo 3: 30 punti
- UFO: 50-300 punti (casuale)

## ARCHITETTURA TECNICA
### Tecnologia
- **.NET 8.0 Windows Forms**
- **C# con Graphics GDI+**
- **System.Drawing** per rendering 2D
- **Double-buffering** per fluidità
- **JSON** per persistenza dati
- **Task async** per annunci vocali

### Struttura del Codice
```
SpaceInvaders/
├── Core/
│   ├── GameEngine.cs         # Motore di gioco principale
│   ├── LeaderboardManager.cs # Gestione punteggi
│   └── Entity.cs             # Entità base
├── Entities/
│   ├── Player.cs             # Giocatore
│   ├── AlienFormation.cs     # Formazione alieni
│   ├── UFO.cs                # Astronave bonus
│   ├── Bullet.cs             # Proiettili
│   └── Shield.cs             # Scudi
├── Graphics/
│   ├── GameForm.cs           # Form principale
│   ├── GraphicsRenderer.cs   # Renderer grafico
│   ├── SpriteLibrary.cs      # Libreria sprite
│   ├── ParticleSystem.cs     # Sistema particelle
│   ├── Effects3D.cs          # Effetti 3D
│   ├── SubtitleSystem.cs     # Sottotitoli
│   ├── VoiceAnnouncer.cs     # Annunci vocali
│   ├── SoundManager.cs       # Gestione audio
│   └── LeaderboardForm.cs    # Form classifica
└── Program.cs                # Entry point
```

## PERFORMANCE
- **Frame Rate**: 30 FPS costanti
- **Risoluzione**: 800x600 pixels
- **Memoria**: ~50 MB
- **CPU**: Minimo dual-core
- **OS**: Windows 10/11

## STILE VISIVO
### Palette Colori Arcade
- **Neon Cyan**: interfaccia e player
- **Magenta**: UFO e effetti speciali
- **Giallo/Oro**: esplosioni e vittoria
- **Verde Lime**: player e scudi
- **Rosso**: nemici e danger

### Effetti Speciali
- Glow dinamico
- Scanlines retrò
- Starfield multilivello
- Vignette CRT
- Trail luminosi
- Rotazioni fluide


## NOTE SVILUPPO
### Versione Attuale: 1.0
**Implementato:**
✅ Effetti 3D pseudo (Amiga style)  
✅ Parallax starfield (Amiga style)  
✅ Effetti arcade (scanlines, vignette, glow)  
✅ Particelle avanzate  
✅ Classifica persistente  
✅ UFO bonus  
✅ Interfaccia italiana  

## CREDITI
**Sviluppato da:** RS  
**Linguaggio:** C# .NET 8.0  
**Framework:** Windows Forms  
**Librerie:** System.Drawing, System.Media  
**Ispirato da:** Space Invaders (Taito, 1978)  
**Stile:** Arcade moderno rivisitato

## COME COMPILARE ED ESEGUIRE
### Requisiti
- .NET 8.0 SDK installato
- Windows 10/11
- Visual Studio 2022 o VS Code (opzionale)

## LICENZA
Progetto educativo e dimostrativo, 2025 RS
Ispirato da: Space Invaders (Taito, 1978)

-----------------------------------------------------------------------------

## COMANDI
| Tasto | Azione |
|-------|--------|
| **← →** o **A D** | Muovi astronave | o Mouse
| **SPAZIO**		    | Spara |
| **Y**				      | Chiama Cortana in aiuto|
| **ESC**		      	| Esci dal gioco |
| **F2**		      	| Nuova partita  |
| **F3**			      | Visualizza classifica |


**BUON DIVERTIMENTO E DIFENDI LA TERRA!**
