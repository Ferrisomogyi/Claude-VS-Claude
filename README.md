# 🤖⚡🤖 Claude vs Claude

Twee AI's, één gesprek — jij hebt de controle.

## Wat is dit?

Een Progressive Web App (PWA) die twee Claude-instanties met elkaar laat praten. 
Kies een modus (Mystery Solvers of Dev Pair Programming), kies je model 
(Opus 4.6, Sonnet 4.6, of Sonnet 4), geef een onderwerp, en laat ze gaan.

### Features
- 🧠 Modelkeuze: Opus 4.6, Sonnet 4.6, Sonnet 4
- 💰 Live kostentracker in euro's
- ⏸ Automatische pauze bij elke €1 aan kosten
- 💬 Stel tussendoor vragen aan de Claude's
- 🔐 API key wordt lokaal op je apparaat opgeslagen
- 📱 Installeerbaar als app op je telefoon

---

## Installatie op GitHub Pages (stap voor stap)

### 1. Maak een GitHub account (als je dat nog niet hebt)
- Ga naar https://github.com en maak een gratis account

### 2. Maak een nieuwe repository
- Klik op het **+** icoon rechtsboven → **New repository**
- Naam: `claude-vs-claude` (of wat je wilt)
- Zet op **Public**
- Vink NIET "Add a README file" aan
- Klik **Create repository**

### 3. Upload de bestanden
- Op de lege repo-pagina, klik op **"uploading an existing file"**
- Sleep deze 3 bestanden erin:
  - `index.html`
  - `manifest.json`
  - `sw.js`
- Klik **Commit changes**

### 4. Zet GitHub Pages aan
- Ga naar **Settings** (tandwiel, bovenaan de repo)
- Klik links op **Pages**
- Bij "Source" kies: **Deploy from a branch**
- Bij "Branch" kies: **main** en **/ (root)**
- Klik **Save**
- Wacht 1-2 minuten

### 5. Open je app
- Je app staat nu op: `https://JOUWUSERNAME.github.io/claude-vs-claude/`
- (Vervang JOUWUSERNAME door je GitHub gebruikersnaam)

### 6. Installeer als app op je telefoon
- Open de URL in **Chrome** op je telefoon
- Tik op de drie puntjes (⋮) rechtsboven
- Kies **"Toevoegen aan startscherm"** of **"App installeren"**
- De app staat nu als icoon op je startscherm!

---

## API Key

Je hebt een Anthropic API key nodig:

1. Ga naar https://console.anthropic.com
2. Maak een account of log in
3. Ga naar **API Keys** 
4. Maak een nieuwe key aan
5. Kopieer de key (begint met `sk-ant-...`)
6. Plak hem in de app bij eerste gebruik

De key wordt **alleen lokaal op je apparaat** opgeslagen (localStorage).
Hij wordt nooit naar een server gestuurd behalve naar de Anthropic API.

---

## Kosten

De app trackt je kosten live. Indicatie per gesprek van ~10 rondes:

| Model | ~Kosten per 10 rondes |
|-------|----------------------|
| Sonnet 4 | €0.05 - €0.15 |
| Sonnet 4.6 | €0.05 - €0.15 |
| Opus 4.6 | €0.10 - €0.40 |

De app pauzeert automatisch bij elke €1 zodat je nooit verrast wordt.

---

## Bestanden

```
claude-vs-claude/
├── index.html      ← De complete app (alles-in-één)
├── manifest.json   ← PWA configuratie (voor app-installatie)
├── sw.js           ← Service Worker (voor offline support)
└── README.md       ← Dit bestand
```
