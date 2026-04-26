# 🕊️ Veni Spiritus

> *« L'Esprit et l'Épouse disent : Viens ! »* — Apocalypse 22 : 17

**Atelier web de rythmes & accords pour la louange et l'adoration.**

Un studio prophétique dans ton navigateur — progressions d'accords, boîte à rythmes, prompteur d'accords défilants, piano 88 touches visuel, sortie LED MIDI, et 10 ambiances musicales et visuelles pour entrer dans la présence.

🌐 **[Ouvrir Veni Spiritus →](https://devjam81.github.io/sanctus/)**

---

## 🎵 Les 10 ambiances

Chaque style change automatiquement la **palette visuelle**, le **son**, le **tempo** et la **progression d'accords par défaut**.

| Style | Ambiance | Son caractéristique |
|---|---|---|
| **Pop louange** | Hillsong, Bethel | Piano + basse classique |
| **Contemplatif** | Adoration douce | Piano avec reverb cathédrale |
| **Gospel** | Soul, énergique | Piano vif, rythmes syncopés |
| **Anthem** | Hymnes puissants | Piano + grosse pulsation |
| **Ballade** | Lent, intime | Piano nu, espace |
| **✦ Prophétique** | Feu, vision | Drone tonique + pad mystique en mineur |
| **☾ Soaking** | Méditation profonde | Pad stratosphérique, durée variable, sub-bass |
| **⟡ Strings atmosphérique** | Bethel TV, Upper Room | Ensemble de strings 4 couches, swell organique |
| **𓋹 Harpe de David** | Apaisement, antique | Arpèges roulants sur 2 octaves |
| **❀ Intimité avec Dieu** | Naomie Grace style | Piano cristallin + nappe + mélodie en arpège |

---

## 🎹 Banques de sons

5 banques disponibles dans le sélecteur "Banque de sons" :

- 🎹 **Synthé classique** — instantané, léger
- ✦ **Piano cristallin** — son Bethel/Hillsong avec ping-pong delay
- ⟡ **Chœur angélique** — FM synth, attaque lente, reverb 14s
- 𓋹 **Instrumental prophétique** — AM synth avec auto-filter mystique
- 🎼 **Vrai piano Salamander** — samples Yamaha C5 Grand Piano (~10 Mo)

---

## ✨ Fonctionnalités

🎼 **10 tonalités** majeures et mineures

🎶 **24 progressions d'accords** classiques

🥁 **Boîte à rythmes 16 pas** personnalisable

🎹 **Cartes d'accord interactives** avec affichage français (Do, Ré, Mi…)

📜 **Prompteur d'accords défilants** synchronisés à la lecture

🎼 **Piano 88 touches visuel** — les notes des accords s'illuminent en doré

🌙 **Mode Veillée** — interface immersive pour adorer dans le noir

⚡ **Sortie LEDs** : MIDI direct (Web MIDI API) ou HTTP vers JamLed Pi

🎵 **Sélecteur de canal MIDI** pour mode "guide silencieux"

---

## 🕊️ Versets cités

Selon le style activé, un verset différent apparaît en bas :

- **Modes classiques** — *Apocalypse 22 : 17*
- **Prophétique** — *Ésaïe 61 : 1*
- **Soaking** — *Jean 15 : 4*
- **Strings atmosphérique** — *Psaume 150 : 6*
- **Harpe de David** — *1 Samuel 16 : 23*
- **Intimité avec Dieu** — *Matthieu 6 : 6*

---

## 🎹 Intégration LEDs JamLed

Veni Spiritus peut piloter une rampe LED WS2812B au-dessus d'un piano via JamLed Pro (Raspberry Pi Zero 2W).

### Mode MIDI direct (recommandé)
- Détecte automatiquement tous les ports MIDI
- Sélection multi-ports avec sauvegarde
- **Latence quasi nulle**
- Sélecteur de canal MIDI (canal 2 = piano silencieux, LEDs allumées)

### Mode HTTP guide
- Envoie l'accord courant + le prochain au Pi
- Clignotement "next chord" pour anticipation

---

## 🛠️ Technique

- **HTML/CSS/JS** vanille, fichier unique
- **[Tone.js](https://tonejs.github.io/)** pour la synthèse audio
- **Web MIDI API** pour la sortie LED
- **Polices** : Cinzel, Cormorant Garamond, JetBrains Mono
- **Aucune dépendance backend**

---

## 🌐 Utilisation

### En ligne (HTTPS)
👉 [https://devjam81.github.io/sanctus/](https://devjam81.github.io/sanctus/)

### Local depuis JamLed Pi
```
http://jamled.local:5000/sanctus
```

---

## 📖 Inspiration

Veni Spiritus s'inspire des mouvements d'adoration contemporains :

- **Hillsong**, **Bethel**, **Upper Room** pour les progressions modernes
- **Steffany Gretzinger**, **Cory Asbury** pour le son atmosphérique
- **Naomie Grace** (YouTube) pour les instrumentales d'intimité francophones
- **La harpe de David** (1 Samuel 16) pour le mode prophétique antique
- **Les vitraux des cathédrales** pour l'esthétique visuelle
- **Veni Creator Spiritus** (hymne du IXe siècle) pour le nom

---

## 📜 Licence

MIT — utilise, modifie, partage librement pour la louange.

---

<p align="center">
  <em>Viens, Esprit Saint, embrase ton peuple.</em>
</p>

<p align="center">🕊️ · ✦ · 🕊️</p>
