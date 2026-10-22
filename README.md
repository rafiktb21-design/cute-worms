# 🐛 Cute Worms 3D - Game Cacing & Buah Segar 🍉✨

Game Cacing/Snake 3D penuh bertema ceria dan menggemaskan yang dibangun dengan **Three.js** dan WebGL. Dilengkapi pencahayaan dinamis, bayangan lembut real-time (*soft shadows*), animasi lokomosi cacing sub-tick yang halus, pulau taman melayang alami, dan 12 model buah 3D prosedural!

## ✨ Fitur Utama 3D

- **Mode Layar Penuh (Fullscreen) & Sudut Pandang Leluasa**:
  - **Layar Penuh Instan (`F` / Tombol ⛶)**: Menampilkan seluruh layar penuh (*100vw x 100vh*) tanpa batasan bingkai, dilengkapi HUD 3D mengambang modern (skor, rekor, target buah segar, kontrol musik, kontrol suara, dan tombol keluar).
  - **Dialog Pop-Up 3D Rapi & Proporsional**: Kotak pop-up dialog (Mulai, Pause, Game Over) tampil sebagai kartu modal 3D terpusat yang presisi, estetik, dan tidak memanjang ke bawah.
  - **Kamera Tenang & Bebas Getaran Saat Makan**: Getaran layar saat memakan buah telah ditiadakan sepenuhnya sehingga pandangan mata pemain tetap stabil, nyaman, dan fokus.
  - **3 Pilihan Sudut Pandang Kamera (`C` / `V` / Tombol 📷)**:
    - **Lebar (Wide - Default)**: Sudut pandang luas, lega, dan lapang dengan FOV optimal dan kompensasi otomatis pada layar vertikal (portrait).
    - **Atas (Top-Down)**: Sudut pandang vertikal murni gaya *arcade* klasik untuk navigasi bebas hambatan.
    - **Santai (Cozy)**: Sudut isometrik sinematik 3D yang hangat dan estetik.
  - **Arena Bermain Bebas Halangan (100% Clear View)**: Posisi awan 3D dipindahkan jauh ke angkasa belakang (`z: -20` s/d `-34`, `y: 14` s/d `19`) dan lebah madu berpatroli di luar dinding luar pulau sehingga cacing, buah segar, dan arena bermain selalu terlihat jelas tanpa tertutup awan sama sekali.

- **Audio Ceria Lengkap (Musik Latar BGM & SFX)**:
  - **Backsound Musik BGM Santai**: Melodi marimba & chiptune bergaya Nintendo/Animal Crossing yang ceria, santai, dan ramah anak, disintesis langsung secara prosedural via Web Audio API tanpa membutuhkan file MP3 eksternal.
  - **Tombol & Pintasan Mute Musik Mandiri (`M` / Tombol 🎵)**: Pemain dapat mematikan atau menyalakan musik latar secara terpisah dari efek suara (SFX) kapan saja.
  - **Efek Suara Imut (SFX)**: Suara makan buah *pop-chime*, belok halus, dan jingle *game over*.

