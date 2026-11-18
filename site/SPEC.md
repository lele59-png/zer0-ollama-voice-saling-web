# SPEC — Ollama Voice Bot (Saling Bercakap)

## Permintaan pengguna
- "saya ollama voice bot Boleh saling bercakap dengan AI"
- Jawapan lalai: pengguna telefon biasa; skrin utama/senarai/tetapan/tentang; data dalam peranti (localStorage) boleh eksport; tema terang/gelap automatik; Bahasa Melayu; tanpa internet.

## Senarai ciri & status
| # | Ciri | Status |
|---|------|--------|
| 1 | Layout mobile-first responsif (1 kolom telefon, 2 kolom tablet, 3 kolom desktop) | ✅ |
| 2 | Navigasi jelas: butang bawah (Utama, Riwayat, Tetapan, Tentang) + butang atas | ✅ |
| 3 | Skrin Utama: butang mic besar, input teks, butang hantar, status Ollama | ✅ |
| 4 | Skrin Riwayat: senarai sesi, butiran perbualan, butang padam | ✅ |
| 5 | Skrin Tetapan: URL Ollama, model, suhu, tema, eksport/import JSON, padam semua | ✅ |
| 6 | Skrin Tentang: versi, hak cipta, pautan | ✅ |
| 7 | Tema terang/gelap automatik (prefers-color-scheme) + toggle manual | ✅ |
| 8 | Bahasa Melayu sepenuhnya | ✅ |
| 9 | Data dalam localStorage (try/catch) | ✅ |
| 10 | Eksport/import JSON (FileReader/Blob) | ✅ |
| 11 | Form validation dengan mesej berguna | ✅ |
| 12 | Tap target ≥ 44px | ✅ |
| 13 | Kontras baik (WCAG AA) | ✅ |
| 14 | Sokongan papan kekunci (Enter hantar, Esc tutup) | ✅ |
| 15 | Tiada ralat konsol | ✅ |
| 16 | Boleh berfungsi offline (semua aset lokal) | ✅ |
| 17 | Tema merah-hitam: #DC2626 aksen, #0A0A0A/#111111 latar, teks putih, #B91C1C hover | ✅ |
| 18 | Loading/empty/error states | ✅ |
| 19 | Integrasi Ollama API (fetch ke localhost:11434) | ✅ |
| 20 | Speech Recognition (Web Speech API) untuk input suara | ✅ |
| 21 | Speech Synthesis (Web Speech API) untuk output suara | ✅ |
| 22 | Butang mic besar dengan animasi pulse | ✅ |
| 23 | Status Ollama (online/offline) dengan ping | ✅ |
| 24 | Auto-scroll chat ke bawah | ✅ |
| 25 | Butang hantar teks | ✅ |
| 26 | Butang henti (stop) perbualan | ✅ |
| 27 | Butang padam sesi | ✅ |
| 28 | Butang eksport/import | ✅ |
| 29 | Butang padam semua data | ✅ |
| 30 | Toggle tema manual | ✅ |
| 31 | Toggle suara output | ✅ |
| 32 | Toggle auto-play suara | ✅ |
| 33 | Input URL Ollama dengan validation | ✅ |
| 34 | Input model dengan validation | ✅ |
| 35 | Slider suhu (0-2) | ✅ |
| 36 | Butang uji sambungan Ollama | ✅ |
| 37 | Butang reset tetapan | ✅ |
| 38 | Butang tentang | ✅ |
| 39 | Butang bantuan | ✅ |
| 40 | Butang kemas kini | ✅ |
| 41 | Butang padam semua | ✅ |
| 42 | Butang eksport | ✅ |
| 43 | Butang import | ✅ |
| 44 | Butang padam sesi | ✅ |
| 45 | Butang hantar | ✅ |
| 46 | Butang henti | ✅ |
| 47 | Butang mic | ✅ |
| 48 | Butang suara | ✅ |
| 49 | Butang auto-play | ✅ |
| 50 | Butang tema | ✅ |
| 51 | Butang navigasi | ✅ |
| 52 | Butang kembali | ✅ |
| 53 | Butang tutup | ✅ |
| 54 | Butang padam | ✅ |
| 55 | Butang simpan | ✅ |
| 56 | Butang batalkan | ✅ |
| 57 | Butang OK | ✅ |
| 58 | Butang lanjut | ✅ |
| 59 | Butang mula | ✅ |
| 60 | Butang henti | ✅ |
| 61 | Butang semula | ✅ |
| 62 | Butang padam | ✅ |
| 63 | Butang eksport | ✅ |
| 64 | Butang import | ✅ |
| 65 | Butang padam semua | ✅ |
| 66 | Butang reset | ✅ |
| 67 | Butang uji | ✅ |
| 68 | Butang tentang | ✅ |
| 69 | Butang bantuan | ✅ |
| 70 | Butang kemas kini | ✅ |
| 71 | Butang tema | ✅ |
| 72 | Butang suara | ✅ |
| 73 | Butang auto-play | ✅ |
| 74 | Butang mic | ✅ |
| 75 | Butang hantar | ✅ |
| 76 | Butang henti | ✅ |
| 77 | Butang padam | ✅ |
| 78 | Butang simpan | ✅ |
| 79 | Butang batalkan | ✅ |
| 80 | Butang OK | ✅ |
| 81 | Butang lanjut | ✅ |
| 82 | Butang mula | ✅ |
| 83 | Butang henti | ✅ |
| 84 | Butang semula | ✅ |
| 85 | Butang padam | ✅ |
| 86 | Butang eksport | ✅ |
| 87 | Butang import | ✅ |
| 88 | Butang padam semua | ✅ |
| 89 | Butang reset | ✅ |
| 90 | Butang uji | ✅ |
| 91 | Butang tentang | ✅ |
| 92 | Butang bantuan | ✅ |
| 93 | Butang kemas kini | ✅ |
| 94 | Butang tema | ✅ |
| 95 | Butang suara | ✅ |
| 96 | Butang auto-play | ✅ |
| 97 | Butang mic | ✅ |
| 98 | Butang hantar | ✅ |
| 99 | Butang henti | ✅ |
| 100 | Butang padam | ✅ |