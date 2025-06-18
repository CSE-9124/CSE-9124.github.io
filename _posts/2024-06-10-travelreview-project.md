---
title: "🌍 TravelReview Project"
date: 2024-06-10 00:00:00 +0800
categories: [Project]
tags: [Project, Java, SQLite]
image:
  path: /assets/images/posts/travelreview/AppLogo.jpg
  alt: TravelReview Project Thumbnail
---

<div align="center">
    <img src="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white" alt="Java">
    <img src="https://img.shields.io/badge/JavaFX-ED8B00?style=for-the-badge&logo=java&logoColor=white" alt="JavaFX">
    <img src="https://img.shields.io/badge/MySQL-00000F?style=for-the-badge&logo=mysql&logoColor=white" alt="MySQL">

<p><strong>Aplikasi Review Tempat Wisata Indonesia</strong></p>

<p><em>Membantu wisatawan menemukan destinasi terbaik dengan ulasan terpercaya</em></p>

<p><a href="https://github.com/CSE-9124/TravelReview-project">🔗 Repository</a> • <a href="#-screenshots">📱 Live Demo</a></p>

</div>

---

## 👥 Tim RoamRangers

<div align="center">
<table>
    <tr>
        <td align="center">
            <strong>Cholyn Sharon Enos</strong><br>
            <sub>H071231040</sub>
        </td>
        <td align="center">
            <strong>Muhammad Dirga Dian Nugraha</strong><br>
            <sub>H071231039</sub>
        </td>
        <td align="center">
            <strong>Amalia Diah Ramadani</strong><br>
            <sub>H071231063</sub>
        </td>
    </tr>
</table>
</div>

**🎯 Tema:** Travel and Culture  
**👨‍🏫 Pendamping:** Muh. Adnan Putra Amiruddin  
**👨‍⚖️ Tim Juri:** Awang Mulya Nugrawan, Rahmaliyah Kadir

---

## 🚀 Tentang TravelReview

> **TravelReview** adalah aplikasi desktop berbasis JavaFX yang dirancang untuk membantu wisatawan Indonesia menemukan tempat wisata terbaik, memberikan rating, serta menulis ulasan tentang pengalaman mereka.

### 🎯 Masalah yang Diselesaikan

| 🔍 **Problem** | 💡 **Solution** |
|---|---|
| **Informasi Tersebar** | Platform terpusat untuk ulasan wisata |
| **Kredibilitas Ulasan** | Sistem verifikasi dan rating yang transparan |
| **Pengalaman User** | Interface yang user-friendly dan intuitif |

### ✨ Mengapa TravelReview?

- 🏝️ **Fokus Indonesia** - Khusus destinasi wisata Nusantara
- 🔒 **Terpercaya** - Sistem login dan verifikasi user
- 📊 **Data Akurat** - Rating berbasis pengalaman nyata
- 🎨 **Modern UI** - Interface yang menarik dan mudah digunakan

---

## 🛠️ Fitur Utama

### 👤 **Fitur User**
```
🏠 Dashboard dengan rekomendasi wisata
📍 Daftar lengkap tempat wisata (card view)
📖 Detail destinasi dengan deskripsi menarik
⭐ Sistem rating dan ulasan
👤 Manajemen profil & foto profil
```

### 🔧 **Fitur Admin**
```
📊 Dashboard admin dengan statistik
🗂️ Manajemen tempat wisata (CRUD)
📋 Tampilan tabel untuk data management
```

### 🔐 **Fitur Umum**
```
🔑 Sistem login/register yang aman
🧭 Navigasi yang intuitif
🚪 Logout dengan konfirmasi
```

---

## 🏗️ Penerapan Prinsip OOP

| **Prinsip** | **Implementasi** | **Contoh Class** |
|:---:|:---:|:---:|
| **🔒 Encapsulation** | Private attributes + Getter/Setter | `User`, `TempatWisata`, `Comment` |
| **🧬 Inheritance** | Class turunan dari parent class | Controllers extend `DbConfig` |
| **🎭 Polymorphism** | Override methods di subclass | Scene classes extend `AScene` |
| **🎯 Abstraction** | Abstract class dengan template | `AScene` abstract class |

### 💡 Detail Implementasi

**1. Abstraction dengan AScene**
```java
// Template pattern untuk semua scene
abstract class AScene {
    protected abstract void initializeComponents();
    protected abstract void setupEventHandlers();
}
```

**2. Inheritance Chain**
```
Application
    ↳ App (Main Class)

DbConfig
    ↳ UsersController
    ↳ TempatWisataController  
    ↳ CommentsController
```

**3. Encapsulation Example**
```java
public class User {
    private String username;    // Private attributes
    private String email;
    
    public String getUsername() { return username; }  // Controlled access
    public void setUsername(String username) { this.username = username; }
}
```

---

## 📱 Screenshots

### 🔐 Authentication

<div align="center">
    <table>
        <tr>
            <td align="center" width="50%">
                <strong>Login</strong><br>
                <img src="{{ site.baseurl }}/assets/images/posts/travelreview/LoginScene.jpg" alt="Login" style="width: 100%; max-width: 400px; height: auto;">
            </td>
            <td align="center" width="50%">
                <strong>Register</strong><br>
                <img src="{{ site.baseurl }}/assets/images/posts/travelreview/RegisterScene.jpg" alt="Register" style="width: 100%; max-width: 400px; height: auto;">
            </td>
        </tr>
    </table>
</div>

### 🏠 User Interface

