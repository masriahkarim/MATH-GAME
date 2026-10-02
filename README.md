# MATH RUSH 🚀

> **“5 Minit. 1 Misi. Jadi Math Hero!”**  
> *A fun 5-minute maths adventure for young Math Heroes.*

MATH RUSH ialah sebuah permainan arked matematik pantas dan interaktif yang direka khusus untuk kanak-kanak berumur 7 hingga 12 tahun. Pemain memilih wira maskot kegemaran mereka, menjawab soalan matematik mengikut tahap umur, membina kombo berterusan, dan menewaskan musuh utama **Math Dragon** dalam pusingan Final Boss 5 minit!

---

## 🌟 Features (Ciri-Ciri Utama)

- **Misi Pantas 5 Minit**: Sesi permainan berfokus dengan pemasa undur, amaran keterujaan (*“🔥 LAST MINUTE!”* & *“🚀 FINAL PUSH!”*).
- **3 Tahap Umur Khas**:
  - 🟢 **7–8 Tahun**: Operasi Tambah, Tolak, Sifir Asas & Bentuk Geometri.
  - 🔵 **9–10 Tahun**: Operasi Darab, Bahagi, Pecahan Mudah & Wang Ringgit.
  - 🟣 **11–12 Tahun**: Operasi Campuran, Peratus, Nisbah & Ukuran.
- **4 Maskot Berpersonaliti**:
  - 🐼 **Panda Hero** (*Tenang dan bijak*)
  - 🤖 **Robo Bot** (*Pantas dan suka nombor*)
  - 🐱 **Kucing Oyen** (*Lincah dan ceria*)
  - 🦖 **Dino Boy** (*Berani dan kuat*)
- **Ekspresi Wajah Dinamik**: Maskot bertindak balas mengikut emosi (Biasa 🙂, Betul 😄, Super Combo 🤩, Cuba Lagi 😮, Menang 🎉).
- **Pertarungan Epik Final Boss**: Berhadapan dengan **Math Dragon** dengan 3 lapisan perisai untuk memenangi Crystal Ajaib!
- **Sistem Ganjaran Lengkap**:
  - ⭐ **Stars**: Diperoleh dengan menjawab betul, bonus round, dan kombo.
  - 🏆 **XP & Level Up**: Capai tahap baharu (Level 1 hingga 5: *Math Explorer*, *Number Ninja*, *Math Dragon Slayer*).
  - 🔥 **Daily Streak**: Rekod hari bermain berturut-turut yang disimpan secara automatik.
  - 🎖️ **Sistem Lencana (Badges)**: 8 lencana pencapaian untuk dibuka.
  - 🛍️ **Almari Aksesori (Closet)**: Pasang topi roket 🚀, cermin mata bintang ⭐, mahkota raja math 👑, dan sayap emas 🪽.
- **Kesan Audio Sintesis Ceria**: Tiada fail MP3 berat; menggunakan Web Audio API sepenuhnya untuk bunyi *ding* betul, kombo naik, dan lagu kemenangan wira.
- **100% Client-Side & Luar Talian**: Berfungsi sepenuhnya dalam pelayar tanpa memerlukan pelayan backend atau pangkalan data luar.
- **Penyimpanan Setempat (localStorage)**: Semua data tahap, bintang, kombo, lencana, dan tetapan bunyi disimpan rapi di dalam pelayar peranti.

---

## 🛠️ Technology (Teknologi)

