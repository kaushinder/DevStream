# DevTinder UI 🚀

### React + Vite + TailwindCSS (Stable Setup – No Version Conflicts)

This project sets up the **DevTinder UI** using **React, Vite, and TailwindCSS** with stable versions that avoid dependency conflicts.

---

## 🛠 Tech Stack

* React
* Vite
* TailwindCSS
* PostCSS
* Autoprefixer

---

## 📦 Stable Versions

| Package              | Version |
| -------------------- | ------- |
| vite                 | ^7      |
| @vitejs/plugin-react | ^5      |
| tailwindcss          | ^3.4    |
| postcss              | latest  |
| autoprefixer         | latest  |

---

# ⚙️ Setup Guide

<details>
<summary>1️⃣ Create Vite React Project</summary>

```bash
npm create vite@latest devTinder-UI
```

Select:

```
Framework: React
Variant: JavaScript
```

Then install dependencies:

```bash
cd devTinder-UI
npm install
```

</details>

---

<details>
<summary>2️⃣ Install Compatible React Plugin</summary>

```bash
npm install @vitejs/plugin-react@5
```

</details>

---

<details>
<summary>3️⃣ Install TailwindCSS</summary>

```bash
npm install -D tailwindcss@3.4 postcss autoprefixer
```

</details>

---

<details>
<summary>4️⃣ Generate Tailwind Config</summary>

```bash
npx tailwindcss init -p
```

This creates:

```
tailwind.config.js
postcss.config.js
```

</details>

---

<details>
<summary>5️⃣ Configure Tailwind</summary>

Edit **tailwind.config.js**

```javascript
/** @type {import('tailwindcss').Config} */
export default {
  content: [
    "./index.html",
    "./src/**/*.{js,ts,jsx,tsx}"
  ],
  theme: {
    extend: {},
  },
  plugins: [],
}
```

</details>

---

<details>
<summary>6️⃣ Add Tailwind to CSS</summary>

Edit **src/index.css**

```css
@tailwind base;
@tailwind components;
@tailwind utilities;
```

</details>

---

<details>
<summary>7️⃣ Configure Vite</summary>

Edit **vite.config.js**

```javascript
import { defineConfig } from 'vite'
import react from '@vitejs/plugin-react'

export default defineConfig({
  plugins: [react()],
})
```

</details>

---

<details>
<summary>8️⃣ Test Tailwind Setup</summary>

Edit **src/App.jsx**

```jsx
function App() {
  return (
    <h1 className="text-4xl font-bold text-red-500">
      DevTinder Tailwind Working 🚀
    </h1>
  )
}

export default App
```

</details>

---

<details>
<summary>9️⃣ Run the Project</summary>

```bash
npm run dev
```

</details>

---

# 📁 Project Structure

```
devTinder-UI
│
├── public
├── src
│   ├── App.jsx
│   ├── main.jsx
│   ├── index.css
│
├── index.html
├── package.json
├── tailwind.config.js
├── postcss.config.js
└── vite.config.js
```

---

# 🔧 Useful Commands

```bash
npm install
npm run dev
npm run build
npm run preview
```

---

# 👨‍💻 Author

**Kaushinder Singh Raghav**
MCA (AI & Machine Learning) – Galgotias University
Aspiring **MERN Stack Developer**
