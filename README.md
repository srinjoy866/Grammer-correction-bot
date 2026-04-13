# ✨ DarkOllama GrammarBot

A sleek, dark-themed web application that uses **Ollama** to correct grammar, spelling, and punctuation in real-time — all running locally on your machine.

![DarkOllama GrammarBot](https://via.placeholder.com/800x400/09090b/8b5cf6?text=DarkOllama+GrammarBot+Screenshot)

## 🚀 Features

- **Real-time grammar correction** powered by local AI models
- **Dark mode UI** with smooth animations and gradients
- **Diff highlighting** — see what changed at a glance
- **Streaming output** — watch corrections appear word by word
- **Keyboard shortcuts** — `Ctrl+Enter` to submit
- **Copy to clipboard** with one click
- **Model selection** — choose from any installed Ollama model
- **Connection status indicator** — know when Ollama is reachable
- **Responsive design** — works on desktop and mobile

## 📋 Prerequisites

- [Ollama](https://ollama.com/) installed and running locally
- At least one language model downloaded (e.g., `llama3`, `mistral`, `phi3`)
- A modern web browser (Chrome, Firefox, Edge, Safari)

## 🛠️ Quick Start

### 1. Install Ollama

Visit [ollama.com](https://ollama.com/) and follow the installation instructions for your OS.

### 2. Download a Model

Open your terminal and pull a model:

```bash
ollama pull llama3
# or
ollama pull mistral
# or
ollama pull phi3
```

### 3. Start Ollama

Make sure the Ollama service is running. By default, it runs on `http://localhost:11434`.

### 4. Open the App

Simply open `index.html` in your browser:

```bash
# macOS
open index.html

# Linux
xdg-open index.html

# Windows
start index.html
```

## ⚙️ Configuration

| Setting | Description | Default |
|---------|-------------|---------|
| **Ollama URL** | The address of your Ollama instance | `http://localhost:11434` |
| **Model** | Select from available downloaded models | Auto-detected |

## ⌨️ Keyboard Shortcuts

| Shortcut | Action |
|----------|--------|
| `Ctrl + Enter` | Trigger grammar correction |

## 🎨 UI Customization

Edit the CSS variables in `index.html` to customize the theme:

```css
:root {
    --accent-color: #8b5cf6;     /* Change the primary accent color */
    --bg-color: #09090b;         /* Background color */
    --success-color: #10b981;    /* Highlight for additions */
    --error-color: #ef4444;      /* Highlight for removals */
}
```

## 🔧 Troubleshooting

### "Disconnected" status
- Ensure Ollama is running: visit `http://localhost:11434` in your browser
- Check if your model is downloaded: run `ollama list` in your terminal

### CORS errors
- Ollama may block browser requests by default. Start Ollama with:
  ```bash
  OLLAMA_ORIGINS="*" ollama serve
  ```

### No models appearing
- Run `ollama pull <model-name>` to download a model first

## 📁 Project Structure

```
grammer_correction_system/
├── index.html          # Main application (HTML + CSS + JS)
└── README.md           # This file
```

## 🤝 Contributing

Contributions are welcome! Feel free to open issues or submit pull requests.

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).

## 🙏 Acknowledgments

- [Ollama](https://ollama.com/) for making local AI accessible
- [Tailwind CSS color palette](https://tailwindcss.com/docs/customizing-colors) for the color scheme inspiration

---

**Built with ❤️ for clean writing**
