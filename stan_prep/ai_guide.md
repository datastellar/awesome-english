# Panduan untuk Asisten AI

Dokumen ini menjelaskan struktur proyek dan alur kerja untuk program belajar intensif Bahasa Inggris persiapan tes PKN STAN.

## Struktur Folder

*   `/stan_prep/`: Direktori utama untuk semua materi persiapan.
    *   `/assessments/`: Menyimpan hasil dari semua asesmen yang dilakukan. Hasil disimpan dalam format JSON untuk kemudahan analisis.
        *   `initial_assessment.json`: Hasil asesmen awal untuk menentukan level kemampuan pengguna.
        *   `monthly_assessment_M{nomor_bulan}.json`: Hasil asesmen bulanan.
    *   `/study_plan/`: Berisi semua rencana belajar.
        *   `study_plan_6_months.md`: Rencana belajar garis besar selama 6 bulan.
        *   `week_{nomor_minggu}_plan.md`: Rencana belajar mingguan yang akan dibuat berdasarkan permintaan pengguna.
*   `ai_guide.md`: File ini. Berisi panduan untuk AI.

## Alur Kerja

1.  **Asesmen Awal:** Program dimulai dengan asesmen awal untuk mengukur kemampuan dasar pengguna dalam Grammar, Vocabulary, dan Reading Comprehension. Hasilnya disimpan di `/assessments/initial_assessment.json`.

2.  **Rencana Belajar 6 Bulan:** Berdasarkan hasil asesmen awal dan target (nilai maksimal TBI STAN), sebuah rencana belajar garis besar dibuat (`/study_plan/study_plan_6_months.md`).

3.  **Rencana Belajar Mingguan:** Setiap minggu, pengguna akan meminta rencana belajar yang lebih detail. Buat rencana ini (`/study_plan/week_{nomor_minggu}_plan.md`) berdasarkan:
    *   Fokus yang ada di rencana 6 bulan.
    *   Progres dan kesulitan yang dihadapi pengguna di minggu sebelumnya.
    *   Sumber daya yang tersedia di `readme.md`.

4.  **Asesmen Bulanan:** Di akhir setiap bulan, lakukan asesmen untuk mengukur kemajuan. Simpan hasilnya dan sesuaikan rencana untuk bulan berikutnya jika diperlukan.

## Tugas AI

*   **Memandu Pengguna:** Bimbing pengguna melalui rencana belajar mingguan.
*   **Membuat Rencana Mingguan:** Buat rencana belajar yang detail dan relevan setiap minggu.
*   **Memberikan Latihan:** Berikan latihan soal yang sesuai dengan materi minggu tersebut.
*   **Menganalisis Hasil:** Analisis hasil asesmen untuk mengidentifikasi kekuatan dan kelemahan.
*   **Menyesuaikan Rencana:** Jadilah fleksibel dan sesuaikan rencana belajar berdasarkan feedback dan progres pengguna.
