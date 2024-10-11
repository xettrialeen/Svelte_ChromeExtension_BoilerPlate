# Svelte Chrome Extension Boilerplate

This project is a boilerplate for creating Chrome extensions using Svelte and Vite. It provides a solid starting point for developers who want to leverage Svelte's reactive capabilities in their Chrome extensions.

## Features

- 🚀 Svelte for building reactive user interfaces
- ⚡ Vite for fast builds and hot module replacement
- 🎨 TailwindCSS for utility-first styling
- 🧩 Content script with injected Svelte component
- 🔄 Inter-script communication (popup to content script)
- 🏗️ Shadow DOM for isolated styling in content scripts

## Prerequisites

- Node.js (v14 or later recommended)
- npm (v6 or later)

## Getting Started

1. Clone this repository:
   ```
   git clone https://github.com/xettrialeen/Svelte_ChromeExtension_BoilerPlate.git
   cd svelte-chrome-extension-boilerplate
   ```

2. Install dependencies:
   ```
   npm install
   ```

3. Build the extension:
   ```
   npm run build
   ```

4. Load the extension in Chrome:
   - Open Chrome and navigate to `chrome://extensions`
   - Enable "Developer mode" in the top right corner
   - Click "Load unpacked" and select the `dist` directory in your project folder

## Development

- Run the development build with watch mode:
  ```
  npm run dev
  ```
  This will rebuild the extension automatically when you make changes.

- After making changes, you need to reload the extension in Chrome:
  - Go to `chrome://extensions`
  - Find your extension and click the refresh icon

## Project Structure

```
src/
├── popup/
│   ├── popup.html
│   ├── popup.js
│   └── App.svelte
├── content/
│   ├── content.js
│   └── ShadowComponent.svelte
├── background.js
└── app.css
public/
├── manifest.json
└── icon.png
```

- `popup/`: Contains the extension popup files
- `content/`: Contains the content script and injected Svelte component
- `background.js`: Background script for the extension
- `app.css`: Global styles and Tailwind imports
- `public/`: Contains static files like manifest.json and icons

## Building for Production

To create a production build, run:

```
npm run build
```

This will generate optimized files in the `dist` directory, ready for submission to the Chrome Web Store.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is open source and available under the [MIT License](LICENSE).

## Acknowledgements

- [Svelte](https://svelte.dev/)
- [Vite](https://vitejs.dev/)
- [TailwindCSS](https://tailwindcss.com/)
- [Chrome Extension Developer Guide](https://developer.chrome.com/docs/extensions/mv3/)

---

Happy coding! If you have any questions or run into issues, please open an issue in this repository.