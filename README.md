
<p align="center">
  <img src="./markskin_banner.png" alt="Markskin Banner" width="800">
</p>

<h1 align="center">Markskin</h1>
<h3 align="center">Style-Driven Markdown for the Modern Age</h3>

---

## 🌟 Features at a Glance

### **Text Styling**  
Add colors, gradients, shadows, and animations directly in Markdown:  
```markdown
🌈#FF5733→Orange Text  
⚫4px→Shadowed Heading  
💫glow 2s→Animated Alert
```

### **Layout Components**  
Build cards, grids, and sections without HTML:  
```markdown
(card:padding=20px,border=2px(
  ## 🗂️ Content Block  
  (bg:#f8f9fa→Highlighted text)  
  - List item  
  - [Button](https://example.com)
))
```

### **Theme Engine**  
Define reusable styles with custom themes:  
```markdown
@define my_theme {  
  primary: "#2ecc71",  
  danger: "#e74c3c",  
  header-gradient: "linear-gradient(45deg, #2ecc71, #3498db)"  
}  

(bg:header-gradient→Main Header)
```

---

## 🛠️ Syntax Essentials

### Basic Formatting
| Style          | Markskin Syntax               | Output Preview (Simplified)       |
|----------------|--------------------------------|------------------------------------|
| **Color**      | `🌈#FF5733→Text`              | <span style="color:#FF5733">Text</span> |
| **Background** | `(bg:#f0f0f0→Text)`           | <span style="background:#f0f0f0">Text</span> |
| **Shadow**     | `⚫5px→Text`                   | <span style="text-shadow:5px 2px 4px #000">Text</span> |
| **Bold**       | `🔶→Important Notice`         | **Important Notice**               |

### Advanced Features
```markdown
<!-- Nested Styles -->
🌈theme(primary)→(⚫2px→Styled Heading)

<!-- Responsive Grids -->
(grid:columns=3,gap=1rem(
  (card→Item 1)  
  (card→Item 2)  
  (card→Item 3)
))
```

---

## 🚀 Getting Started

1. **Download Files**:  
   - `markskin_parser.js` (core engine)  
   - `markskin_banner.png` (logo)  
   - `readme_plus.md` (advanced documentation)

2. **Basic Implementation**:  
```html
<!DOCTYPE html>
<html>
<head>
  <title>Markskin Demo</title>
  <script src="markskin_parser.js"></script>
</head>
<body>
  <script>
    const input = "(🌈#2ecc71→Welcome) to Markskin!";
    document.body.innerHTML = MarkskinParser.parse(input);
  </script>
</body>
</html>
```

---

## 🎨 Theming System

### Default Theme (Embedded)
```json
{
  "primary": "#007BFF",
  "secondary": "#6C757D",
  "success": "#28A745",
  "gradient-header": "linear-gradient(45deg, #007BFF, #00CED1)"
}
```

### Custom Theme File
Create `theme.json`:  
```json
{
  "brand-colors": {
    "main": "#FF6B6B",
    "accent": "#4ECDC4"
  }
}
```
Use in Markdown:  
```markdown
(bg:brand-colors.main→Primary Section)
```

---

## 🔒 Security & Validation

Markskin includes:  
- **Syntax Validation**: Rejects malformed tags  
- **CSS Sanitization**: Allows only safe properties  
- **Output Escaping**: Converts `<` and `>` to entities  

Example safety check:  
```javascript
if (input.includes("<script>")) {
  throw Error("Invalid content detected!");
}
```

---

## 📚 Extended Documentation

For advanced usage, custom components, and contributor guidelines:  
👉 See **[readme_plus.md](./readme_plus.md)**

---

## 📜 License

Developed by **Ferki**.  
Open-source under [MIT License](./LICENSE).

---

<p align="center">
  💡 Transform your Markdown today — no dependencies, no complexity!
</p>
``` 

This version:  
✅ **Zero external links** (only local file references)  
✅ **Self-contained documentation**  
✅ **Ready-to-use code snippets**  
✅ **Optional advanced guide** via `readme_plus.md`