- **Frontend**: [React 19](https://react.dev/) + [TypeScript](https://www.typescriptlang.org/)
- **Build Tool**: [Vite 8](https://vitejs.dev/)
- **Styling**: [Tailwind CSS v4](https://tailwindcss.com/)
- **Icons**: [Lucide React](https://lucide.dev/)
- **Celebration Effects**: [Canvas Confetti](https://www.npmjs.com/package/canvas-confetti)
- **Audio**: Web Audio API (Native browser sound synthesis)
- **Deployment Target**: [GitHub Pages](https://pages.github.com/) (Static Web Application)

---

## 💻 Run Locally (Menjalankan Secara Tempatan)

Ikuti langkah mudah ini untuk menjalankan permainan di komputer anda:

1. **Clone repository ini:**
   ```bash
   git clone https://github.com/USERNAME/math-rush.git
   cd math-rush
   ```

2. **Pasang pakej dependensi:**
   ```bash
   npm install
   ```

3. **Mulakan server pembangunan (development server):**
   ```bash
   npm run dev
   ```

4. Buka pelayar web dan layari alamat:
   ```
   http://localhost:3000
   ```

5. **Uji binaan pengeluaran (production build):**
   ```bash
   npm run build
   npm run preview
   ```

---

## 🚀 Deploy to GitHub Pages (Cara Publish ke GitHub Pages)

Project ini telah siap dikonfigurasi dengan **GitHub Actions** automatik. Anda hanya perlu tolak (*push*) kod ke GitHub:

### Langkah 1: Tolak Kod ke GitHub Repository
```bash
git init
git add .
git commit -m "feat: Initial commit for MATH RUSH game"
git branch -M main
git remote add origin https://github.com/USERNAME/NAMA-REPO-ANDA.git
git push -u origin main
```

### Langkah 2: Aktifkan GitHub Pages dalam Repository Settings
1. Buka repository anda di laman web **GitHub**.
2. Klik tab **Settings** (di bahagian atas repository).
3. Di menu sebelah kiri, klik **Pages** (di bawah seksyen *Code and automation*).
4. Di bawah tajuk **Build and deployment** > **Source**:
   - Pilih **GitHub Actions** (bukan *Deploy from a branch*).
5. GitHub Actions workflow (`.github/workflows/deploy.yml`) akan bermula secara automatik!
6. Pergi ke tab **Actions** untuk melihat proses *Build and Deploy*.
7. Selepas 1-2 minit, URL permainan anda akan dipaparkan di bahagian atas tab **Settings > Pages**:
   ```
   https://USERNAME.github.io/NAMA-REPO-ANDA/
   ```

---

## 📁 Project Structure (Struktur Folder)

```text
/
├── .github/
│   └── workflows/
│       └── deploy.yml          # GitHub Actions workflow untuk deployment automatik
├── public/
│   └── favicon.svg             # Web app icon roket rasmi
├── src/
│   ├── assets/
│   │   └── images/             # Imej maskot (Panda, Robot, Kucing, Dino, Dragon Boss)
│   ├── components/
│   │   ├── BadgesModal.tsx     # Modal paparan lencana wira
│   │   ├── BossBattleScreen.tsx# Skrin pertempuran Dragon Boss 
│   │   ├── CartoonBackground.tsx# Latar belakang kartun awan, bukit & istana
│   │   ├── CharacterAvatar.tsx # Komponen avatar maskot dengan ekspresi emosi
│   │   ├── GameScreen.tsx      # Skrin utama gameplay matematik 3-zon
│   │   ├── Header.tsx          # Bar status (Bintang, Streak, Mute Sound FX)
│   │   ├── HomeScreen.tsx      # Skrin utama dengan butang ▶️ MULA MAIN besar
│   │   ├── RewardScreen.tsx    # Skrin kemenangan misi & sambutan Level Up
│   │   └── ShopClosetModal.tsx # Almari kosmetik & aksesori
│   ├── types/
│   │   └── game.ts             # Definisi Typescript (Question, Profile, Mascot, etc.)
│   ├── utils/
│   │   ├── characters.ts       # Maklumat maskot, aksesori & lencana
│   │   ├── confetti.ts         # Animasi letupan konfeti & bintang
│   │   ├── questionGenerator.ts# Penjana soalan matematik adaptif mengikut umur
│   │   ├── sound.ts            # Web Audio API audio synthesizer ceria
│   │   └── storage.ts          # Pengurusan localStorage profil & data pemain
│   ├── App.tsx                 # Komponen akar navigasi skrin
│   ├── index.css               # Import Tailwind CSS & fon tersuai
│   └── main.tsx                # Titik permulaan React DOM
├── index.html                  # Fail HTML utama dengan meta tags & favicon
├── package.json                # Skrip binaan & senarai dependensi
├── tsconfig.json               # Konfigurasi TypeScript
├── vite.config.ts              # Konfigurasi Vite dengan base: './' untuk GitHub Pages
├── .gitignore                  # Senarai fail dikecualikan dari Git
└── README.md                   # Dokumentasi lengkap projek
```

---

## 📄 License

Projek ini dibangunkan untuk tujuan pendidikan dan belum mempunyai lesen sumber terbuka rasmi (*All rights reserved*).