- **Dunia 3D Penuh & Pulau Taman Alami**:
  - **Latar Belakang & Panorama Diorama 3D Cerah (Bukan Biru Polos)**:
    - **Gradasi Langit Cerah Menawan**: Langit biru cerah berlapis dengan transilusi hangat fajar (*azure blue* ke *peach dawn*).
    - **Pelangi 3D Melengkung Megah**: Busur pelangi 6 warna pastel 3D di cakrawala dengan tumpuan awan putih lembut di kedua ujungnya.
    - **Matahari 3D Tersenyum dengan Sinar Berputar**: Matahari kartun ceria dengan pipi merona dan 10 sinar emas yang berputar terus-menerus.
    - **Balon Udara Lucu Bergaris**: Melayang santai melintasi langit dengan keranjang gantung dan gerakan mengapung lembut.
    - **Pulau Satelit Mini Kincir Angin & Kelinci Lucu**: Pulau mini di barat laut lengkap dengan kincir angin yang bilahnya berputar mulus dan kelinci putih gemas yang melompat-lompat ceria serta menggoyangkan telinganya.
    - **Pulau Satelit Mini Pondok & Burung Pipit Kuning**: Pulau mini di timur laut dengan pondok mungil berasap dan burung pipit kuning yang mengangguk-angguk di pagar kayu.
    - **3 Kupu-kupu Kartun Cantik Berterbangan**: Kupu-kupu pink, kuning, dan toska yang mengepakkan sayap dengan lincah mengitari tepian taman bermain.
    - **Lautan Awan Mengambang di Bawah Pulau**: Gumpalan awan halus di kedalaman langit yang memberikan sensasi pulau melayang di nirwana fantasi.
  - **Latar Rumput Hijau Zamrud**: Arena bermain berupa padang rumput hijau cerah alami tanpa garis kotak-kotak (*no checkerboard / grid lines*).
  - **Pencahayaan Tone Mapping ACES (Bebas Overexposure)**: Dilengkapi `ACESFilmicToneMapping` yang mencegah efek silau/kabut putih berlebih, menghasilkan warna-warna cerah, kaya, dan berkilau (*saturated & vibrant*).
  - **Pulau Melayang (Floating Island)**: Struktur pulau taman mengambang dengan tebing tanah cokelat manis, pembatas batu alam, jamur polkadot 3D aneka warna, maskot lebah madu 3D melayang dengan sayap bergetar, serta puluhan bunga daisy, kosmos pink, lonceng ungu, dan semanggi yang bergoyang tertiup angin.
  - **Pencahayaan & Bayangan Lembut Real-Time**: Kombinasi *HemisphereLight* langit-bumi alami, sinar matahari hangat (*Directional Sunlight*) dengan bayangan halus *PCFSoftShadowMap*, cahaya permata buah (*point light lantern*), dan lampu sorot cacing (*headlight*).
  - **Kamera Perspektif Isometrik Diorama**: Sudut pandang *tilt perspective* isometrik 40° yang memberikan sensasi miniatur lucu dan imut.

- **Antarmuka 3D Penuh (3D Skeuomorphic / Kawaii Claymorphism)**:
  - Tombol aksi 3D tebal dan membal dengan efek tekan fisik (*tactile 3D press*).
  - Frame konsol 3D bergaya game portabel dengan bevel mengkilap dan bayangan dalam.
  - Carousel skin 3D dengan kartu timbul dan preview emoji melayang.
  - Papan skor dan banner buah 3D emboss dengan efek pop animasi menggemaskan.

- **Karakter Cacing 3D Ultra-Cute & Unik (Royal Kawaii Worm)**:
  - **Pergerakan Sub-Tick 60 FPS**: Interpolasi gerakan *smoothstep* sub-tick membuat cacing merayap dengan gelombang lokomosi ulat (*caterpillar wave*) lentur tanpa patah-patah.
  - **Ruas Tubuh Empuk & Ornamen Mutiara Punggung**: Ruas badan bola lembut dengan mutiara emas pastel berkilau di punggung segmen.
  - **Kaki Tapak Mungil (Cute Squishy Paws)**: Sepasang kaki kecil menggemaskan di sisi setiap ruas badan yang mengayun ritmis seperti tapak kaki cilik yang lincah.
  - **Ekor Rattle Lonceng Emas (*Lucky Tail Rattle*)**: Ujung ekor berhiaskan lonceng emas berkilau dan cincin rattle yang bergoyang ceria.
  - **Kepala Ekspresif & Menggemaskan**:
    - **Mahkota Mini Kerajaan Emas (*Royal Golden Tiara*)**: Mahkota mungil emas murni bertatahkan 5 butir permata warna-warni (Ruby, Sapphire, Emerald, Amethyst, Topaz) yang bergoyang anggun di atas kepala.
    - **Tunas Daun Keberuntungan & Bunga Sakura (*Lucky Sprout with Sakura Blossom*)**: Tangkai tunas hijau dengan bunga sakura mekar di sisi mahkota.
    - **Mata Kristal Anime Kawaii 3 Catchlight**: Mata bola kaca besar dengan iris gelap memikat, 3 titik kilau bintang (*triple specular catchlights*), bulu mata melengkung, dan kedipan bahagia saat memakan buah (`^ ^`).
    - **Moncong Chubby & Hidung Mungil**: Bentuk moncong bulat boneka dengan hidung kancing pink manis.
    - **Mulut Chomping dengan Lidah Menjulur (*Playful Wagging Tongue*)**: Mulut yang membuka-menutup riang dengan lidah pink kenyal yang bergetar menggemaskan saat bergerak.
    - **Pipi Merona Berbintang (*Blushing Cheeks with Twinkle Accent*)**: Pipi merah muda lembut berpendar kilau bintang.
    - **Antena Kristal Bercahaya**: Sepasang antena pegas berujung bola kristal yang memancarkan pendaran lembut (*emissive glow*) dan bergoyang membal.

