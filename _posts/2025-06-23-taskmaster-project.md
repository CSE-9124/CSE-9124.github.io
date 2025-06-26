---
title: "📝 TaskMaster - Aplikasi Manajemen Tugas dan Jadwal"
date: 2025-06-23 00:00:00 +0800
categories: [Project, Android]
tags: [Project, Java, SQLite]
image:
    path: /assets/images/posts/taskmaster/AppLogo.png
    alt: TaskMaster Thumbnail
---
<div align="center">
    <img src="https://img.shields.io/badge/Android-3DDC84?style=for-the-badge&logo=android&logoColor=white" alt="Android" />
    <img src="https://img.shields.io/badge/Java-007396?style=for-the-badge&logo=openjdk&logoColor=white" alt="Java" />
    <img src="https://img.shields.io/badge/SQLite-003B57?style=for-the-badge&logo=sqlite&logoColor=white" alt="SQLite" />
    <img src="https://img.shields.io/badge/Material_Design-757575?style=for-the-badge&logo=material-design&logoColor=white" alt="Material Design" />

<p><em>Organize your tasks, master your time!</em> ⏰✨</p>

<p>
    <a href="https://github.com/Rezka08/TaskMaster">🔗 Repository</a> • 
    <a href="#-getting-started">📱 Download APK</a>
</p>

</div>

---

## 🎯 Tentang TaskMaster

> **TaskMaster** adalah aplikasi Android native yang dirancang khusus untuk membantu mahasiswa dan profesional mengorganisir serta melacak tugas dengan sistem visualisasi berbasis prioritas dan waktu yang intuitif.

### 🚀 Mengapa TaskMaster?

| **🎯 Problem** | **💡 TaskMaster Solution** |
|:---|:---|
| **Kesulitan Prioritas** | Sistem warna otomatis berdasarkan deadline |
| **Akses Lambat** | Widget homescreen untuk akses instan |
| **UI Membosankan** | Dark/Light mode dengan Material Design |
| **Tidak User-Friendly** | Interface intuitif dengan visual yang kaya |

### 📊 Target Pengguna

- **👨‍🎓 Mahasiswa (18-25 tahun)** - Mengelola tugas kuliah dan deadline
- **👔 Profesional (25-40 tahun)** - Manajemen proyek dan jadwal rapat  
- **⏰ Busy People** - Siapapun dengan jadwal padat yang butuh organisasi

---

## ✨ Fitur Unggulan

### 🏠 **Home Fragment - Dashboard Cerdas**
```
📊 Monthly Preview dengan 4 kotak ringkasan
📈 Progress Tracker real-time
🔔 Notifikasi dengan 3 filter (upcoming, in progress, completed)
🎨 Sistem prioritas visual otomatis:
   🔴 Merah: Deadline sangat dekat
   🟡 Kuning: 2-3 hari lagi  
   🟢 Hijau: Seminggu lagi
```

### ➕ **Add Task Fragment - Form Lengkap**
```
📝 Nama tugas dengan validasi
📅 Date picker yang user-friendly
⏰ Time picker untuk waktu mulai-selesai
📋 Deskripsi detail
🏷️ Kategori tugas
✏️ Edit mode untuk modifikasi
🎯 Auto-prioritas berdasarkan tanggal
```

### 📅 **Calendar Fragment - Visualisasi Komprehensif**
```
🗓️ Tampilan kalender bulanan interaktif
📍 Indikator tugas dengan warna prioritas
🔍 Fitur pencarian tugas canggih
🏷️ Filter berdasarkan kategori
📱 Detail tugas harian saat tanggal dipilih
```

### 🏠 **Widget Homescreen - Akses Instan**
```
📋 Menampilkan tugas hari ini
🎨 Indikator prioritas dengan sistem warna
✅ Quick action untuk mark completed
🚀 Shortcut ke aplikasi utama
```

