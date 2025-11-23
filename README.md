
# Access to full customization of VS Code

Open your `settings.json` in vs code and paste this [Settings](./settings.json).

Necessary Files to download :

## 🖋️ Fonts & Typography

* [Dank Mono Regular](DankMono-Regular.otf)
* [Dank Mono Italic](DankMono-Italic.otf)
* [Dank Mono Bold](DankMono-Bold.otf)

* [JetBrains Mono Regular](JetBrainsMono-Regular.ttf)
* [JetBrains Mono Italic](JetBrainsMono-Italic.ttf)
* [JetBrains Mono](JetBrainsMono-Bold.ttf)

* [Fira Code](FiraCode-Regular.ttf)

---

## ✅ Extension recommended

* **One Dark Pro** — theme
* **Material Icon Theme** — file icons
* **Prettier - Code formatter** — formatting
* **ESLint** — linting + fixes on save
* **Java Extension Pack** (or **Red Hat Java**) — if you work with Java (formatter referenced)
* **C/C++ (ms-vscode.cpptools)** — if you work with C (formatter referenced)

## 🔎 What this settings file does (quick summary)

* Sets **One Dark Pro** theme and **material icon theme**.
* Uses larger, readable editor fonts and enables ligatures.
* Enables bracket pair colorization, smooth caret animation, and nicer line heights/spaces for comfort.
* Uses **Prettier** as default formatter and formats on save.
* Runs ESLint on save and enables import/fix-on-save actions.
* Tailwind CSS IntelliSense & Emmet tweaks for React/TSX.
* Terminal defaults (bash on Linux) and font settings for integrated terminal.
* UI layout: sidebar/panel on the right, activity bar default.
* Disables some “noisy” features (minimap off, sticky scroll off, breadcrumbs off).
* Some language-specific default formatters (Java, C).

---

**What to do:**

* If you own **Dank Mono**, install it system-wide and the editor will pick it up.
* If not, install **JetBrains Mono** or **Fira Code** (both free) — they work great and support ligatures.
* After installing a font, restart VS Code to pick it up.

**Terminal font:** Terminal uses `JetBrains Mono` as a fallback — you can change it (same installation process).

---

## ⚙️ Key settings you may want to tweak

* `workbench.colorTheme` — change if you prefer another theme.
* `workbench.iconTheme` — change if you prefer other icons.
* `editor.fontSize`, `editor.lineHeight`, `editor.fontFamily` — tweak to taste (especially if your monitor DPI differs).
* `livePreview.defaultPreviewPath` — must be changed to your local file path if you use Live Preview.
* `terminal.integrated.defaultProfile.linux` — change to `zsh` if you use Zsh.

---

## 📁 How to apply this `settings.json`

1. Open VS Code.
2. Press `Ctrl+Shift+P` → **Preferences: Open Settings (JSON)**.
3. Replace the contents with your `settings.json` (or merge the keys you want).
4. Save and restart VS Code.

---

## 🔧 Troubleshooting

* **Font not applied?** Restart VS Code. Make sure the font is installed system-wide. Double-check spelling in `editor.fontFamily`.
* **Extensions not working?** Reinstall extension and reload the window (Ctrl+Shift+P → Developer: Reload Window).
* **Prettier/ESLint conflicts?** Ensure `editor.defaultFormatter` points to Prettier for the languages you want, and that ESLint’s autofix rules don’t conflict with Prettier (use `eslint-config-prettier` to avoid rule clashes).
* **Live Preview path wrong?** Update `livePreview.defaultPreviewPath` to a valid HTML file path on your machine.

## ❤️ Final tips

* Tweak `editor.fontSize`, `lineHeight`, and `tabSize` to your comfort — small changes make big UX improvements.
* Install the recommended extensions, restart, and give your eyes a few days to get used to the theme + fonts.
* If you want, I can create a minimal `extensions.json` (workspace recommendations) you can add to your repo so teammates get the same extension suggestions.
