# gh-ozod-demoplay

Ozod Demo — kompaniya veb-saytining demo versiyasi. Oddiy va tushunarli HTML/CSS tuzilmasiga asoslangan statik veb-sahifa bo'lib, navigatsiya, login forma va footer bo'limlarini o'z ichiga oladi.

---

## 📋 Loyiha haqida

Bu loyiha — kompaniya veb-saytining dastlabki (demo) versiyasi. Asosiy maqsad: navigatsiya, login tugmasi va footer bo'lgan oddiy veb-sahifa yaratish.

---

## 🗂️ Fayl tuzilmasi

```
gh-ozod-demoplay/
├── index.html       # Asosiy sahifa (navigatsiya, login, footer)
├── style.css        # Stillar fayli
└── README.md        # Loyiha haqida ma'lumot
```

---

## 🧩 Tarkib

| Bo'lim     | Tavsif                                      |
|------------|---------------------------------------------|
| `<nav>`    | Kompaniya nomi va navigatsiya ro'yxati      |
| `<main>`   | Login sarlavhasi va tugma                   |
| `<footer>` | Kompaniya nomi, mualliflik huquqi va status |

---

## 🚀 Ishga tushirish

Loyihani ishga tushirish uchun hech qanday server kerak emas — to'g'ridan-to'g'ri brauzerda oching:

```bash
# 1. Reponi clone qiling
git clone https://github.com/diliraboeshboyev-crypto/gh-ozod-demoplay.git

# 2. Papkaga kiring
cd gh-ozod-demoplay

# 3. index.html faylini brauzerda oching
open index.html        # macOS
start index.html       # Windows
xdg-open index.html    # Linux
```

---

## 🛠️ Ishlatilgan texnologiyalar

- **HTML5** — sahifa tuzilmasi
- **CSS3** — stillar (`style.css` orqali)

---

## ⚠️ Aniqlangan xatolar (Bug Report)

Kodda quyidagi xatolar mavjud bo'lib, tuzatish tavsiya etiladi:

### 1. `<div>` tegida noto'g'ri atribut
```html
<!-- ❌ Xato -->
<div style="container">

<!-- ✅ To'g'ri -->
<div class="container">
```

### 2. `<ul>` tegi yopilmagan
```html
<!-- ❌ Xato: <ul> yopilmagan, ichki <ul> ham noto'g'ri -->
<ul>
    <li>Home</li>
    <li>page</li>
    <li>disabled</li>
<ul>   ← bu yopish tegi emas, yangi ochish tegi!

<!-- ✅ To'g'ri -->
<ul>
    <li>Home</li>
    <li>Page</li>
    <li>Disabled</li>
</ul>
```

### 3. `&copy:` entity noto'g'ri yozilgan
```html
<!-- ❌ Xato -->
<p>&copy:copyright2026</p>

<!-- ✅ To'g'ri -->
<p>&copy; 2026 Company. All rights reserved.</p>
```

### 4. `<title>` bo'sh qoldirilgan
```html
<!-- ❌ Xato -->
<title></title>

<!-- ✅ To'g'ri -->
<title>Ozod Demo — Company</title>
```

### 5. Imlo xatosi — "Compamiy"
```html
<!-- ❌ Xato -->
<h3>Compamiy</h3>

<!-- ✅ To'g'ri -->
<h3>Company</h3>
```

---

## ✅ Tuzatilgan HTML kodi

Barcha xatolar tuzatilgan to'liq kod:

```html
<!doctype html>
<html lang="en">
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>Ozod Demo — Company</title>
    <link rel="stylesheet" href="style.css">
  </head>
  <body>
    <div class="container">

      <nav>
        <h1>Company</h1>
        <ul>
          <li>Home</li>
          <li>Page</li>
          <li>Disabled</li>
        </ul>
      </nav>

      <main>
        <h2>Login Form</h2>
        <hr>
        <button>Click to Login</button>
      </main>

      <footer>
        <h3>Company</h3>
        <p>&copy; 2026 Company. All rights reserved.</p>
        <p>Status: Active</p>
      </footer>

    </div>
  </body>
</html>
```

---

## 📌 Kelajakdagi rejalar (To-do)

- [ ] Login formaga `<form>`, `<input>` va parol maydoni qo'shish
- [ ] `style.css` faylini to'ldirish (responsive dizayn)
- [ ] Navigatsiya havolalarini `<a>` teglari bilan bog'lash
- [ ] JavaScript orqali login funksiyasini ulash
- [ ] Sahifani GitHub Pages orqali deploy qilish

---

## 👤 Muallif

**diliraboeshboyev-crypto**
GitHub: [@diliraboeshboyev-crypto](https://github.com/diliraboeshboyev-crypto)

---

## 📄 Litsenziya

MIT License — bepul foydalanish va tarqatish mumkin.
