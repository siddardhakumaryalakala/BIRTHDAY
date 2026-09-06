# BIRTHDAY
# 🎬 For You — A Birthday Film

> An interactive cinematic birthday website built entirely with **HTML, CSS, and JavaScript**.

A little different from a normal birthday website — this project turns a birthday message into a **mini interactive movie** with scenes, animations, memories, a timeline, an interactive letter, a gift box, birthday cake, candles, confetti, music, and a final birthday reveal.

---

## ✨ Features

### 🎞️ Cinematic Experience

* Movie-style introduction
* Cinematic letterbox bars
* Chapter counter
* Scroll-based chapter navigation
* Smooth scrolling
* Animated scene transitions

### 🌌 Animated Background

* Dynamic star field using HTML Canvas
* Twinkling stars
* Shooting stars
* Mouse-based parallax effect
* Animated glowing nebula effects
* Film-grain overlay
* Vignette effect

### 📸 Memory Gallery

* Polaroid-style memory cards
* Floating animations
* Hover interactions
* Custom captions and timestamps
* Easy replacement with real photos

### 📝 Chaos Wall

* Scrap-paper style memory cards
* "Exhibit A, B, C..." layout
* Random-looking rotations
* Pin and tape effects
* Interactive hover animations

### 💕 Best Memories

* Animated memory quotes
* Floating hearts
* Responsive typography
* Scroll-triggered reveal animations

### ⏳ Friendship Timeline

* Vertical timeline
* Animated progress line
* Timeline markers
* Highlighted milestones
* Responsive mobile timeline

### 💌 Interactive Letter

* Animated envelope
* Interactive seal
* Envelope opening animation
* Typewriter effect
* Skip typing interaction
* Personalized signature

### 🎁 Interactive Gift

* Animated gift box
* Gift opening animation
* Confetti burst
* Birthday cake reveal

### 🎂 Birthday Cake

* CSS-generated cake
* Animated candles
* Flickering flames
* Candle blow-out interaction
* Smoke animation
* Birthday wish interaction

### 🎉 Final Reveal

* Happy Birthday animation
* Animated name reveal
* Personalized message
* Confetti drizzle
* Credits section
* Replay button

### 🎵 Sound

* Built-in Web Audio API
* Happy Birthday music-box style melody
* Envelope chime
* Gift opening sound
* Candle whoosh sound
* Music toggle button

### 📱 Responsive Design

Works across:

* 💻 Desktop
* 💻 Laptop
* 📱 Mobile
* 📲 Tablet

The layout automatically adapts for smaller screens.

---

# 🛠️ Technologies Used

This project intentionally avoids frameworks and external JavaScript libraries.

| Technology                | Usage                                   |
| ------------------------- | --------------------------------------- |
| HTML5                     | Website structure                       |
| CSS3                      | Styling, animations & responsive layout |
| JavaScript                | Interactions & dynamic content          |
| Canvas API                | Stars & confetti                        |
| Web Audio API             | Music & sound effects                   |
| Intersection Observer API | Scroll animations                       |
| Google Fonts              | Typography                              |

### Fonts

The website uses:

* **Fraunces** — Main cinematic typography
* **Caveat** — Handwritten memories and letters
* **Space Mono** — Cinematic technical labels

---

# 📂 Project Structure

```text
birthday-film/
│
├── index.html
│
├── README.md
│
├── assets/
│   ├── images/
│   │   ├── memory-01.jpg
│   │   ├── memory-02.jpg
│   │   └── memory-03.jpg
│   │
│   └── music/
│       └── birthday.mp3
│
└── screenshots/
    └── preview.png
```

> The current version can run as a single `index.html` file without additional assets.

---

# 🚀 Getting Started