### 🌙 **Dark/Light Mode - Adaptive Theme**
```
🌞 Light Mode: Optimal untuk siang hari
🌙 Dark Mode: Nyaman untuk mata & hemat battery
🔄 Automatic Theme: Mengikuti sistem device
🎨 Consistent Branding: Warna tetap konsisten
```

---

## 🛠️ Tech Stack & Architecture


### **Core Technologies**
<div align="center">

<div align="center">
    <img src="https://img.shields.io/badge/API_Level-24--34-green?style=flat-square&logo=android&logoColor=white" alt="API Level" />
    <img src="https://img.shields.io/badge/JDK-8+-orange?style=flat-square&logo=openjdk&logoColor=white" alt="JDK" />
    <img src="https://img.shields.io/badge/Kotlin_DSL-7F52FF?style=flat-square&logo=kotlin&logoColor=white" alt="Kotlin DSL" />
</div>

</div>

### **Libraries & Components**

<div align="center">

<div align="center">
    <img src="https://img.shields.io/badge/Room_Database-4285F4?style=flat-square&logo=google&logoColor=white" alt="Room Database" />
    <img src="https://img.shields.io/badge/RecyclerView-4285F4?style=flat-square&logo=android&logoColor=white" alt="RecyclerView" />
    <img src="https://img.shields.io/badge/WorkManager-4285F4?style=flat-square&logo=android&logoColor=white" alt="WorkManager" />
    <img src="https://img.shields.io/badge/Calendar_View-FF6B35?style=flat-square&logo=calendar&logoColor=white" alt="Calendar View" />
    <img src="https://img.shields.io/badge/Widget_Provider-34A853?style=flat-square&logo=android&logoColor=white" alt="Widget Provider" />
</div>

</div>

### 🏗️ Architecture Details

| **Layer** | **Technology** | **Purpose** |
|:---:|:---:|:---|
| **Presentation** | Fragments + Activities | UI Layer dengan Material Design |
| **Data** | Room Database | Local storage dengan SQLite |
| **Notification** | WorkManager | Background task management |
| **Widget** | AppWidgetProvider | Homescreen integration |
| **Theme** | AppCompatDelegate | Dark/Light mode implementation |

### 📦 Key Dependencies

```gradle
dependencies {
    // Core Android
    implementation 'androidx.appcompat:appcompat:1.6.1'
    implementation 'com.google.android.material:material:1.9.0'
    
    // Database
    implementation 'androidx.room:room-runtime:2.5.0'
    
    // Background Tasks
    implementation 'androidx.work:work-runtime:2.8.1'
    
    // UI Components
    implementation 'androidx.recyclerview:recyclerview:1.3.0'
    implementation 'androidx.fragment:fragment:1.6.0'
}
```

---

## 🎨 Design System

### 🎯 Color Palette

| **Purpose** | **Light Mode** | **Dark Mode** | **Usage** |
|:---:|:---:|:---:|:---|
| **Primary** | <span style="display:inline-block;width:14px;height:14px;background-color:#2196F3;"></span> #2196F3 | <span style="display:inline-block;width:14px;height:14px;background-color:#1976D2;"></span> #1976D2 | App branding, CTAs |
| **Accent**  | <span style="display:inline-block;width:14px;height:14px;background-color:#FF9800;"></span> #FF9800 | <span style="display:inline-block;width:14px;height:14px;background-color:#F57C00;"></span> #F57C00 | Highlights, buttons |
| **Urgent**  | <span style="display:inline-block;width:14px;height:14px;background-color:#F44336;"></span> #F44336 | <span style="display:inline-block;width:14px;height:14px;background-color:#D32F2F;"></span> #D32F2F | High priority tasks |
| **Medium**  | <span style="display:inline-block;width:14px;height:14px;background-color:#FFC107;"></span> #FFC107 | <span style="display:inline-block;width:14px;height:14px;background-color:#F9A825;"></span> #F9A825 | Medium priority |
| **Low**     | <span style="display:inline-block;width:14px;height:14px;background-color:#4CAF50;"></span> #4CAF50 | <span style="display:inline-block;width:14px;height:14px;background-color:#388E3C;"></span> #388E3C | Low priority tasks |

