# 💌 Teachers' Day Letter — Sir Randy Bello

**LIVE VIEW:** https://babasajustinecatherine978-droid.github.io/Teacher-day-card/

A creative and interactive **Teachers' Day digital letter** made with **HTML, CSS, and JavaScript**.

This project is designed as a personalized appreciation letter for **Sir Randy Bello**, a Web Development instructor. It features an animated envelope, an interactive letter, floating hearts, and a Dark/Light Mode switch.

---

## ✨ Features

* 💌 Interactive animated envelope
* 📖 Animated letter opening effect
* ❤️ Floating heart animations
* 🌙 Dark Mode
* ☀️ Light Mode
* 💾 Remembers the selected theme using `localStorage`
* 🖼️ Teacher photo included in the letter
* ✨ Smooth CSS transitions and animations
* ⌨️ Keyboard support using `Enter` or `Space`
* 📱 Responsive design for desktop and mobile devices
* ♿ Reduced-motion support for users who prefer less animation
* 🎨 Professional pink, black, and light-themed design
* 📚 Personalized Teachers' Day message for Sir Randy Bello

---

## 🛠️ Technologies Used

| Technology   | Purpose                                                    |
| ------------ | ---------------------------------------------------------- |
| HTML5        | Website structure and letter content                       |
| CSS3         | Design, animations, transitions, responsive layout         |
| JavaScript   | Envelope interaction, theme switching, and floating hearts |
| LocalStorage | Saves the user's Dark/Light Mode preference                |

---

## 📁 Project Structure

```text
Teachers_day_card/
│
├── index.html
├── README.md
│
└── images/
    └── bello.png.jpg
```

> Make sure the image path in `index.html` matches the location of your image.

The current project references the teacher image as:

```html
<img class="teacher-photo"
     src="Teachers_day_card/images/bello.png.jpg"
     alt="Sir Randy Bello">
```

---

## 🚀 How to Use

### 1. Download or Clone the Project

Clone the repository:

```bash
git clone https://github.com/YOUR-USERNAME/teachers-day-letter.git
```

Then open the project folder:

```bash
cd teachers-day-letter
```

---

### 2. Check Your Files

Make sure your project contains the required files:

```text
index.html
README.md
images/
└── bello.png.jpg
```

---

### 3. Open the Website

This project does not require a server or database.

Simply double-click:

```text
index.html
```

It will open in your web browser.

You can also right-click `index.html` and select:

**Open with → Google Chrome / Microsoft Edge / Firefox**

---

## 💌 How the Letter Works

When the website opens, you will see the Teachers' Day introduction and an animated envelope.

Click the envelope to open the letter.

The opening animation reveals the personalized message for Sir Randy Bello and creates floating heart animations.

You can also press:

```text
Enter
```

or

```text
Space
```

when the envelope is focused to open it.

---

## 🌙 Dark / Light Mode

The website includes a theme switch in the top navigation bar.

Click:

```text
☀️ Light Mode
```

to switch to Light Mode.

The button changes to:

```text
🌙 Dark Mode
```

Click it again to return to Dark Mode.

The selected theme is automatically saved in the browser using `localStorage`, so your preference remains after refreshing the page.

---

## ✏️ How to Customize the Letter

You can personalize the project by editing the text directly inside `index.html`.

### Change the Teacher's Name

Find:

```html
<span>
    Sir Randy Bello
</span>
```

Replace it with the teacher's name you want.

For example:

```html
<span>
    Sir Juan Dela Cruz
</span>
```

---

### Change the Subtitle

Find the subtitle:

```html
<p class="subtitle">
    A small letter for a teacher whose lessons go
    beyond code — inspiring creativity, patience,
    confidence, and the courage to keep learning.
</p>
```

Replace the text with your own message.

---

### Change the Main Letter

The main letter content is inside:

```html
<div class="letter" id="letter">
```

You can edit the paragraphs inside this section.

Example:

```html
<p>
    Thank you for your guidance, patience, and
    dedication. Your lessons have inspired us
    to become better students and developers.
</p>
```

---

### Change the Teacher Photo

Replace the image file in the `images` folder.

For example:

```text
images/
└── teacher.jpg
```

Then update the HTML:

```html
<img class="teacher-photo"
     src="images/teacher.jpg"
     alt="Teacher">
```

