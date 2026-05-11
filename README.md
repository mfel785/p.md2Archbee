# p.md2Archbee

## 📄 Overview
**p.md2Archbee** is a lightweight, browser-based tool that converts **Markdown files exported from Paligo** into a format compatible with **Archbee**.

The tool runs entirely in the browser — no data is uploaded, stored, or processed on a server.

---

## Features

- Removes Paligo UUID artifacts (`<span id="UUID-...">`)
- Converts Paligo admonitions (`> [!NOTE]`, `> [!WARNING]`, etc.)
  → into Archbee `:::hint` blocks
- Supports multiple consecutive hints
- Preserves:
  - paragraphs
  - lists
  - indentation
- Converts hard line breaks into readable text
- Works offline (pure HTML + JavaScript)

---

## Supported Hint Types

| Paligo    | Archbee |
|----------|--------|
| NOTE     | info   |
| IMPORTANT| info   |
| TIP      | tip    |
| WARNING  | warning|
| CAUTION  | warning|
| DANGER   | danger |

---

## How to Use

Here's how it works

1. Click "Select File."
2. Select the Markdown file you want to optimize.
3. Click "Adjust Markdown File."

The file will be optimized and then automatically downloaded.

---

## Deployment (GitHub Pages)

1. Create a repository  
2. Upload `index.html` to the root  
3. Go to:  
   Settings → Pages  

4. Set:  
   Source: Deploy from branch  
   Branch: main / (root)  

5. Access your tool:  
   https://<username>.github.io/<repository>/

---

## Security

- Runs completely in the browser  
- No external API calls  
- No data storage  
- No data transmission  

---

## Technical Details

- HTML5, CSS3, Vanilla JavaScript  
- Uses FileReader API  
- Uses Blob API for downloads  
- No dependencies  

---

## Known Limitations

- Only supports standard Paligo admonition syntax (`> [!TYPE]`)  
- Nested blockquotes (`>>`) are not fully supported  
- Very complex Markdown structures may need manual adjustment  

---

## Possible Enhancements

- Drag & Drop upload  
- Additional Markdown transformations  
- More hint types  
- UI improvements  
- Batch processing  

---

## Author

**mfel**  
Created: 2026-05-07  

---

## Version

v1.0 – Initial Release
