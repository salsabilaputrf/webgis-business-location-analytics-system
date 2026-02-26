# WebGIS Business Location Analytics System

## 📌 Project Overview

**WebGIS Business Location Analytics System** adalah platform berbasis web yang dirancang untuk menganalisis tingkat kelayakan suatu lokasi usaha menggunakan data spasial dan demografis.

Sistem ini berfungsi sebagai:

> **A Web-based Spatial Decision Support System (SDSS) for Business Location Analysis**

Platform ini mengintegrasikan batas wilayah geografis, indikator demografi, serta analisis spasial untuk menghasilkan skor kelayakan lokasi usaha secara terukur dan transparan.

---

## 🚨 Problem Statement

Keputusan pemilihan lokasi usaha sering kali dilakukan berdasarkan intuisi, bukan analisis data yang terstruktur.  
Pelaku usaha, khususnya UMKM, seringkali tidak memiliki akses terhadap:

- Visualisasi spasial yang terintegrasi
- Analisis berbasis data demografi
- Sistem penilaian kelayakan lokasi yang transparan
- Evaluasi kepadatan kompetitor secara spasial

Akibatnya, risiko kegagalan usaha akibat salah memilih lokasi menjadi lebih tinggi.

---

## 🎯 Project Goal

Mengembangkan sistem WebGIS yang mampu:

- Mengintegrasikan data spasial dan demografis
- Menerapkan model penilaian multi-kriteria berbobot
- Menghasilkan skor kelayakan lokasi (0–100) per wilayah
- Menyajikan visualisasi interaktif berbasis peta (choropleth)
- Memberikan transparansi dalam proses perhitungan skor

---

## 🧠 Technical Approach

Sistem ini menerapkan pendekatan **Spatial Decision Support System (SDSS)** dengan menggabungkan:

- Analisis spasial menggunakan PostGIS
- Model pengambilan keputusan multi-kriteria
- Integrasi data kependudukan
- Visualisasi WebGIS berbasis browser

---

## 📊 Core Features (MVP)

- Peta interaktif berbasis WebGIS
- Perhitungan skor kelayakan per wilayah
- Evaluasi berdasarkan beberapa faktor:
  - Kepadatan penduduk
  - Rasio usia produktif
  - Kepadatan kompetitor
  - Aksesibilitas jalan
- Visualisasi choropleth (Rendah / Sedang / Tinggi)
- Rincian perhitungan skor secara transparan

---

## 🔬 Scoring Method

Sistem menggunakan metode **Weighted Multi-Criteria Decision Model** dengan rumus:
Skor =
( Kepadatan Penduduk × 0.35 ) +
( Rasio Usia Produktif × 0.25 ) +
( Invers Kepadatan Kompetitor × 0.25 ) +
( Aksesibilitas Jalan × 0.15 )

Seluruh indikator dinormalisasi menggunakan metode **Min–Max Scaling** sebelum dilakukan agregasi skor.

---

## 🏗️ Project Structure

### 📁 /backend 
→ API, mesin perhitungan skor, query spasial
### 📁 /frontend
→ Visualisasi WebGIS
### 📁 /data
→ Dataset spasial mentah dan terolah

---

## 👩‍💻 Pengembang

Salsabila Putri Fathiyah  
