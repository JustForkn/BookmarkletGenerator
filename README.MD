# 🤖 Bookmarklet AI

> Generate custom browser bookmarklets using AI and Groq.

Bookmarklet AI is a simple GitHub Pages website that lets you describe what you want a bookmarklet to do, sends the request to Groq, and returns **only a ready-to-use JavaScript bookmarklet**.

## ✨ Features

* 🤖 AI-powered bookmarklet generation
* ⚡ Powered by Groq
* 🔖 Generates bookmarklets only
* 📋 One-click **Copy** button
* 🌐 Works as a static GitHub Pages site
* 📄 Everything runs from a single `index.html`
* ⌨️ `Ctrl + Enter` / `Cmd + Enter` generates a bookmarklet
* 🖥️ Dark modern interface
* 📱 Mobile responsive

## 🚀 Setup

### 1. Download or clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/YOUR_REPOSITORY.git
```

### 2. Open `index.html`

Find this line:

```js
const GROQ_API_KEY = "";
```

Put your Groq API key between the quotes:

```js
const GROQ_API_KEY = "gsk_your_key_here";
```

### 3. Open the website

You can run `index.html` locally or publish the repository with GitHub Pages.

## 🌐 GitHub Pages

1. Upload `index.html` and `README.md` to your repository.
2. Open your repository on GitHub.
3. Go to **Settings**.
4. Open **Pages**.
5. Under **Build and deployment**, select your branch.
6. Save.
7. GitHub will provide your website URL.

## 🧠 How It Works

Enter a request such as:

```text
Make a bookmarklet that adds a draggable dark mode button to any website.
```

The site sends the request to Groq and asks the model to return:

```text
javascript:...
```

The generated bookmarklet appears in the output box.

Click:

```text
Copy
```

and paste it into a browser bookmark.

## 🔑 API Key

The API key is configured in:

```js
const GROQ_API_KEY = "";
```

You can also temporarily enter a key in the API-key box on the website.

### ⚠️ Important

If you put your Groq API key directly into `index.html` and upload it to a **public GitHub repository**, anyone can view the key in your source code.

For a public production site, use a backend/serverless proxy instead of exposing the key in client-side JavaScript.

## ⚙️ Configuration

The Groq model can be changed here:

```js
const GROQ_MODEL = "openai/gpt-oss-120b";
```

The API endpoint is configured here:

```js
const GROQ_ENDPOINT =
    "https://api.groq.com/openai/v1/chat/completions";
```

## 📁 Files

```text
/
├── index.html
└── README.md
```

## 🛠️ Example Requests

Try requests like:

```text
Make a bookmarklet that changes every webpage background to black.
```

```text
Make a bookmarklet that adds a floating calculator to the current page.
```

```text
Make a bookmarklet that highlights every link on the page.
```

```text
Make a bookmarklet that adds a button that scrolls to the bottom of the page.
```

```text
Make a bookmarklet that shows the current page URL in a popup.
```

## 📜 License

Use, modify, and customize this project according to the license you choose for your repository.

---

### ⭐ Bookmarklet AI

**Describe it → Generate it → Copy it → Bookmark it.**
