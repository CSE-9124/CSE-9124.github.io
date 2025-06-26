---
title: "♻️ PILASAKI' - Pilah Sampah Kita"
date: 2024-10-27 00:00:00 +0800
categories: [Website, Project]
tags: [Website, HTML, CSS, Bootstarp, Javascript, PHP, Laravel, MYSQL]
image: 
    path: /assets/images/posts/pilasaki/AppThumbnail.png
    alt: PILASAKI' Thumbnail
---
<div align="center">

  <img src="/assets/images/posts/pilasaki/top.jpg" alt="PILASAKI Banner">

  <p><strong>🏆 FINALIS ICONIC IT 2024</strong></p>

  <img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white" alt="Git"/>
  <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" />
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5"/>
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3"/>
  <img src="https://img.shields.io/badge/Bootstrap-7952B3?style=for-the-badge&logo=bootstrap&logoColor=white" alt="Bootstrap"/>
  <img src="https://img.shields.io/badge/TensorFlow.js-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white" alt="TensorFlow.js"/>
  <img src="https://img.shields.io/badge/PHP-777BB4?style=for-the-badge&logo=php&logoColor=white" alt="PHP"/>
  <img src="https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white" alt="MySQL"/>
  <img src="https://img.shields.io/badge/Laravel-FF2D20?style=for-the-badge&logo=laravel&logoColor=white" alt="Laravel"/>

  <p><em>Website Edukasi Pengelolaan Sampah untuk Indonesia yang Berkelanjutan</em></p>

  <p><a href="https://github.com/PeterChen712/Pilasaki">🔗 Repository</a> • <a href="#-screenshots--demo">🌐 Live Demo</a></p>

</div>

---

## 🎯 About PILASAKI

> **PILASAKI** (Pilah Sampah Kita) adalah platform web inovatif yang dikembangkan untuk **ICONIC IT 2024**, bertujuan meningkatkan kesadaran masyarakat tentang pengelolaan sampah melalui teknologi modern dan pendekatan edukatif yang menarik.

### 🌍 Visi & Misi

**🎯 Visi**
- Menciptakan Indonesia yang bersih dan berkelanjutan melalui edukasi pengelolaan sampah

**📋 Misi**
- ✅ Meningkatkan pemahaman masyarakat tentang jenis sampah dan cara pengelolaannya
- ✅ Menyediakan artikel informatif dan terkini mengenai pengelolaan sampah  
- ✅ Mendukung Tujuan Pembangunan Berkelanjutan (SDGs) dalam pendidikan dan keberlanjutan kota

---

## 🚀 Fitur Unggulan

### 📚 **1. Sistem Manajemen Konten Artikel**
- 📝 Kategorisasi artikel yang terstruktur
- 🔍 Fitur pencarian canggih
- 📖 Riwayat artikel yang telah dibaca
- 🏷️ Tag dan filtering yang mudah

### 🤖 **2. Klasifikasi Sampah Otomatis dengan AI**
- 🧠 Powered by **TensorFlow.js**
- 📸 Upload gambar untuk analisis otomatis
- 🎯 Identifikasi kategori sampah secara real-time
- 💡 Saran pengelolaan berdasarkan jenis sampah

### 💬 **3. Forum Diskusi Interaktif**
- 🗣️ Platform diskusi antar pengguna
- 📢 Berbagi pengalaman dan tips
- 🤝 Komunitas peduli lingkungan
- ⭐ System rating dan feedback

---

## 🛠️ Tech Stack

| **Category** | **Technology** | **Purpose** |
|:---:|:---:|:---:|
| **Backend** | Laravel 11 | Web Framework |
| **Frontend** | Blade Templates | Server-side Rendering |
| **Styling** | TailwindCSS | Modern CSS Framework |
| **Database** | MySQL | Data Storage |
| **AI/ML** | TensorFlow.js | Image Classification |
| **Build Tool** | Vite | Asset Bundling |
| **Authentication** | Laravel Socialite | Social Login |
| **Image Processing** | Intervention Image | Image Manipulation |

### 📦 Dependencies Highlight

```json
{
  "backend": {
    "laravel/framework": "^11.9",  
    "intervention/image": "^3.7",
    "laravel/socialite": "^5.15",  
    "anhskohbo/no-captcha": "^3.6"
  },
  "frontend": {
    "tailwindcss": "^3.4.14",
    "vite": "^5.0",
    "axios": "^1.6.4"
  }
}
```

---

## 🎨 Screenshots & Demo

### 🏠 Homepage & Dashboard
<p align="center"><em>Clean, modern interface dengan navigasi yang intuitif</em></p>

![Dashboard](/assets/images/posts/pilasaki/home.png)

### 📖 Content Management
<p align="center"><em>Sistem artikel dengan kategorisasi dan pencarian yang powerful</em></p>

![Artikel Feature](/assets/images/posts/pilasaki/artikel.png)

### 🤖 AI Classification
<p align="center"><em>Machine learning untuk klasifikasi sampah otomatis</em></p>

![AI Classification Demo](/assets/images/posts/pilasaki/demoAI.gif)

![Classification Interface](/assets/images/posts/pilasaki/klasifikasi.png)

### 💬 Community Forum  
<p align="center"><em>Platform diskusi untuk membangun komunitas</em></p>

![Forum Discussion](/assets/images/posts/pilasaki/diskusi.png)

---

## 🚀 Quick Start

