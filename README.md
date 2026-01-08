# 🫙 Waiter Tip Distribution System

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Live-success?style=for-the-badge)
![Privacy](https://img.shields.io/badge/Privacy-Local_Storage-blue?style=for-the-badge&logo=adguard)

---

## 📑 Table of Contents
- [🚀 Introduction](#-introduction)
- [🌐 Live Demo](#-live-demo)
- [✨ Key Features](#-key-features)
- [⚡ Detailed Workflow](#-detailed-workflow)
- [🛠️ Tech Stack](#️-tech-stack)
- [⚙️ Self-Hosting Guide](#️-self-hosting-guide)
- [🌟 Future Enhancements](#-future-enhancements)
- [🤝 Contributing](#-contributing)
- [📜 License](#-license)

---

## 🚀 Introduction
End-of-shift mathematics should not be a headache.  
**The Tip Jar** is a modern, lightweight web application designed to transform the chaotic process of distributing gratuities into a **seamless, fair, and transparent** operation. 

Whether you manage a small cafe or a bustling restaurant, this tool ensures every staff member gets their fair share based on precise weighting factors, all while keeping your data 100% private on your own device.

---

## 🌐 Live Demo
Experience the application live at:  
👉 **[https://jar.alfanitaf.duckdns.org](https://jar.alfanitaf.duckdns.org)**

---

## ✨ Key Features
1. ⚖️ **Weighted Distribution Algorithm** – Fairly calculate shares based on staff seniority or hours worked using adjustable weight factors.
2. 💾 **Zero-Knowledge Persistence** – All data is saved instantly to **LocalStorage**. No external databases, no cloud uploads, 100% privacy.
3. 📊 **Professional Reporting** – One-click export to **Excel (.xlsx)** with detailed breakdowns for accounting.
4. 🌍 **Polyglot Interface** – Instant toggle between **English** 🇬🇧 and **Greek** 🇬🇷.
5. 🎨 **Glassmorphism UI** – A sleek, responsive, and modern interface that works perfectly on mobile and desktop.

---

## ⚡ Detailed Workflow
✅ **Step 1** – **Configure Staff**: Input waiter names and assign weight factors (e.g., 1.0 for full share, 0.5 for half).  
✅ **Step 2** – **Daily Entry**: Select the date and input the total cash tips collected.  
✅ **Step 3** – **Selection**: Check the boxes for who worked that specific shift.  
✅ **Step 4** – **Calculation**: Instant real-time preview of the split.  
✅ **Step 5** – **Archive**: Save the entry to history and Export to Excel at the end of the month.

---

## 🛠️ Tech Stack
This project utilizes a lightweight, dependency-free architecture:

* **Core:** HTML5, CSS3 (Custom Glassmorphism), Vanilla JavaScript.
* **Libraries:** `SheetJS` (xlsx) for data export.
* **Storage:** Browser LocalStorage API.
* **Icons:** SVG & CSS Animations.

---

## ⚙️ Self-Hosting Guide
Want to run this on your own Ubuntu/Apache server?

**1. Clone the repo:**
```bash
git clone [https://github.com/avasileios/tip-distribution-app.git](https://github.com/avasileios/tip-distribution-app.git)
sudo mkdir -p /var/www/jar
sudo cp tip-distribution-app/index.html /var/www/jar/

```

**2. Configure Apache (`/etc/apache2/sites-available/jar.conf`):**

```apache
<VirtualHost *:80>
    ServerName your.domain.com
    DocumentRoot /var/www/jar
    <Directory /var/www/jar>
        Options -Indexes +FollowSymLinks
        AllowOverride All
        Require all granted
    </Directory>
</VirtualHost>

```

**3. Enable & Secure:**

```bash
sudo a2ensite jar.conf
sudo systemctl reload apache2
sudo certbot --apache -d your.domain.com

```

---

## 🌟 Future Enhancements

* 🌓 **Dark/Light Mode** – Toggle themes for late-night shifts.
* 📅 **Date Range Filters** – Custom filtering for history exports.
* 📈 **Visual Analytics** – Charts to track tipping trends over time.

---

## 🤝 Contributing

Contributions are welcome!

Please submit a pull request or open an issue to discuss improvements or features.

---

## 📜 License

This project is licensed under the **MIT License**.

---

<div align="center">
<sub>Created with ❤ by <a href="https://www.google.com/search?q=https://alfanitaf.duckdns.org">Vasileios Antonopoulos</a></sub>
</div>