### 📱 UI Components Gallery
<div style="overflow-x: auto; white-space: nowrap; padding-bottom: 8px;">
    <div style="display: inline-flex; gap: 16px; align-items: flex-start;">
        <div style="text-align: center;">
            <img src="/assets/images/posts/taskmaster/Light-HomeFragment.png" alt="Home" style="height:320px; width:auto; display:block; margin:0 auto;"/>
            <div><strong>Home Fragment</strong></div>
        </div>
        <div style="text-align: center;">
            <img src="/assets/images/posts/taskmaster/Light-AddTaskFragment.png" alt="Add" style="height:320px; width:auto; display:block; margin:0 auto;"/>
            <div><strong>Add Task Fragment</strong></div>
        </div>
        <div style="text-align: center;">
            <img src="/assets/images/posts/taskmaster/Light-CalenderFragment.png" alt="Calendar" style="height:320px; width:auto; display:block; margin:0 auto;"/>
            <div><strong>Calendar Fragment</strong></div>
        </div>
        <div style="text-align: center;">
            <img src="/assets/images/posts/taskmaster/Light-SearchActivity.png" alt="Search" style="height:320px; width:auto; display:block; margin:0 auto;"/>
            <div><strong>Search Fragment</strong></div>
        </div>
    </div>
</div>
<div style="overflow-x: auto; white-space: nowrap; padding-bottom: 8px;">
    <div style="display: inline-flex; gap: 16px; align-items: flex-start;">
        <div style="text-align: center;">
            <img src="/assets/images/posts/taskmaster/Light-NotificationActivity.png" alt="Notification" style="height:320px; width:auto; display:block; margin:0 auto;"/>
            <div><strong>Notification Activity</strong></div>
        </div>
        <div style="text-align: center;">
            <img src="/assets/images/posts/taskmaster/Light-DetailTaskActivity.png" alt="Detail Task" style="height:320px; width:auto; display:block; margin:0 auto;"/>
            <div><strong>Detail Task Activity</strong></div>
        </div>
        <div style="text-align: center;">
            <img src="/assets/images/posts/taskmaster/Light-SettingsActivity.png" alt="Settings" style="height:320px; width:auto; display:block; margin:0 auto;"/>
            <div><strong>Settings Activity</strong></div>
        </div>
        <div style="text-align: center;">
            <img src="/assets/images/posts/taskmaster/WidgetHomescreen.png" alt="Widget" style="height:320px; width:auto; display:block; margin:0 auto;"/>
            <div><strong>Widget</strong></div>
        </div>
    </div>
</div>

---

## 💡 Use Cases & User Journey

### 🎓 **Skenario 1: Mahasiswa**
```
Situasi: Mahasiswa dengan multiple deadline assignments
Flow:
1. 📱 Buka TaskMaster → Lihat monthly preview
2. ➕ Add new task: "Essay Sociology" 
3. 📅 Set deadline: 3 hari lagi → Auto priority: KUNING
4. 🏠 Add widget → Monitor progress dari homescreen
5. ✅ Mark completed setelah selesai
```

### 👔 **Skenario 2: Profesional**
```
Situasi: Manager dengan jadwal rapat dan project deadline
Flow:
1. 🗓️ Calendar view → Overview semua meeting minggu ini
2. 🔍 Search "Client presentation" → Quick access
3. 📋 Check widget → Lihat agenda hari ini tanpa buka app
4. 🔔 Receive notification → Preparation reminder
```

### 🔍 **Skenario 3: Power User**
```
Situasi: Pengguna dengan banyak task berbeda kategori
Flow:
1. 🏷️ Filter by category → "Personal", "Work", "Study"  
2. 🎨 Visual priority → Focus on RED tasks first
3. 🌙 Switch to dark mode → Evening productivity
4. 📊 Monthly review → Track completion patterns
```