Make sure the filename and path are correct.

---

### Change the Signature

Find:

```html
<div class="signature">
    Your Student ♥️
</div>
```

You can change it to:

```html
<div class="signature">
    From Your Students ♥️
</div>
```

---

## 🎨 Changing the Colors

The main colors are controlled by CSS variables near the beginning of the `<style>` section.

For example:

```css
:root {
    --pink: #ff4f9a;
    --pink-light: #ff9fc8;
    --pink-dark: #d91f70;

    --black: #080808;
    --black2: #151515;

    --white: #ffffff;
}
```

You can change these values to create your own color theme.

For example, you could use:

```css
--pink: #6c63ff;
--pink-light: #a29bfe;
--pink-dark: #4834d4;
```

---

## ❤️ Floating Hearts

The website automatically creates floating heart animations using JavaScript.

The hearts are generated by:

```javascript
function createHeart() {
    const heart = document.createElement("div");

    heart.className = "floating-heart";

    heart.textContent =
        Math.random() > 0.5
            ? "♥"
            : "♡";
}
```

Additional hearts are automatically created every few seconds.

You can change the animation timing here:

```javascript
setInterval(
    function() {
        if (Math.random() > 0.35) {
            createHeart();
        }
    },
    1800
);
```

---

## 📱 Responsive Design

The website automatically adjusts for smaller screens using CSS media queries.

Mobile devices receive:

* Smaller envelope size
* Smaller teacher image
* Adjusted letter spacing
* Responsive typography
* Mobile-friendly layout

You can test the design using your browser's developer tools.

In Chrome or Edge:

```text
Right Click → Inspect → Toggle Device Toolbar
```

---

## ♿ Reduced Motion

The project includes support for users who prefer reduced animation.

The CSS detects:

```css
@media (prefers-reduced-motion: reduce)
```

and reduces animation and transition durations.

---

## 🌐 Deploy to GitHub Pages

You can publish this project online for free using **GitHub Pages**.

### Step 1 — Create a Repository

Create a new GitHub repository, for example:

```text
teachers-day-letter
```

### Step 2 — Upload Your Files

Upload:

```text
index.html
README.md
images/
```

Make sure the image remains inside the correct folder.

### Step 3 — Enable GitHub Pages

Go to:

```text
Repository → Settings → Pages
```

Under **Build and deployment**, select:

```text
Source: Deploy from a branch
```

Choose:

```text
Branch: main
Folder: / (root)
```

Then click:

```text
Save
```

GitHub will generate a public website link for your project.

---

## 🧪 Running Locally

No installation is required.

You do **not** need:

* Node.js
* npm
* PHP
* MySQL
* Python
* A web server

Just open:

```text
index.html
```

in a modern web browser.

---

## 📸 Preview

The website presents an elegant Teachers' Day experience:

```text
┌─────────────────────────────────────────┐
│       A LETTER OF GRATITUDE             │
│                          ☀️ Light Mode  │
│                                         │
│          Teachers' Day                  │
│                                         │
│       For Sir Randy Bello               │
│                                         │
│     ┌─────────────────────────┐         │
│     │                         │         │
│     │        💗              │         │
│     │     ENVELOPE            │         │
│     │                         │         │
│     │  Click to open          │         │
│     └─────────────────────────┘         │
│                                         │
└─────────────────────────────────────────┘
```

After opening:

```text
┌───────────────────────────────────────┐
│          Teachers' Day 2026       ♥️  │
│                                       │
│  [ Teacher Photo ]   Dear Sir Randy,  │
│                                       │
│  Thank you for every lesson...        │
│                                       │
│  Your guidance helped us...           │
│                                       │
│       ♥️ ───────────────── ♥️         │
│                                       │
│  With sincere appreciation...         │
│                                       │
│          Your Student ♥️              │
│                                       │
│          [ Close Letter ]             │
└───────────────────────────────────────┘
```

---

## 📄 License

This project is created for educational and personal use.

You are free to modify the design, message, colors, images, and animations for your own Teachers' Day project.

---

## 👨‍💻 Author

Created as a creative Web Development project using:

**HTML • CSS • JavaScript**

Made with ❤️ for **Sir Randy Bello**.

---

## ⭐ Support

If you like this project, consider giving the repository a ⭐ on GitHub!

Thank you for visiting! 💌
