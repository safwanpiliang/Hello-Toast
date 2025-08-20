# HelloToast - Aplikasi Android Kotlin

## Deskripsi
HelloToast adalah aplikasi Android sederhana yang dibuat menggunakan Kotlin sebagai tugas praktikum mata kuliah Pemrograman Perangkat Bergerak. Aplikasi ini mendemonstrasikan konsep dasar pengembangan Android seperti View Binding, Event Handling, dan Toast Messages.

## Fitur Utama
- **Counter**: Tombol untuk menambah angka yang ditampilkan
- **Toast Message**: Tombol untuk menampilkan pesan toast dengan nilai counter saat ini
- **UI Responsif**: Antarmuka yang sederhana dan mudah digunakan

## Teknologi yang Digunakan
- **Bahasa**: Kotlin
- **Platform**: Android
- **Min SDK**: 24 (Android 7.0)
- **Target SDK**: 36
- **Build System**: Gradle dengan Kotlin DSL
- **UI**: View Binding dengan LinearLayout

## Struktur Project
\`\`\`
app/
├── src/main/
│   ├── java/com/example/hellotoast/
│   │   └── MainActivity.kt          # Activity utama
│   ├── res/
│   │   ├── layout/
│   │   │   └── activity_main.xml    # Layout utama
│   │   ├── values/
│   │   │   ├── strings.xml          # String resources
│   │   │   └── colors.xml           # Color resources
│   │   └── mipmap-*/                # App icons
│   └── AndroidManifest.xml          # Manifest aplikasi
├── build.gradle.kts                 # Build configuration
└── proguard-rules.pro              # ProGuard rules
\`\`\`

## Cara Menjalankan
1. **Prasyarat**:
   - Android Studio (versi terbaru)
   - Android SDK dengan API level 24 atau lebih tinggi
   - Emulator Android atau perangkat fisik

2. **Langkah-langkah**:
   \`\`\`bash
   # Clone atau download project
   git clone <repository-url>
   
   # Buka project di Android Studio
   # File -> Open -> Pilih folder HelloToast
   
   # Sync project dengan Gradle files
   # Build -> Clean Project
   # Build -> Rebuild Project
   
   # Jalankan aplikasi
   # Run -> Run 'app' atau tekan Shift+F10
   \`\`\`

## Cara Menggunakan Aplikasi
1. **Buka aplikasi** - Aplikasi akan menampilkan angka 0 di bagian atas
2. **Tekan tombol "COUNT"** - Angka akan bertambah satu setiap kali ditekan
3. **Tekan tombol "TOAST"** - Akan muncul pesan toast yang menampilkan nilai counter saat ini

## Komponen Utama

### MainActivity.kt
- Menggunakan View Binding untuk mengakses komponen UI
- Mengelola state counter dengan variabel `number`
- Mengimplementasikan OnClickListener untuk kedua tombol

### activity_main.xml
- Layout menggunakan LinearLayout dengan orientasi vertikal
- TextView untuk menampilkan angka dengan background kuning
- Dua Button dalam LinearLayout horizontal dengan weight yang sama

## Konsep Android yang Dipelajari
- **View Binding**: Cara modern untuk mengakses view tanpa findViewById
- **Event Handling**: Menangani klik tombol dengan OnClickListener
- **Toast Messages**: Menampilkan pesan singkat kepada pengguna
- **Layout Management**: Penggunaan LinearLayout dan weight
- **Resource Management**: Penggunaan string dan color resources

## Dependencies
```kotlin
implementation(libs.androidx.core.ktx)
implementation(libs.androidx.appcompat)
implementation(libs.material)
implementation(libs.androidx.activity)
implementation(libs.androidx.constraintlayout)
