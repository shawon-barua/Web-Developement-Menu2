# Ristorante Con Fusion — Front-End Web Development (AngularJS)

A front-end web application for a fictional restaurant named **Ristorante Con Fusion**, developed as part of the AngularJS course module.

---

## 🍽️ About the Project

**Ristorante Con Fusion** is a dynamic web application built using **AngularJS (1.x)** and **Bootstrap 3**. It showcases a rich user experience for restaurant browsing, menu exploration, dish reviews/ratings, and contact form handling with client-side form validation.

### ✨ Key Features

- **Dynamic Menu Page (`menu.html`)**:
  - Filter dishes by category (*All*, *Appetizers*, *Mains*, *Desserts*).
  - Toggle dish description visibility (*Show / Hide Details*).
  - Real-time price and special badges display.
- **Dish Detail & Reviews (`dishdetail.html`)**:
  - Detailed dish view with customer ratings and comments.
  - Interactive comment submission form with real-time form validation.
  - Live preview of comments as the user types before submission.
- **Contact & Feedback (`contactus.html`)**:
  - Structured feedback form with AngularJS two-way data binding.
  - Validation for feedback channel selection (Email vs. Phone).
- **Service Layer Architecture**:
  - Organized modular code using `confusionApp`.
  - `menuFactory` service (`services.js`) providing centralized data management for dishes and comments.
  - Dedicated controllers (`controllers.js`) for menu management, dish details, comment submission, and feedback.

---

## 🛠️ Tech Stack & Tools

- **Framework**: [AngularJS 1.4.x](https://angularjs.org/)
- **UI & Styling**: [Bootstrap 3.3.5](https://getbootstrap.com/), [Font Awesome 4.4.0](https://fontawesome.com/)
- **Package Management**:
  - [npm](https://www.npmjs.com/) (Build tools & dev dependencies)
  - [Bower](https://bower.io/) (Client-side libraries)
- **Build & Task Runners**:
  - [Gulp](https://gulpjs.com/) (Concat, Minification, Image Optimization, Uglify, BrowserSync)
  - [Grunt](https://gruntjs.com/) (Alternative build automation configuration)
- **Linting**: JSHint

---

## 📂 Project Structure

```text
confusionweek2/
├── app/                      # Application source files
│   ├── images/               # Image assets
│   ├── scripts/              # Angular JavaScript files
│   │   ├── app.js            # Main Angular module initialization
│   │   ├── controllers.js    # Angular controllers (Menu, Dish, Feedback, etc.)
│   │   └── services.js       # Angular services (menuFactory)
│   ├── styles/               # Custom CSS styles
│   ├── contactus.html        # Contact Us & feedback page
│   ├── dishdetail.html       # Dish detail and comments page
│   └── menu.html             # Main restaurant menu page
├── dist/                     # Production distribution build (generated)
├── Gruntfile.js              # Grunt task runner configuration
├── gulpfile.js               # Gulp task runner configuration
├── package.json              # Node.js dependencies and project metadata
├── bower.json                # Bower client-side dependencies
└── .gitignore                # Git ignore rules
```

---

## 🚀 Getting Started

### Prerequisites

Ensure you have Node.js, npm, and Bower installed:
- [Node.js](https://nodejs.org/) (v10+ recommended for legacy Gulp 3/Grunt compatibility)
- [Bower](https://bower.io/) (`npm install -g bower`)
- [Gulp CLI](https://gulpjs.com/) / [Grunt CLI](https://gruntjs.com/)

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/shawon-barua/confusionweek2.git
   cd confusionweek2
   ```

2. **Install Node dependencies:**
   ```bash
   npm install
   ```

3. **Install Bower components:**
   ```bash
   bower install
   ```

### Running the Application

- **Quick Local Server (Recommended):**
  ```bash
  npx serve .
  # or
  npx http-server . -p 8080 -o
  # or
  python -m http.server 8000
  ```
  Then visit:
  - **Menu Page:** `http://localhost:3000/app/menu.html`
  - **Dish Detail & Comments:** `http://localhost:3000/app/dishdetail.html`
  - **Contact Us:** `http://localhost:3000/app/contactus.html`

- **With Gulp (Live development server & watch):**
  ```bash
  gulp watch
  ```
  or build the distribution:
  ```bash
  gulp
  ```

- **With Grunt:**
  ```bash
  grunt serve
  ```
  or build the distribution:
  ```bash
  grunt
  ```

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).
