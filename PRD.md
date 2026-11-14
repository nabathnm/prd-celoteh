# PRD Celoteh

## Timeline
11 – 19 November 2026

## Target User
* **Primary User:** Orang tua/wali anak usia 2–6 tahun dengan keterlambatan bicara (*speech delay*).
* **Secondary User:** Anak usia dini (pengguna sesi interaktif bersama orang tua).
* **Tertiary User:** Terapis wicara (penerima dokumentasi laporan latihan di rumah).

## SDGS
SDG 4 (Quality Education) – Sub-target 4.2: Akses stimulasi perkembangan bahasa anak usia dini yang inklusif dan menyenangkan.

## Konsep
Aplikasi pendamping stimulasi bicara anak di rumah melalui pembelajaran interaktif **berbasis minat anak (*interest-driven learning*)** yang menyatu dengan latihan suara (*voice recording*), reward gamifikasi, dan pemantauan perkembangan untuk orang tua.

## Link Figma
[Link Desain Figma Celoteh](https://figma.com)

## Overview
Celoteh adalah aplikasi pendamping stimulasi bicara anak yang membantu orang tua memberikan latihan bahasa dan komunikasi secara terarah di rumah melalui topik-topik yang diminati anak (hewan, kendaraan, buah, benda di rumah, dinosaurus, dan keluarga). Aplikasi ini mencakup seluruh alur pengalaman pengguna mulai dari Onboarding dan Authentication, pembuatan Child Profile berbasis minat, pemantauan aktivitas utama melalui Dashboard, pelaksanaan sesi belajar interaktif 4 tahap pada Learning Materials, hingga Progress Tracking secara berkala.

Celoteh bertujuan menjadikan stimulasi bicara bagian dari rutinitas harian yang menyenangkan, mudah diakses, konsisten, dan terdokumentasi dengan baik.

> **Catatan:** Celoteh adalah media pendamping stimulasi di rumah, bukan alat diagnosis medis dan bukan pengganti terapi wicara profesional.

## Problem Statement
Orang tua dengan anak yang mengalami keterlambatan bicara sering menghadapi tiga kesulitan utama:
1. **Anak Cepat Bosan & Tidak Termotivasi:** Metode latihan bicara konvensional yang kaku membuat anak enggan bersuara. Anak membutuhkan stimulasi melalui objek dan tema yang benar-benar mereka sukai.
2. **Bingung Memilih Stimulasi:** Sulit menentukan aktivitas dan materi kata yang relevan dan menyenangkan untuk dilatihkan di rumah.
3. **Perkembangan Tidak Terdokumentasi:** Tidak ada sarana mudah untuk mendokumentasikan rekaman suara dan perkembangan anak dari waktu ke waktu untuk dikonsultasikan ke terapis.

## How Might We
Bagaimana membantu orang tua melatih bicara anak di rumah melalui tema-tema yang disukai anak secara terstruktur, menyenangkan, dan terdokumentasi dengan baik?

## Product Goals
* Membantu orang tua melakukan stimulasi bicara berbasis minat anak secara terstruktur.
* Menyediakan media belajar interaktif audio-visual yang ramah anak dan bebas rasa takut salah.
* Meningkatkan konsistensi latihan harian di rumah melalui streak motivasi.
* Mempermudah dokumentasi rekaman suara dan catatan perkembangan anak untuk kebutuhan konsultasi dengan terapis.

## Flow
Buka Aplikasi → Onboarding → Register / Login → Child Profile (Pilih Minat Anak) → Dashboard → Belajar Tema Minat → Sesi 4 Tahap (Kenali → Tirukan → Rekam → Hore!) → Progress Tracking & Ekspor Terapis

## Features & UI Flow Ringkas

### 1. Onboarding
Tiga halaman pengenalan tentang stimulasi bicara berbasis suara dan minat anak, serta peran penting orang tua.
Flow: Onboarding Page 1 → Onboarding Page 2 → Onboarding Page 3 → Mulai Sekarang → Register / Login

### 2. Authentication
Gerbang masuk orang tua menggunakan email dan password, dengan alur pendaftaran, masuk akun, dan pemulihan kata sandi.
Flow: Buka Aplikasi → Login / Register → Child Profile (Pengguna Baru) / Dashboard (Pengguna Lama)

### 3. Child Profile
Pengisian identitas anak dan pemetaan tema minat favorit anak (hewan, buah, kendaraan, benda di rumah, dinosaurus, keluarga) serta kondisi awal komunikasi anak.
Flow: Register / Login → Buat Profil Anak → Pilih Minat & Tema Favorit → Kondisi Komunikasi → Gambaran Awal → Dashboard / Mulai Belajar

### 4. Dashboard
Pusat navigasi ringkasan tema minat aktif, streak latihan harian, ringkasan perbendaharaan kata, aktivitas belajar terakhir, dan tombol cepat "Lanjutkan Belajar".
Flow: Login / Selesai Profil → Dashboard → Lanjutkan Belajar / Pilih Tema / Lihat Progres

### 5. Learning Materials
Materi interaktif berbasis tema minat anak dengan sesi belajar 4 tahap (Kenali → Tirukan → Rekam → Hore!) yang menyatu dengan perekaman suara dan reward apresiasi tanpa vonis salah.
Flow: Beranda → Belajar → Pilih Tema → Pilih Subtema → Kenali → Tirukan → Rekam → Hore! → Subtema Berikutnya / Kembali ke Tema

### 6. Progress Tracking
Pemantauan capaian kata per tema minat, arsip dan komparasi rekaman suara anak, log aktivitas harian, catatan observasi orang tua, serta fitur ekspor laporan untuk terapis wicara.
Flow: Dashboard / Bottom Nav → Progress Tracking → Pilih Tab (Capaian Tema / Arsip Suara / Riwayat / Catatan) → Putar Rekaman / Tambah Catatan / Ekspor Laporan

## Hubungan Antar Fitur
* **Child Profile $\rightarrow$ Dashboard & Learning Material:** Tema favorit yang dipilih di profil anak langsung direkomendasikan pada kartu utama Dashboard dan diberi label "Rekomendasi" pada Learning Material.
* **Learning Material $\rightarrow$ Dashboard & Progress Tracking:** Setiap sesi belajar yang selesai langsung menambah streak latihan dan progres tema di Dashboard, serta otomatis mengirimkan rekaman audio anak ke tab Arsip Suara dan log latihan di Progress Tracking.
* **Progress Tracking $\rightarrow$ Terapis:** Data capaian kata, riwayat latihan, dan catatan observasi orang tua dapat diekspor menjadi laporan ringkas (PDF/WhatsApp) untuk bahan konsultasi terapis wicara.
