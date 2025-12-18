
### 2. Kustomisasi Konten

Ini adalah bagian terpenting. Ganti placeholder dan konten contoh dengan milik Anda.

#### A. Informasi Umum (Ganti di semua file HTML)

-   **Nama TTM & Nama Kamu:** Ganti `[Nama TTM]` dengan nama orang yang Anda tuju, dan `[Nama Kamu]` dengan nama Anda.
-   **Warna Aksen:**
    -   Di dalam tag `<style>` di setiap file, cari baris `--color-accent: #A67C52;`.
    -   Ganti `#A67C52` (coklat emas) dengan `#7A8B7E` (sage green) atau warna lain yang Anda suka.

#### B. Homepage (`index.html`)

-   **Foto Hero:** Ganti `src="https://images.unsplash.com/..."` pada tag `<img>` dengan path foto Anda (misal: `assets/images/hero-portrait.jpg`).
-   **Subheading:** Ubah teks "The person who makes my coffee order sound like poetry" dengan kalimat personal Anda.

#### C. Timeline (`timeline.html`)

-   **Menambah Milestone Baru:**
    1.  Salin seluruh blok `<div class="timeline-item ...> ... </div>`.
    2.  Tempelkan di bawah item terakhir.
    3.  Ubah isi `span` (tanggal), `h3` (judul), `p` (cerita), dan `src` pada tag `<img>` (foto).
    4.  Untuk membuat item muncul di sisi berlawanan, tambahkan kelas `md:mr-auto` pada `div` dengan kelas `bg-white` dan hapus kelas `ml-auto md:ml-0`.

#### D. Peta Kenangan (`places.html`)

-   **Mengatur Pusat Peta:** Di dalam `<script>`, ubah koordinat pada `L.map('map', { center: [LAT, LNG], ... })`.
-   **Menambah Lokasi Baru:**
    1.  Di dalam `<script>`, cari array `const places = [...]`.
    2.  Salin dan tempel objek `{ ... }` di dalam array.
    3.  Ubah nilai `coords`, `title`, `memory`, `date`, dan `imgUrl` untuk setiap lokasi baru.

#### E. Halaman "Little Things" (`things.html`)

-   **Menambah Kartu Baru:**
    1.  Salin seluruh blok `<div class="flip-card ...> ... </div>`.
    2.  Tempelkan di dalam `div` dengan kelas `grid`.
    3.  Ubah teks di `flip-card-front` (hal kecil) dan `flip-card-back` (alasannya).

#### F. Surat Pribadi (`letter.html`)

-   **Password:** Di dalam `<script>`, ubah nilai `const correctOTP = "DDMMYYYY";` dengan tanggal anniversary Anda.
-   **Isi Surat:** Ganti teks placeholder di dalam `<div class="prose ...">` dengan surat pribadi Anda.

### 3. Cara Menjalankan Lokal

Agar semua fitur (terutama peta) berjalan normal, **jangan** cukup dengan double-click file `index.html`.

**Cara Termudah: Gunakan Live Server di VS Code**

1.  Install [Visual Studio Code](https://code.visualstudio.com/).
2.  Buka VS Code, buka tab **Extensions**, cari dan install **Live Server** (oleh Ritwick Dey).
3.  Buka folder proyek Anda di VS Code.
4.  Klik kanan pada file `index.html` dan pilih **"Open with Live Server"**.

Website Anda akan terbuka di browser dengan alamat `http://127.0.0.1:5500` dan semua fitur akan berfungsi dengan sempurna.

## 🌐 Cara Deploy (Publishing)

Cara termudah dan gratis adalah menggunakan **GitHub Pages**.

1.  **Upload ke GitHub:**
    -   Buat repository baru di [GitHub](https://github.com).
    -   Upload semua file website Anda ke repository tersebut.
2.  **Aktifkan GitHub Pages:**
    -   Di repository Anda, buka tab **Settings**.
    -   Di menu sebelah kiri, pilih **Pages**.
    -   Di bagian "Build and deployment", pada "Source", pilih **Deploy from a branch**.
    -   Pada "Branch", pilih `main` (atau `master`) dan folder `/ (root)`.
    -   Klik **Save**.

Website Anda akan tayang dalam beberapa menit di alamat `https://[username-github].github.io/[nama-repository]/`.

## 💌 Kata Penutup

Proyek ini dirancang untuk menjadi kanvas bagi perasaan Anda. Jangan ragu untuk bereksperimen dengan teks dan foto. Keindahan website ini terletak pada detail personal yang Anda masukkan. Selamat berkarya!
