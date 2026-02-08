# Node2Know — Pug Intro

A lightweight introduction to the **Pug** view engine (formerly Jade) for Node.js.

This demo demonstrates how to configure Express to use Pug and how to render basic, static views using Pug's clean, whitespace-sensitive syntax.

## 🚀 Core Concepts

### 1. Setup

- Configuring the view engine in `app.js`.
  ```javascript
  app.set("view engine", "pug");
  app.set("views", path.join(__dirname, "views"));
  ```

### 2. Syntax

- **Indentation**: Uses indentation (spaces/tabs) to define nesting, rather than closing tags.
- **Classes/IDs**: Uses `.className` and `#idName` shorthand, similar to CSS selectors.
- **Attributes**: attributes are defined in parentheses `(src="/img.png")`.

```pug
// Example
article.card
  h2 Welcome to Pug
  p.content No closing tags required!
```

---

## 🧭 Routes & Features

### Home (`/`)

- Renders `views/index.pug`.
- Demonstrates basic HTML structure in Pug (doctype, html, head, body).

### Things (`/things`)

- Renders `views/things.pug`.
- Shows a static list layout.

### Static Pages (`/about`, `/josh`)

- Demonstrates serving standard `.html` files alongside Pug views using `res.sendFile`.

---

## 📦 Install & Run

1.  **Install Dependencies**

    ```bash
    npm install
    ```

2.  **Start Server**

    ```bash
    npm run dev
    ```

3.  **Visit**
    - [http://localhost:3000](http://localhost:3000)

---

## 📁 Project Structure

```txt
.
├── app.js               # Express Application Entry
├── routers/             # Express Routers
├── views/
│   ├── index.pug        # Home view
│   └── things.pug       # Static list view
├── public/              # Static assets
└── README.md
```

---

## License

**Node2Know-LEARN-1.0**
