<div align="center">
  <img src="../logo/logo_olah.png" alt="OLAH Logo" width="400" height="150">

  <h3><b>Punya Sisa Bahan Makanan? di OLAH Aja!</b></h3>
</div>

---

### 🧩 What's this?

**OLAH** adalah project capstone dari program Coding Camp 2026. Project ini dibangun oleh tim **`CC26-PSU127`** dengan tema *Sustainable Living & Responsible Consumption*.

---

<div align="center">
  <h3>👥 Team Members 👥</h3>
  <table align="center">
    <tr>
      <th>Learning Path</th>
      <th>Cohort ID</th>
      <th>Name</th>
    </tr>
    <tr>
      <td>AI Engineer</td>
      <td>CACC193D6Y0545</td>
      <td>Maghfur Hasani</td>
    </tr>
    <tr>
      <td>AI Engineer</td>
      <td>CACC319D6X0506</td>
      <td>Angelin Viona Lumban Tobing</td>
    </tr>
    <tr>
      <td>Data Scientist</td>
      <td>CDCC200D6X2238</td>
      <td>Yunita Asri Prameswari</td>
    </tr>
    <tr>
      <td>Data Scientist</td>
      <td>CDCC289D6X0619</td>
      <td>Titania Rahmawati</td>
    </tr>
    <tr>
      <td>Full Stack Developer</td>
      <td>CFCC308D6X1326</td>
      <td>Marita Habibah</td>
    </tr>
    <tr>
      <td>Full Stack Developer</td>
      <td>CFCC308D6X1325</td>
      <td>Putri Anisa</td>
    </tr>
  </table>
</div>

---

### 📎 Project Description

**OLAH** adalah platform inovatif yang dirancang untuk membantu masyarakat Indonesia mengelola stok bahan makanan secara cerdas guna mengurangi limbah pangan. Melalui sistem inventaris pintar dan rekomendasi resep berbasis AI, kami hadir untuk mengubah sisa bahan di dapur Anda menjadi hidangan lezat.

---

### 🔍 Apa yang Bisa OLAH Lakukan?

- 🍽️ Rekomendasi resep adaptif berbasis bahan yang kamu miliki
- ⏰ Pengingat masa simpan bahan agar tidak terbuang sia-sia
- 🛒 Daftar belanja otomatis untuk pengelolaan stok lebih efisien

---

### 🚀 Instalasi & Menjalankan Aplikasi

Pastikan kamu sudah menginstal **Node.js** dan **npm** sebelum memulai.

#### 🖥️ Frontend

```bash
# 1. Clone repository
git clone https://github.com/habibahh9/olah-frontend.git
cd olah-frontend

# 2. Install dependencies
npm install

# 3. Setup environment variables
cp .env.example .env
# Edit .env sesuai kebutuhan

# 4. Jalankan development server
npm run dev
```

> Buka browser di `http://localhost:5173`

**Build untuk Production:**
```bash
npm run build
```

---

#### ⚙️ Backend

```bash
# 1. Install dependencies
npm install

# 2. Setup environment variables
cp .env.example .env
```

Isi file `.env` dengan konfigurasi berikut:

```env
MONGODB_URI=mongodb+srv://user:pass@cluster.mongodb.net/olah_db
JWT_SECRET=kunci_panjang_rahasia_disini
CLIENT_URL=http://localhost:5173
PORT=5000

# URL FastAPI dari Tim AI
AI_MODEL_URL=http://localhost:8000
AI_TIMEOUT_MS=8000
```

```bash
# 3. Seed resep ke MongoDB
# Letakkan recipe_metadata.json di root folder, lalu jalankan:
npm run seed

# Reset database lalu seed ulang:
RESET=true npm run seed

# Atau gunakan path custom:
RECIPE_FILE=../ai/saved_model/recipe_metadata.json npm run seed

# 4. Jalankan server
npm run dev    # development (dengan nodemon)
npm start      # production
```

---

### 🥘 Akses Website 🍴

- 🌐 **[OLAH — olah-api.vercel.app](https://olah-api.vercel.app)**

---

### 📽️ Final Presentation 🎞️

- 🎬 [Video Presentasi](https://youtu.be/KReQAnJI_ds?si=8nYjt0APFBHVFz0Ro)
- 📖 [Video Tutorial](https://youtu.be/ewCG9WR-CZs?si=6bGborqhkYTr1iqD)
