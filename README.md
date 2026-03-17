# 🎉 GameNight

Eine Party-Spiele-App für Gruppen — online & offline spielbar!

## Spiele
- 🤔 Wer würde eher (🟢 Online)
- 🎭 Wahrheit oder Pflicht (🟢 Online)
- 🎲 Würfelspiel
- 🕵️ Imposter
- 🙅 Ich habe noch nie (🟢 Online)
- 🔤 Kategorien
- 🔥 Heiße Kartoffel (🟢 Online)
- ⚡ Reaktionszeit
- 🔥 Heißer Stuhl
- 🥠 Glückskeks
- 💬 Flüster-Roulette
- ⚡ Blitz-Quiz (🟢 Online — 430+ Fragen!)
- 🎨 Malen & Raten (🟢 Online)

## Neue Features (Update)
- ✅ **Blitz-Quiz**: 430+ Fragen in 7 Kategorien (Allgemein, Popkultur, Wissenschaft, Geschichte, Sport, Essen, Deutschland)
- ✅ **Keine Wiederholungen**: Fragen wiederholen sich nicht innerhalb einer Session
- ✅ **Admin-Wörter → Spicy**: Alle im Admin-Panel hinzugefügten Wörter landen automatisch im Spicy-Pool des jeweiligen Spiels
- ✅ **Live-Voting Sync**: Abstimmungen bei "Wer würde eher" werden in Echtzeit für alle Spieler aktualisiert

## Online-Lobby
Erstelle eine Lobby und teile den Code mit Freunden!  
Der Host steuert das Spiel — alle Mitspieler sehen nur was sie sehen sollen.

## Supabase Setup
Die App nutzt Supabase für Online-Multiplayer. Benötigte Tabellen:
- `lobbies` — Lobby-Räume
- `lobby_players` — Spieler in einer Lobby
- `lobby_events` — Echtzeit-Spielereignisse
- `bq_sessions` — Blitz-Quiz Sessions
- `bq_answers` — Spielerantworten
- `draw_rounds` — Malen & Raten Runden
- `draw_strokes` — Zeichenstriche
- `draw_guesses` — Rateversuche
- `custom_words` — Admin-eigene Wörter

## Deployment (GitHub Pages)

1. Erstelle ein neues GitHub-Repository
2. Lade alle Dateien hoch (oder nutze git push)
3. Gehe zu Settings → Pages → Source: main branch → / (root)
4. Die App ist unter `https://USERNAME.github.io/REPO-NAME/` erreichbar

```bash
git init
git add .
git commit -m "GameNight deploy"
git remote add origin https://github.com/USERNAME/gamenight.git
git push -u origin main
```

## Lokale Nutzung
Einfach `index.html` im Browser öffnen!