<div align="center">
    <table>
        <tr>
            <td align="center" width="50%">
                <strong>Home Dashboard</strong><br>
                <img src="{{ site.baseurl }}/assets/images/posts/travelreview/HomeScene.jpg" alt="Home Dashboard" style="width: 100%; max-width: 400px; height: auto;">
            </td>
            <td align="center" width="50%">
                <strong>Daftar Wisata</strong><br>
                <img src="{{ site.baseurl }}/assets/images/posts/travelreview/DaftarTempatWisata.jpg" alt="Daftar Wisata" style="width: 100%; max-width: 400px; height: auto;">
            </td>
        </tr>
    </table>
</div>

### 📖 Detail & Review

<div align="center">
    <table>
        <tr>
            <td align="center" width="50%">
                <strong>Detail Wisata</strong><br>
                <img src="{{ site.baseurl }}/assets/images/posts/travelreview/DetailTempatWisata.jpg" alt="Detail Wisata" style="width: 100%; max-width: 400px; height: auto;">
            </td>
            <td align="center" width="50%">
                <strong>Rating & Ulasan</strong><br>
                <img src="{{ site.baseurl }}/assets/images/posts/travelreview/RatingUlasan.jpg" alt="Rating & Ulasan" style="width: 100%; max-width: 400px; height: auto;">
            </td>
        </tr>
    </table>
</div>

### 👤 Profile & Admin

<div align="center">
    <table>
        <tr>
            <td align="center" width="50%">
                <strong>User Profile</strong><br>
                <img src="{{ site.baseurl }}/assets/images/posts/travelreview/ProfileScene.jpg" alt="User Profile" style="width: 100%; max-width: 400px; height: auto;">
            </td>
            <td align="center" width="50%">
                <strong>Admin Dashboard</strong><br>
                <img src="{{ site.baseurl }}/assets/images/posts/travelreview/AdminHomeScene.jpg" alt="Admin Dashboard" style="width: 100%; max-width: 400px; height: auto;">
            </td>
        </tr>
    </table>
</div>

### ⚙️ Admin Management

<div align="center">
    <table>
        <tr>
            <td align="center" width="33.33%">
                <strong>Tabel Management</strong><br>
                <img src="{{ site.baseurl }}/assets/images/posts/travelreview/TableTempatWisata.jpg" alt="Table Management" style="width: 100%; max-width: 400px; height: auto;">
            </td>
            <td align="center" width="33.33%">
                <strong>Add Wisata</strong><br>
                <img src="{{ site.baseurl }}/assets/images/posts/travelreview/AddTempatWisata.jpg" alt="Add Wisata" style="width: 100%; max-width: 400px; height: auto;">
            </td>
            <td align="center" width="33.33%">
                <strong>Edit Wisata</strong><br>
                <img src="{{ site.baseurl }}/assets/images/posts/travelreview/EditTempatWisata.jpg" alt="Edit Wisata" style="width: 100%; max-width: 400px; height: auto;">
            </td>
        </tr>
    </table>
</div>

---

## 🧪 Testing Results

<div align="center">

<p><strong>✅ 15/15 Test Cases Passed</strong></p>

</div>

| 🧪 **Test Case** | 📋 **Description** | 🎯 **Result** |
|:---:|---|:---:|
| **1** | Login dengan kredensial salah | ✅ |
| **2** | Login tanpa input | ✅ |
| **3** | Register dengan field kosong | ✅ |
| **4** | Menambah & menampilkan komentar | ✅ |
| **5** | Sistem rating tempat wisata | ✅ |
| **6** | Handle data kosong | ✅ |
| **7** | Logout functionality | ✅ |
| **8** | Upload foto profil | ✅ |
| **9** | Default profile picture | ✅ |
| **10** | Update profil user | ✅ |
| **11** | Validasi email format | ✅ |
| **12** | Admin login access | ✅ |
| **13** | CRUD tempat wisata - Create | ✅ |
| **14** | CRUD tempat wisata - Update | ✅ |
| **15** | CRUD tempat wisata - Delete | ✅ |

---

## 🎯 Tech Stack

| **Category** | **Technology** |
|:---:|:---:|
| **Language** | Java |
| **UI Framework** | JavaFX |
| **Database** | MySQL |
| **IDE** | IntelliJ IDEA / Eclipse |
| **Version Control** | Git & GitHub |

---

## 📅 Development Timeline

| **Date** | **Milestone** |
|:---:|:---:|
| **13 Mei 2024** | 🚀 Project Kickoff |
| **22 Mei 2024** | 📋 Planning & Design |
| **23 Mei 2024** | 🔧 Core Development |
| **27 Mei 2024** | 🧪 Testing Phase |
| **29 Mei 2024** | 🎉 Final Review |

---

## 🚀 Getting Started

```bash
# Clone repository
git clone https://github.com/CSE-9124/TravelReview-project.git

# Buka project di IDE
cd TravelReview-project

# Setup database MySQL
# Import database schema

# Run aplikasi
# Execute main class: App.java
```

---

## 🎉 Kesimpulan

**TravelReview** berhasil mengimplementasikan konsep Object-Oriented Programming dengan sempurna, menghadirkan solusi nyata untuk masalah wisatawan Indonesia dalam mencari informasi destinasi terpercaya. Dengan interface yang user-friendly dan fitur yang lengkap, aplikasi ini siap membantu mempromosikan pariwisata Indonesia.

---

<div align="center">

<p><strong>🏆 Final Project Object-Oriented Programming</strong></p>

<p><em>Universitas Hasanuddin - 2024</em></p>

</div>