## 1. Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/birthday-film.git
```

## 2. Open the Project

Go into the project directory:

```bash
cd birthday-film
```

## 3. Run the Website

You can simply open:

```text
index.html
```

in your browser.

For the best development experience, use **VS Code + Live Server**.

---

# 🎨 Personalization

One of the main goals of this project is making personalization extremely easy.

You don't need to search through the entire HTML file.

Inside the JavaScript section, find:

```javascript
const CONFIG = {
```

Everything important can be changed there.

---

## 👤 Change the Name

Find:

```javascript
name: "Alex",
```

Change it to your friend's name:

```javascript
name: "Ananya",
```

The name automatically appears throughout the website.

---

## ✍️ Change the Signature

Find:

```javascript
signature: "your favorite human",
```

For example:

```javascript
signature: "Siddu",
```

The signature will appear in the letter and final scene.

---

# 📸 Adding Your Own Photos

The current version uses placeholder images from:

```text
picsum.photos
```

Example:

```javascript
<img src="https://picsum.photos/seed/${m.seed}/560/640.jpg">
```

For real memories, replace the image source with your own local images.

For example:

```text
assets/images/memory-01.jpg
assets/images/memory-02.jpg
assets/images/memory-03.jpg
```

Then change the image rendering code to use:

```javascript
<img src="assets/images/memory-01.jpg">
```

---

# 💭 Customize Memories

Inside `CONFIG`, you'll find:

```javascript
memories: [
  {
    seed: "film-01",
    caption: "The day we met.",
    stamp: "SOMEWHERE AT THE BEGINNING"
  }
]
```

You can change the captions and timestamps.

Example:

```javascript
memories: [
  {
    seed: "memory-01",
    caption: "The day our friendship officially became chaos.",
    stamp: "2022 — THE BEGINNING"
  },
  {
    seed: "memory-02",
    caption: "That trip we'll never forget.",
    stamp: "SUMMER 2024"
  },
  {
    seed: "memory-03",
    caption: "Still one of my favorite memories.",
    stamp: "FOREVER"
  }
]
```

---

# 🤣 Customize the Chaos Wall

Change:

```javascript
chaos: [
```

Example:

```javascript
chaos: [
  {
    tag: "EXHIBIT A",
    text: "That one night when we stayed awake until 3AM talking about everything."
  },
  {
    tag: "EXHIBIT B",
    text: "The trip where absolutely nothing went according to plan."
  },
  {
    tag: "EXHIBIT C",
    text: "Every 'five minute' conversation that somehow lasted three hours."
  }
]
```

---

# 💕 Customize Best Memories

Change:

```javascript
best: [
```

Example:

```javascript
best: [
  "The conversations that made <em>everything feel better.</em>",
  "The laughs that made <em>ordinary days unforgettable.</em>",
  "And every little moment that somehow became <em>a memory.</em>"
]
```

You can use `<em>` to highlight specific words.

---

# ⏳ Customize the Timeline

The timeline is controlled through:

```javascript
timeline: [
```

Example:

```javascript
timeline: [
  {
    year: "2022",
    title: "The beginning",
    text: "The year everything started."
  },
  {
    year: "2023",
    title: "The chaos",
    text: "Too many memories. Not enough photos."
  },
  {
    year: "2024",
    title: "The good times",
    text: "Some of my favorite memories happened here."
  },
  {
    year: "∞",
    title: "Still here",
    heart: true,
    text: "And we're just getting started."
  }
]
```

---

# 💌 Customize the Letter

The letter is stored inside:

```javascript
letter: `
Dear {name},

...
`
```

You can completely replace the message.

The special placeholder:

```text
{name}
```

automatically becomes the friend's name.

For example:

```javascript
letter: `
Dear {name},

Happy birthday!

I don't know how we went from a random conversation
to creating this many memories together.

Thank you for being there through all the chaos,
the late-night conversations, the laughs,
and everything in between.

Here's to all the memories we've already made
and all the ones still waiting for us.

Happy birthday.
`
```

---

# 🎂 Change the Number of Candles

The cake currently uses:

```javascript
const CANDLE_N = 5;
```

Change it to:

```javascript
const CANDLE_N = 10;
```

and the website will automatically generate 10 candles.

---

# 🎉 Customize the Final Message

Find:

```javascript
finalMessage:
```

Example:

```javascript
finalMessage:
"Another year, another collection of memories. Here's to more adventures, more laughs, more chaos, and everything still waiting for us."
```

---

# 🎵 Music

The website uses the **Web Audio API** instead of requiring an audio file.

The music can be enabled using the music button in the bottom-right corner.

Because modern browsers restrict automatic audio playback, the user needs to interact with the music button before audio starts.

---

# 🧠 How the Website Works

The experience is divided into **8 chapters**:

```text
SC.00 → Prologue
   ↓
SC.01 → Title Card
   ↓
SC.02 → First Memory
   ↓
SC.03 → The Crazy Ones
   ↓
SC.04 → Best Memories
   ↓
SC.05 → Timeline
   ↓
SC.06 → The Letter
   ↓
SC.07 → Finale
```

The user progresses through the story simply by scrolling.

---

# ⚙️ Important JavaScript Systems

### Intersection Observer

Used for detecting when elements enter the viewport.

This powers:

* Text reveals
* Polaroid animations
* Timeline animations
* Chapter tracking
* Floating hearts

---

### Canvas API

Two canvases are used.

#### Star Canvas

```html
<canvas id="stars"></canvas>
```

Responsible for:

* Stars
* Twinkling
* Shooting stars
* Parallax movement

#### Confetti Canvas

```html
<canvas id="confetti"></canvas>
```

Responsible for:

* Gift explosion
* Confetti physics
* Final celebration

---

### Web Audio API

Used to generate:

* Birthday melody
* Chimes
* Whoosh effects
* Pop sounds

No audio library is required.

---

# 📱 Responsive Design

The website includes a mobile breakpoint:

```css
@media (max-width:720px)
```

On mobile:

* Timeline becomes single-column
* Navigation spacing changes
* Polaroids resize
* Scrap cards resize
* Typography scales automatically

---

# ♿ Accessibility

Some accessibility features are included:

* Keyboard interaction
* `aria-label`
* `aria-pressed`
* Focus-visible outlines
* Reduced-motion support
* Semantic sections
* Keyboard support for interactive elements

The website also respects:

```css
prefers-reduced-motion
```

for users who prefer reduced animation.

---

# 🌐 Deployment

Because this is a static website, it can be deployed easily using platforms such as:

* GitHub Pages
* Netlify
* Vercel
* Cloudflare Pages

No backend or database is required.

---

# 💡 Future Improvements

Possible additions:

* [ ] Real photo gallery
* [ ] Background music upload
* [ ] Custom cursor
* [ ] Photo transitions
* [ ] Video memory section
* [ ] Secret hidden message
* [ ] Password-protected birthday page
* [ ] Countdown to birthday
* [ ] Fireworks animation
* [ ] Interactive memory map
* [ ] Voice message
* [ ] Mobile swipe navigation
* [ ] Shareable personalized URL
* [ ] QR code to open the birthday film
* [ ] Personalized theme selector

---

# ❤️ Why This Project?

Most birthday websites are basically:

> "Happy Birthday 🎂"

This project tries to turn a birthday message into an **experience**.

Instead of simply reading a message, the person:

```text
Scrolls
   ↓
Discovers
   ↓
Remembers
   ↓
Interacts
   ↓
Opens the letter
   ↓
Opens the gift
   ↓
Blows out the candles
   ↓
Gets the final birthday message
```

It's basically a tiny **interactive birthday movie** built with vanilla web technologies.

---

# 📜 License

This project is free to use, modify, and personalize.

If you use it for someone special, make it your own. ❤️

---

## ⭐ If You Like It

Give the repository a ⭐ and feel free to customize it for your own best friend.

**Made with HTML, CSS, JavaScript, memories, and way too much dramatic animation. 🎬❤️**

---

### 🎬 End Credits

```text
WRITTEN & DIRECTED BY
YOUR BEST FRIEND

STARRING
THE BEST HUMAN EVER

SPECIAL THANKS
FOR ALL THE MEMORIES

NO FRIENDSHIPS WERE HARMED
IN THE MAKING OF THIS WEBSITE

FIN.
```
