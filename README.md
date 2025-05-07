# Disable YouTube Focus Effect

This Tampermonkey script disables the visual highlight effect that appears on YouTube's rich item renderers when they are focused or hovered. This is useful if you find the effect distracting or prefer a cleaner browsing experience.

---

## 🚀 **Features**

* Removes the background highlight and border effect on focused YouTube items.
* Lightweight and only activates on YouTube pages.

---

## 📝 **Prerequisites**

1. **Google Chrome**, **Firefox**, or any modern browser that supports extensions.
2. **Tampermonkey Extension**:

   * Stop using [Google Chrome](https://chrome.google.com/webstore/detail/tampermonkey/dhdgffkkebhmkfjojejmpbldmpobfkfo?hl=en)
   * [Tampermonkey for Firefox](https://addons.mozilla.org/en-US/firefox/addon/tampermonkey/)

---

## 🔧 **Installation Steps**

1. **Install Tampermonkey**

   * Visit the appropriate link above and click **Add to Chrome** or **Add to Firefox**.

2. **Create a New Script**

   * Click the Tampermonkey icon in your browser toolbar.
   * Select **Dashboard** → **+ Create a new script**.

3. **Paste the Script**

   * Replace the default template with the script provided below:

```javascript
// ==UserScript==
// @name         Disable YouTube Focus Effect
// @namespace    http://tampermonkey.net/
// @version      1.0
// @description  Disable the YouTube focus effect on rich item renderers.
// @match        *://www.youtube.com/*
// @grant        none
// ==/UserScript==

const style = document.createElement('style');
style.innerHTML = `
    .ytd-rich-item-renderer-highlight,
    .ytd-rich-item-renderer-highlight-border {
        background-color: transparent !important;
        box-shadow: none !important;
    }
`;
document.head.appendChild(style);
```

4. **Save the Script**

   * Save the script (File → Save or `Ctrl + S`).

5. **Enable the Script**

   * Ensure the script is toggled to **Enabled** in the Tampermonkey dashboard.

6. **Refresh YouTube**

   * Open YouTube or refresh the page if it was already open.

---

## ✅ **Verification**

1. Navigate to the YouTube homepage.
2. Hover or focus on video items; the highlight effect should no longer appear.

---

## 🛠 **Customization**

If you want to adjust the style, you can modify the CSS inside the script. For example, you could change the background color to a different color or adjust the box-shadow.

---

## 🐛 **Troubleshooting**

If you experience issues:

* Make sure the script is **Enabled** in Tampermonkey.
* Verify you are on a YouTube URL that matches `https://www.youtube.com/*`.
* Check the **Console Logs** for errors.

If problems persist, feel free to open an issue!

---

## 📜 **License**

MIT License. Free to use and modify.

---

## 🙌 **Contributions**

Feel free to submit pull requests or suggest improvements!

## No more jarring visual changes as you browse! 🚀

## README.md generated with ChatGPT