### 📋 Prerequisites
- PHP >= 8.2
- Composer
- Node.js & NPM
- MySQL
- XAMPP (recommended)

### 🔧 Installation

```bash
# 1. Clone repository
git clone https://github.com/PeterChen712/Pilasaki.git
cd Pilasaki

# 2. Install PHP dependencies
composer install

# 3. Setup environment
cp .env.example .env
php artisan key:generate

# 4. Install Node dependencies  
npm install

# 5. Configure database (.env file)
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=pilasaki
DB_USERNAME=root
DB_PASSWORD=

# 6. Run migrations & seed data
php artisan migrate
php artisan db:seed

# 7. Build assets
npm run build

# 8. Start development server
php artisan serve
```

### 🌐 Access Application
Open your browser and visit: `http://localhost:8000`

---

## 🏗️ Project Structure

```
pilasaki/
├── 📁 app/                    # Laravel application logic
│   ├── Http/Controllers/      # Request handlers
│   ├── Models/               # Eloquent models
│   └── Services/             # Business logic
├── 📁 database/              # Database files
│   ├── migrations/           # Database schema
│   └── seeders/             # Sample data
├── 📁 public/               # Public assets
├── 📁 resources/            # Frontend resources
│   ├── views/               # Blade templates
│   ├── css/                 # Stylesheets
│   └── js/                  # JavaScript files
├── 📁 routes/               # Application routes
└── 📁 storage/              # File storage
```

---

## 🎯 SDGs Alignment

| **SDG Goal** | **Our Impact** |
|:---:|:---:|
| **🎓 Quality Education** | Platform edukasi sampah interaktif |
| **🏙️ Sustainable Cities** | Solusi pengelolaan sampah perkotaan |
| **🌍 Climate Action** | Mengurangi dampak lingkungan |
| **♻️ Responsible Consumption** | Edukasi pola konsumsi berkelanjutan |

---

## 🏆 ICONIC IT 2024 Journey

### 🗓️ Competition Timeline

| **Phase** | **Date** | **Milestone** |
|:---:|:---:|:---:|
| **📝 Registration** | Nov 2024 | Tim terdaftar |
| **💡 Ideation** | Dec 2024 | Konsep PILASAKI |
| **⚡ Development** | Jan 2025 | MVP Development |
| **🎯 Submission** | Feb 2025 | **FINALIST!** |

### 🎖️ Achievement
- **🏆 FINALIST** - Top 10 Web Development Competition
- **💡 Innovation Award** - AI Integration Excellence  
- **🌱 Social Impact Recognition** - Environmental Solution

---

## 🚀 Key Features Deep Dive

### 🤖 AI-Powered Waste Classification

**How it works:**
1. 📸 User uploads waste image
2. 🧠 TensorFlow.js processes image
3. 🎯 AI identifies waste category
4. 💡 System provides disposal recommendations
5. 📊 Analytics tracks classification patterns

**Supported Categories:**
- ♻️ Recyclable (Plastic, Paper, Metal)
- 🗑️ Non-recyclable 
- ☣️ Hazardous waste
- 🌿 Organic waste

### 📚 Smart Content Management

**Features:**
- 🏷️ **Auto-tagging** - AI-suggested tags
- 🔍 **Advanced Search** - Full-text search with filters
- 📈 **Analytics** - Reading patterns and popular content
- 📱 **Mobile-first** - Responsive design

### 💬 Community Engagement

**Community Features:**
- 👥 User profiles and achievements
- 💬 Threaded discussions
- ⭐ Reputation system
- 🏆 Gamification elements

---

## 🔮 Future Roadmap

### 🎯 Phase 2 (Q2 2025)
- [ ] 📱 Mobile App Development (Flutter)
- [ ] 🌐 Multi-language Support
- [ ] 📊 Advanced Analytics Dashboard
- [ ] 🤖 Chatbot Integration

### 🎯 Phase 3 (Q3 2025)
- [ ] 🚛 Waste Collection Scheduling
- [ ] 🏪 Marketplace for Recycled Products
- [ ] 🎮 Gamification & Rewards System
- [ ] 🌏 Regional Expansion

---

## 👥 Team

<div align="center">

  <p><strong>Tim Developer PILASAKI</strong></p>
  <img src="/assets/images/posts/pilasaki/Team.png" alt="Team"/>
  <p><em>Web Development Competition ICONIC IT 2024</em></p>

</div>

---

## 🤝 Contributing

Kami welcome kontribusi dari komunitas! Silakan:

1. 🍴 Fork repository
2. 🌿 Create feature branch (`git checkout -b feature/AmazingFeature`)
3. 💾 Commit changes (`git commit -m 'Add AmazingFeature'`)
4. 📤 Push to branch (`git push origin feature/AmazingFeature`)
5. 🔄 Open Pull Request

---

## 🙏 Acknowledgments

- 🏆 **ICONIC IT 2024** - Platform kompetisi yang luar biasa
- 🌱 **Environmental Community** - Inspirasi untuk solusi berkelanjutan  
- 🤖 **TensorFlow Team** - AI framework yang powerful
- 💎 **Laravel Community** - Framework yang amazing

---

<div align="center">

<p><strong>🌱 Mari Bersama Pilah Sampah Kita untuk Indonesia Berkelanjutan! 🌍</strong></p>

<p><em>PILASAKI - ICONIC IT 2024 Finalist</em></p>

<hr>

<p><strong>Made with 💚 for a sustainable Indonesia</strong></p>

</div>