- **12 Koleksi Model Buah 3D Prosedural PBR**:
  Setiap buah dirancang dengan geometri 3D prosedural, material mengkilap (*MeshStandardMaterial*), bayangan real-time, animasi melayang/rotasi santai, dan 3 bintang emas ajaib yang mengorbit:
  1. 🍉 **Semangka**: Potongan semangka merah segar dengan biji hitam dan kulit hijau berlapis.
  2. 🍓 **Stroberi**: Stroberi montok bermahkota daun kelopak hijau dan tangkai.
  3. 🍌 **Pisang**: Pisang kuning melengkung manis dengan ujung cokelat alami.
  4. 🍇 **Anggur**: Gugusan buah anggur ungu berkilau dengan daun ranting.
  5. 🍊 **Jeruk**: Jeruk oranye segar lengkap dengan tangkai dan daun.
  6. 🍎 **Apel Merah**: Apel merah mengilap dengan lekukan tangkai dan daun.
  7. 🍏 **Apel Hijau**: Apel hijau renyah yang segar.
  8. 🍍 **Nanas**: Nanas manis bermahkota daun hijau runcing.
  9. 🍒 **Ceri**: Sepasang buah ceri merah tua dengan tangkai lengkung ganda.
  10. 🥑 **Alpukat**: Belahan alpukat hijau mentega dengan biji bulat cokelat.
  11. 🍋 **Lemon**: Lemon kuning cerah dengan ujung khas dan daun.
  12. 🍑 **Persik**: Buah persik merah muda lembut dengan belahan manis.

- **Efek Partikel 3D & Audio Imut**:
  - Percikan sari buah 3D (*juice burst*), bintang bertaburan, cincin gelombang kejut lantai (*shockwave rings*), jejak debu bintang (*stardust trail*), dan teks skor 3D melayang (+10 Nama Buah).
  - Hentakan kamera mikro (*3D camera shake*) yang lembut saat makan atau menabrak.
  - Suara makan dan game over yang disintesis langsung menggunakan Web Audio API tanpa perlu file eksternal.

- **6 Pilihan Skin Cacing Unik**:
  - 🍓 Mimi Berry (Stroberi Pink)
  - 🥑 Mochi Matcha (Alpukat/Matcha)
  - 🦄 Rainbow Sky (Pelangi Ajaib)
  - 🐝 Bubu Bee (Lebah Madu)
  - 🧋 Taro Boba (Boba Manis)
  - 🍬 Blueberry Fluff (Permen Kapas)

- **Kemudahan Akses**:
  - Menggunakan library Three.js (r128) lokal yang sudah disertakan (`three.min.js`), dengan fallback CDN otomatis.
  - Kontrol lengkap: Keyboard (WASD / Tombol Panah / Spasi), Virtual D-Pad, dan Touch Swipe untuk smartphone & tablet.
  - Skor tertinggi otomatis tersimpan di `localStorage`.

## 🚀 Cara Menjalankan
Buka file `index.html` langsung di browser modern mana pun (Google Chrome, Microsoft Edge, Mozilla Firefox, Safari, dll.). Tidak memerlukan instalasi atau dependensi eksternal!

## 📄 Lisensi
MIT License