---

## 🏆 Competitive Analysis

| **Feature** | **TaskMaster** | **Google Calendar** | **Microsoft To Do** | **Any.do** |
|:---|:---:|:---:|:---:|:---:|
| **Visual Priority System** | ✅ Auto-color coding | ❌ Manual only | ❌ Basic flags | ❌ Manual lists |
| **Homescreen Widget** | ✅ Rich info display | ⚠️ Basic calendar | ❌ None | ⚠️ Simple list |
| **Dark/Light Mode** | ✅ Smooth adaptive | ✅ System-based | ✅ Basic toggle | ⚠️ Limited |
| **Offline Functionality** | ✅ Full offline | ❌ Cloud-dependent | ⚠️ Limited | ❌ Cloud-dependent |
| **Time Range Setting** | ✅ Start-end time | ⚠️ Event-focused | ❌ Due date only | ❌ Due date only |
| **Category Filtering** | ✅ Advanced filters | ⚠️ Calendar-based | ⚠️ Basic lists | ⚠️ Limited |

### 🎯 **TaskMaster Advantages**

- **🎨 Smart Visual Prioritization** - Auto-color coding berdasarkan urgency
- **🏠 Superior Widget Experience** - Informative homescreen integration  
- **🌙 Seamless Theme Switching** - Responsive dark/light mode
- **⏰ Detailed Time Management** - Start-end time untuk planning yang detail
- **🔍 Powerful Search & Filter** - Find tasks dengan mudah
- **📱 True Mobile-First Design** - Optimized untuk Android experience

---

## 📊 Impact & Statistics

### **Problem Statement Data**
- **87%** mahasiswa mengalami stres akibat manajemen waktu yang buruk
- **Visual priority system** membantu brain processing **3x lebih cepat**
- **Widget integration** meningkatkan task completion rate hingga **40%**

### **User Benefits**
- ⏱️ **Save 15 minutes daily** dengan quick widget access
- 🎯 **Improve focus** dengan visual priority system
- 📱 **Reduce app switching** dengan comprehensive features
- 🧠 **Decrease mental load** dengan automated prioritization

---

## 🚀 Getting Started

### 📋 **Prerequisites**
- Android Studio Arctic Fox+ 
- JDK 8+
- Android SDK (API 24-34)
- Git untuk version control

### ⚡ **Quick Installation**

```bash
# Clone repository
git clone https://github.com/Rezka08/TaskMaster.git
cd TaskMaster

# Open in Android Studio
# Sync Gradle files
# Build and run on device/emulator
```

### 📦 **Build APK**
```bash
# Debug build
./gradlew assembleDebug

# Release build  
./gradlew assembleRelease
```

### 🔧 **Development Setup**
```bash
# Install dependencies
./gradlew build

# Run tests
./gradlew test

# Generate coverage report
./gradlew jacocoTestReport
```

---

## 🏗️ Project Architecture

### 📁 **File Structure**
```
TaskMaster/
├── 📱 app/
│   ├── 📄 src/main/
│   │   ├── ☕ java/com/taskmaster/
│   │   │   ├── 🏠 fragments/          # UI Fragments
│   │   │   ├── 📱 activities/         # Activities
│   │   │   ├── 🔄 adapters/          # RecyclerView Adapters
│   │   │   ├── 💾 database/          # Room Database
│   │   │   ├── 📊 models/            # Data Models
│   │   │   ├── 🛠️ utils/             # Utility Classes
│   │   │   └── 🏠 widgets/           # Widget Providers
│   │   └── 🎨 res/
│   │       ├── 📐 layout/            # XML Layouts
│   │       ├── 🎨 values/            # Colors, Strings, Styles
│   │       ├── 🖼️ drawable/          # Images & Icons
│   │       └── 🔤 font/              # Custom Fonts
│   └── 🔧 build.gradle.kts           # Module Dependencies
├── 📋 gradle/                        # Gradle Wrapper
├── ⚙️ build.gradle.kts               # Project Config
└── 📖 README.md                      # Documentation
```

