<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Biodata Claudia</title>
  <link rel="stylesheet" href="style.css">
</head>

  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
      background: linear-gradient(135deg, #e0c3fc, #8ec5fc);
      color: #333;
    }

    header {
      background: linear-gradient(to right, hwb(332 16% 19%), #ec4b91);
      padding: 20px;
      text-align: center;
      color: pink;
      position: sticky;
      top: 0;
      z-index: 1000;
    }

    header h1 {
      margin: 0;
      font-size: 28px;
      letter-spacing: 2px;
    }

    nav { margin-top: 10px; }
    nav a {
      margin: 20px;
      color: white;
      text-decoration: none;
      font-weight: bold;
      transition: 0.3s;
    }
    nav a:hover { color: #ffde59; }

    section {
      padding: 60px 20px;
      max-width: 900px;
      margin: auto;
      background: rgba(215, 109, 139, 0.9);
      margin-top: 40px;
      border-radius: 15px;
      box-shadow: 0 6px 15px rgba(0, 0, 0, 0.1);
      animation: fadeInUp 1s ease;
    }
    section h2 {
      text-align: center;
      margin-bottom: 20px;
      color: hwb(350 77% 7%);
      font-size: 26px;
    }
    p { text-align: justify; line-height: 1.8; font-size: 16px; }

    @keyframes fadeInUp {
      from { opacity: 0; transform: translateY(30px); }
      to { opacity: 1; transform: translateY(0); }
    }

    /* Slideshow */
    .slideshow-container {
      position: relative;
      max-width: 200px;
      margin: 0 auto 20px auto;
      box-shadow: 0 6px 12px rgba(0, 0, 0, 0.3);
      border-radius: 20px;
      overflow: hidden;
    }
    .slide { display: none; }
    .slide img {
      width: 100%;
      height: 280px;
      object-fit: cover;
      border-radius: 20px;
    }

    /* Riwayat pendidikan */
    .edu-card {
      display: flex;
      align-items: center;
      gap: 20px;
      margin: 20px 0;
      background: #ecc6c6;
      border-radius: 15px;
      padding: 10px;
      box-shadow: 0 3px 8px rgba(0, 0, 0, 0.1);
    }
    .edu-card img {
      width: 150px;
      height: 100px;
      object-fit: cover;
      border-radius: 10px;
    }

    /* Organisasi */
    .org-card {
      background: white;
      padding: 20px;
      margin: 20px auto;
      max-width: 600px;
      border-radius: 15px;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
      text-align: center;
    }
    .org-card img {
      width: 180px;
      height: auto;
      border-radius: 10px;
      margin-top: 10px;
      display: block;
      margin-left: auto;
      margin-right: auto;
    }

    /* Tab prestasi */
    .tabs {
      margin-top: 20px;
      text-align: center;
    }
    .tab-buttons button {
      padding: 10px 20px;
      margin: 5px;
      border: none;
      cursor: pointer;
      border-radius: 8px;
      background: #6a11cb;
      color: white;
      font-weight: bold;
      transition: 0.3s;
    }
    .tab-buttons button:hover {
      background: #2575fc;
    }
    .tab-content { display: none; }
    .tab-content.active { display: block; }

    /* Album foto */
    .gallery {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 15px;
    }
    .gallery img {
      width: 180px;
      height: auto;
      border-radius: 10px;
      box-shadow: 0 4px 6px rgba(0, 0, 0, 0.3);
      transition: transform 0.3s;
    }
    .gallery img:hover {
      transform: scale(1.05);
    }

    /* Funfact */
    .funfact-list {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 15px;
    }
    .funfact-card {
      background: #fff;
      padding: 15px;
      border-radius: 12px;
      box-shadow: 0 4px 6px rgba(0, 0, 0, 0.2);
      width: 200px;
      text-align: center;
    }

    /* Kontak */
    #kontak {
      text-align: center;
      padding: 40px 20px;
      background: #f6bdbd;
      border-radius: 15px;
      margin-top: 40px;
    }
    .kontak-container {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 30px;
      max-width: 600px;
      margin: auto;
    }
    .kontak-box {
      display: flex;
      align-items: center;
      gap: 10px;
      background: white;
      padding: 12px 20px;
      border-radius: 12px;
      box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
      font-size: 18px;
      width: calc(50% - 15px);
      box-sizing: border-box;
      justify-content: center;
      margin-bottom: 15px;
    }
  </style>
</head>
<body>

  <audio id="musik" loop>
    <source src="musik.mp3" type="audio/mpeg">
  </audio>
  <button id="musik-btn" style="position: fixed; bottom: 20px; right: 20px; padding: 10px;">🎶</button>

  <header>
    <h1>✨ Biodata Claudia ✨</h1>
    <nav>
      <a href="#hello">Hello</a>
      <a href="#data-diri">Data Diri</a>
      <a href="#pendidikan">Pendidikan</a>
      <a href="#organisasi">Organisasi</a>
      <a href="#prestasi">Prestasi</a>
      <a href="#funfact">Fun Fact</a>
      <a href="#cita-cita">Cita-Cita</a>
      <a href="#harapan">Harapan</a>
      <a href="#kontak">Kontak</a>
    </nav>
  </header>

  <section id="hello">
    <h2>Hello, Saya Claudia 👋</h2>
    <div class="slideshow-container">
      <div class="slide fade"><img src="foto1.png" alt="claudiaa.png"></div>
      <div class="slide fade"><img src="foto3.png" alt="foto3.png"></div>
      <div class="slide fade"><img src="foto4.png" alt="foto4.png"></div>
      <div class="slide fade"><img src="foto5.png" alt="foto5.png"></div>
      <div class="slide fade"><img src="foto6.png" alt="foto6.png"></div>
      <div class="slide fade"><img src="foto7.png" alt="foto7.png"></div>
    </div>
    <p>Halo semuanyaa! Inilah kisahku sebagai mahasiswi ilmu komputer di Universitas Negeri Medan😊. Saya anak ke dua dari dua bersaudara. Menjadi orang pertama peraih gelar sarjana di keluarga adalah mimpiku, yang disertai dengan doa ibuku dan keluargaku. Ya, inilah perjalananku yang dimulai dari pengumuman SNBT Tahun 2024!! </p>
  </section>

  <section id="data-diri">
    <h2>Data Diri 📌</h2>
    <p><b>Nama:</b> Claudia Agatha Br Tarigan</p>
    <p><b>NIM:</b> 4243250027</p>
    <p><b>Agama:</b> Katolik</p>
    <p><b>Tempat tanggal lahir:</b> Pancur Batu, 21 Mei 2006</p>
    <p><b>Alamat:</b> Jalan Delitua, Dusun 1 Desa Namo Bintang</p>
    <p><b>Hobi :</b> Memasak, bernyanyi, edit foto/video</p>
  </section>

  <section id="pendidikan">
    <h2>Riwayat Pendidikan ✍</h2>
    <div class="edu-card">
      <img src="sekolah1.webp" alt="SD">
      <div><b>SD:</b> METHODIST-AN PANCUR BATU </div>
    </div>
    <div class="edu-card">
      <img src="sekolah2.jpg" alt="SMP">
      <div><b>SMP:</b> NEGERI 1 PANCUR BATU</div>
    </div>
    <div class="edu-card">
      <img src="sekolah3.jpg" alt="SMA">
      <div><b>SMA:</b> NEGERI 1 PANCUR BATU</div>
    </div>
  </section>

  <section id="organisasi">
    <h2>Organisasi yang Diikuti</h2>
    <div class="org-card">
      <h3>OSIS SMA (2022/2023) </h3>
      <p>Sebagai anggota bidang keagamaan. Aktif dalam kegiatan rohani atau acara keagamaan.</p>
      <img src="organisasi1.jpg" alt="Foto OSIS SMA">
    </div>
    <div class="org-card">
      <h3>Pengurus Komunitas Siswa-Siswi Katolik (2022-2024) </h3>
      <p>Bersatu dalam Iman, Bertumbuh dalam Kasih, Melayani dengan Sukacita</p>
      <img src="organisasi2.jpg" alt="Foto Pengurus KSSK">
    </div>
    <div class="org-card">
      <h3> Pengurus Orang Muda Katolik di Gereja (2023-2025) </h3>
      <p>Sebagai sekretaris, saya mencatat setiap langkah pelayanan, menjaga keteraturan, dan menghadirkan kasih Kristus dalam kebersamaan</p>
      <img src="organisasi4.jpg" alt="Foto UKM Paduan Suara">
    </div>
    <div class="org-card">
      <h3> Guru Sekolah Minggu (2019-sekarang) </h3>
      <p>Guru Sekolah Minggu yang melayani dengan kasih, menuntun anak-anak bertumbuh dalam iman</p>
      <img src="organisasi3.jpg" alt="Foto UKM Paduan Suara">
      <img src="organisasi5.jpg" alt="Foto UKM Paduan Suara">
    </div>
  </section>

  <section id="prestasi">
    <h2>Prestasi 🤩</h2>
    <div class="tabs">
      <div class="tab-buttons">
        <button onclick="showTab('daftar')">📜 Daftar Prestasi</button>
        <button onclick="showTab('album')">🖼️ Album Foto</button>
      </div>
      <div id="daftar" class="tab-content active">
        <ul>
          <li>Juara Kelas dari kelas 1-6 SD </li>
          <li>Peserta OSN bidang Fisika tingkat provinsi</li>
          <li>Peserta OSN tingkat mahasiswa bidang bahasa indonesia dan bahasa inggris </li>
        </ul>
      </div>
      <div id="album" class="tab-content">
        <div class="gallery">
          <img src="prestasi1.jpg" alt="Prestasi 1">
          <img src="prestasi2.jpg" alt="Prestasi 2">
          <img src="prestasi3.jpg" alt="Prestasi 3">
          <img src="sertifikat3.png" alt="Prestasi 4">
          <img src="sertifikat2.png" alt="Prestasi 5">
          <img src="sertifikat4.png" alt="Prestasi 6">
        </div>
      </div>
    </div>
  </section>

  <section id="funfact">
    <h2> Fun Fact Tentang Aku</h2>
    <div class="funfact-list">
      <div class="funfact-card">aku suka nyanyi di kamar mandi atau lagi jalan sendiri</div>
      <div class="funfact-card">aku suka ketawa sendiri gara-gara hal receh</div>
      <div class="funfact-card">aku tidak suka telur setengah matang</div>
      <div class="funfact-card">aku kalo tidur siang bangunnya bisa malam hari </div>
      <div class="funfact-card">aku tidak suka pembayaran online, dan aku tidak punya akun sejenis itu</div>
    </div>
  </section>

  <section id="cita-cita">
    <h2>🌟 Cita-Cita</h2>
    <p>Saya bercita-cita menjadi seorang Data Scientist/Analyst yang mempelajari cara mengolah dan menganalisis data agar bisa memberikan infromasi yang bermanfaat. Saya juga bercita-cita menjadi dosen di Universitas ternama. Dengan mendapatkan gaji yang besar, saya juga ingin membangun usaha sampingan seperti rumah kontrakan untuk masa depan yang lebih mandiri dan bermanfaat. Meskipun saya tidak berasal dari sekolah kejuruan dan ahli dalam komputer, namun saya yakin jika saya selalu berusaha dan terus belajar, saya pasti bisa!! </p>
    <div style="text-align: center; margin-top: 20px;">
      <img src="citacita.jpg" alt="Foto Cita-Cita" style="width: 300px; border-radius: 15px; box-shadow: 0 4px 8px rgba(0, 0, 0, 0.3);">
    </div>
  </section>

  <section id="harapan">
    <h2>💫 Harapan</h2>
    <p>Harapan saya adalah dapat menyelesaikan studi saya di jurusan Ilmu Komputer dengan baik dan tepat waktu, sehingga bisa segera mengaplikasikan ilmu yang saya pelajari di dunia kerja. Saya ingin menjadi seorang Data Scientist yang mampu mengolah dan menganalisis data untuk memberikan solusi dan manfaat bagi masyarakat. Selain itu, saya juga berharap dapat membangun usaha seperti kontrakan sebagai langkah menuju kemandirian finansial di masa depan. Saya ingin terus berkembang, beradaptasi dengan perkembangan teknologi, dan tetap rendah hati dalam setiap pencapaian. Yang paling penting, saya berharap ibu saya selalu diberikan kesehatan dan panjang umur, sehingga dapat menyaksikan perjalanan saya hingga sukses nanti.</p>
    <div style="text-align: center; margin-top: 20px;">
      <img src="ibuu.jpg" alt="Foto Cita-Cita" style="width: 300px; border-radius: 15px; box-shadow: 0 4px 8px rgba(0, 0, 0, 0.3);">
    </div>
  </section>

  <section id="kontak">
    <h2>Kontak Saya</h2>
    <div class="kontak-container">
      <div class="kontak-box">
        <span>📞</span>
        <span>085763376610</span>
      </div>
      <div class="kontak-box">
        <span>📷</span>
        <span>claudiia_agatha</span>
      </div>
      <div class="kontak-box">
        <span>▶️</span>
        <span>@claudiaagatha3944</span>
      </div>
      <div class="kontak-box">
        <span>✉️</span>
        <span>claudiaagatha5@gmail.com</span>
      </div>
    </div>
  </section>

  <script>
    // Musik
    const musik = document.getElementById("musik");
    const btn = document.getElementById("musik-btn");

    let isPlaying = false;
    btn.addEventListener("click", () => {
      if (isPlaying) {
        musik.pause();
        btn.innerHTML = "🎶";
      } else {
        musik.play();
        btn.innerHTML = "⏸️";
      }
      isPlaying = !isPlaying;
    });

    // Slideshow
    let slideIndex = 0;
    showSlides();
    function showSlides() {
      let slides = document.getElementsByClassName("slide");
      for (let i = 0; i < slides.length; i++) slides[i].style.display = "none";
      slideIndex++;
      if (slideIndex > slides.length) { slideIndex = 1 }
      slides[slideIndex - 1].style.display = "block";
      setTimeout(showSlides, 4000);
    }

    // Tab prestasi
    function showTab(tabId) {
      let tabs = document.querySelectorAll(".tab-content");
      tabs.forEach(tab => tab.classList.remove("active"));
      document.getElementById(tabId).classList.add("active");
    }
    
    // Inisialisasi tab "daftar" sebagai tab aktif saat halaman dimuat
    document.addEventListener('DOMContentLoaded', () => {
      showTab('daftar');
    });
  </script>

</body>
</html>
