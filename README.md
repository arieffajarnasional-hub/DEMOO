# DEMOO — ARISA Edge-AI Leaf Diagnostic & Benchmark Station

Progressive Web App (PWA) interaktif untuk pemindaian, visualisasi segmentasi lesi U-Net, dan evaluasi benchmark model AI penyakit daun padi pada sistem **ARISA (Agronomic Risk Intelligence System for Agriculture)** untuk ajang **OPSI 2026**.

## Fitur Utama

1. **Benchmark Daun Langsung (Instant Diagnostic Benchmark)**:
   - Pilih sampel daun dari galeri (Blas Daun, Hawar Bakteri, Bercak Cokelat, Kontrol Sehat) atau gunakan fitur Acak.
   - Analisis dan metrik benchmark muncul seketika (zero latency).
2. **Dual-View Visual Inspection**:
   - Beralih instan antara **Citra Asli Lapangan (Raw RGB)** dan **Overlay Segmentasi U-Net (Kontur Kanopi & Mask Lesi)**.
3. **Metrik Diagnostik Komprehensif**:
   - Akurasi / Keyakinan Model INT8 Edge
   - Disease Severity Index (DSI %) & Kuantifikasi Piksel
   - Klasifikasi Fase Pertumbuhan (Vegetatif, Generatif, Pemasakan, Panen)
   - Skor Indeks Risiko Terintegrasi (IARI) & Tingkat Risiko (Rendah / Sedang / Tinggi)
4. **Benchmark Perangkat Keras (Edge vs Cloud)**:
   - Latensi Edge (Raspberry Pi 4 INT8: ~412 ms) vs Cloud Server (~89 ms)
   - Efisiensi kompresi model (4.7 MB INT8 vs 49 MB FP32)
   - Validasi Gatekeeper Kanopi Padi (ExG, NGRDI, Dominasi Merah)
5. **Rekomendasi Agronomi & PPL Terarah**:
   - Panduan tindakan teknis lapangan, manajemen pupuk N/P/K, dan aplikasi fungisida/bakterisida terukur.
6. **Siap Deployment Railway & GitHub**:
   - Dilengkapi server produksi Node.js mandiri (`server.js`), healthcheck `/health`, konfigurasi `railway.json`, dan `Procfile`.