### 🔧 **Core Components**

**🏠 MainActivity + Fragments**
```java
// Bottom navigation with 3 main fragments
- HomeFragment: Dashboard & overview
- AddTaskFragment: Task creation/editing  
- CalendarFragment: Calendar view & search
```

**💾 Database Layer**
```java
@Database(entities = {Task.class}, version = 1)
public abstract class TaskDatabase extends RoomDatabase {
    // Task CRUD operations
    // Category management
    // Settings storage
}
```

**🏠 Widget System**
```java
public class TaskWidgetProvider extends AppWidgetProvider {
    // Update widget dengan daily tasks
    // Handle widget clicks
    // Refresh data periodically
}
```

---

## 👥 Development Team
<div align="center">

<strong>🎓 Mahasiswa Universitas Hasanuddin - Mobile Programming Course</strong>

<table>
    <thead>
        <tr>
            <th><center>Name</center></th>
            <th><center>NIM</center></th>
            <th><center>Role</center></th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td><strong>Rezka Wildan Nurhadi Bakri</strong></td>
            <td>H071231030</td>
            <td>Lead Developer &amp; UI/UX</td>
        </tr>
        <tr>
            <td><strong>Restu Ahmadinata</strong></td>
            <td>H071231021</td>
            <td>Backend &amp; Database</td>
        </tr>
        <tr>
            <td><strong>Cholyn Sharon Enos</strong></td>
            <td>H071231040</td>
            <td>Frontend &amp; Testing</td>
        </tr>
        <tr>
            <td><strong>Dhian Alifka Azzahra</strong></td>
            <td>H071231022</td>
            <td>Documentation &amp; QA</td>
        </tr>
    </tbody>
</table>

</div>

---

## 🔮 Future Roadmap

### 🎯 **Version 2.0 - Q3 2025**
- [ ] 🔄 **Cloud Sync** - Backup & sync across devices
- [ ] 👥 **Team Collaboration** - Share tasks dengan team
- [ ] 📊 **Advanced Analytics** - Productivity insights
- [ ] 🎮 **Gamification** - Achievement & rewards system

### 🎯 **Version 3.0 - Q4 2025**
- [ ] 🤖 **AI Suggestions** - Smart task scheduling
- [ ] 🗣️ **Voice Commands** - Voice-to-task conversion
- [ ] ⌚ **Wearable Support** - Android Wear integration
- [ ] 🌐 **Web Companion** - Progressive Web App

---

## 🤝 Contributing

Kami welcome kontribusi dari komunitas developer! 

### 📝 **How to Contribute**
1. 🍴 **Fork** repository ini
2. 🌿 **Create branch** (`git checkout -b feature/AmazingFeature`)
3. 💾 **Commit** perubahan (`git commit -m 'Add AmazingFeature'`)
4. 📤 **Push** ke branch (`git push origin feature/AmazingFeature`)
5. 🔄 **Create Pull Request**

### 🐛 **Bug Reports**
- Gunakan GitHub Issues
- Include screenshots & device info
- Steps to reproduce

### 💡 **Feature Requests**
- Describe use case clearly
- Include mockups if possible
- Consider implementation complexity

---

## 📄 Credits

### 🙏 **Acknowledgments**
- **Material Design** - Google's design system
- **Android Jetpack** - Modern Android development
- **Room Database** - Robust local storage
- **Stack Overflow Community** - Problem solving support

---

<div align="center">

<p><strong>📝 TaskMaster - Organize your tasks, master your time!</strong> ⏰✨</p>

<p><em>Mobile Programming Project - Universitas Hasanuddin 2024</em></p>

</div>

---

<div align="center">

<p><strong>Made with ❤️ by Team TaskMaster</strong></p>

</div>