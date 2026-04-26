# ✦ Sanctus

> *« Je chanterai à l'Éternel tant que je vivrai »* — Psaume 104 : 33

**Atelier web de rythmes & accords pour la louange et l'adoration.**

Un studio prophétique dans ton navigateur — progressions d'accords, boîte à rythmes, prompteur d'accords défilants, et 9 ambiances musicales et visuelles pour entrer dans la présence.

🌐 **[Ouvrir Sanctus →](https://devjam81.github.io/sanctus/)**

---

## 🎵 Les 9 ambiances

Chaque style change automatiquement la **palette visuelle**, le **son**, le **tempo** et la **progression d'accords par défaut**.

| Style | Ambiance | Son caractéristique |
|---|---|---|
| **Pop louange** | Hillsong, Bethel | Piano + basse classique |
| **Contemplatif** ⭐ | Adoration douce | Piano avec reverb cathédrale |
| **Gospel** | Soul, énergique | Piano vif, rythmes syncopés |
| **Anthem** | Hymnes puissants | Piano + grosse pulsation |
| **Ballade** | Lent, intime | Piano nu, espace |
| **✦ Prophétique** | Feu, vision | Drone tonique + pad mystique en mineur |
| **☾ Soaking** | Méditation profonde | Pad stratosphérique, durée variable, sub-bass |
| **⟡ Strings atmosphérique** | Bethel TV, Upper Room | Ensemble de strings 4 couches, swell organique |
| **𓋹 Harpe de David** | Apaisement, antique | Arpèges roulants sur 2 octaves, résonance sympathique |

---

## ✨ Fonctionnalités

🎼 **10 tonalités** majeures et mineures (Do, Sol, Ré, La, Mi, Si, Fa, Si♭, Mi♭, La♭)

🎶 **24 progressions d'accords** classiques — I-V-vi-IV, vi-IV-I-V, i-VII-III-VI, etc.

🥁 **Boîte à rythmes 16 pas** — grosse caisse, caisse claire, charleston, shaker (clic pour activer/désactiver, pattern personnalisable)

🎹 **Cartes d'accord interactives** — clic pour preview, affichage en français (Do, Ré, Mi…) et chiffrage romain

📜 **Prompteur d'accords défilants** — l'accord courant se centre sur un curseur doré, les suivants en aperçu (parfait pour chanter)

⏱️ **Compteur mesure / temps** + **4 pulsations** dorées qui battent visuellement

🌙 **Mode Veillée** (bouton ☾ en haut à droite) — interface qui s'efface, juste accords et prompteur géant pour adorer dans le noir

⚡ **Sortie LEDs** double mode :
- **MIDI direct** via Web MIDI API (basse latence, marche sur HTTPS)
- **HTTP guide** vers JamLed Pi avec clignotement "next chord" pour anticiper

---

## 🕊️ Versets cités

Selon le style activé, un verset différent apparaît en bas :

- **Modes classiques** — *Psaume 104 : 33* — « Je chanterai à l'Éternel tant que je vivrai »
- **Prophétique** — *Ésaïe 61 : 1* — « L'Esprit du Seigneur, l'Éternel, est sur moi »
- **Soaking** — *Jean 15 : 4* — « Demeurez en moi, et je demeurerai en vous »
- **Strings atmosphérique** — *Psaume 150 : 6* — « Que toute âme qui respire loue l'Éternel »
- **Harpe de David** — *1 Samuel 16 : 23* — « Toutes les fois que le mauvais esprit était sur Saül, David prenait la harpe et en jouait »

---

## 🎹 Intégration LEDs JamLed

Sanctus peut piloter une rampe LED WS2812B au-dessus d'un piano via **JamLed Pro** (Raspberry Pi Zero 2W).

### Mode MIDI direct (recommandé)
- Détecte automatiquement tous les ports MIDI du navigateur
- Sélection multi-ports (piano Yamaha, port virtuel JamLed, etc.)
- Sauvegarde la sélection dans le navigateur
- **Latence quasi nulle**

### Mode HTTP guide
- Envoie l'accord courant + le prochain au Pi via REST
- Clignotement de l'accord suivant → anticipation visuelle
- Routes Flask à ajouter à JamLed : `/sanctus/notes` et `/sanctus/clear`

---

## 🛠️ Technique

- **HTML/CSS/JS** vanille, fichier unique
- **[Tone.js](https://tonejs.github.io/)** pour la synthèse audio (PolySynth, FMSynth, AMSynth, MembraneSynth, NoiseSynth)
- **Web MIDI API** pour la sortie LED
- **Polices** : Cinzel (titres lapidaires), Cormorant Garamond (corps), JetBrains Mono (mono)
- **Aucune dépendance backend** — fonctionne en HTML statique sur GitHub Pages

---

## 🌐 Utilisation

### En ligne (HTTPS)
👉 [https://devjam81.github.io/sanctus/](https://devjam81.github.io/sanctus/)

✅ Audio • ✅ MIDI direct • ❌ HTTP LEDs (mixed content)

### Local depuis JamLed Pi (HTTP)
```
http://jamled.local:5000/sanctus
```
✅ Tout fonctionne (ajouter route `/sanctus` dans `jamled_pro.py`)

---

## 📖 Inspiration

Sanctus s'inspire des mouvements d'adoration contemporains :

- **Hillsong**, **Bethel**, **Upper Room** pour les progressions modernes
- **Steffany Gretzinger**, **Cory Asbury**, **Amanda Cook** pour le son atmosphérique
- **La harpe de David** (1 Samuel 16) pour le mode prophétique antique
- **Les vitraux des cathédrales** pour l'esthétique visuelle

---

## 🎼 Captures d'écran

> *(à ajouter — montre les différentes ambiances : Cathédrale, Prophétique, Soaking, Strings, Harpe)*

---

## 📜 Licence

MIT — utilise, modifie, partage librement pour la louange.

---

<p align="center">
  <em>Que ton atelier devienne sanctuaire.</em>
</p>

<p align="center">✦ · ✦ · ✦</p>
