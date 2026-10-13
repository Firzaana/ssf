# Data Heat Island – Riset Remote Sensing

Replikasi dan adaptasi analisis *data heat island effect* (kenaikan Land Surface Temperature di sekitar AI data center) berdasarkan paper acuan Marinoni et al. (2026), arXiv:2603.20897. Struktur folder mengikuti spreadsheet "TIMELINE REMOTE SENSING" (Oktober 2026).

## Struktur folder (urut sesuai timeline)

| Folder | Tahap timeline |
|---|---|
| `01_dataset_finalization` | Finalisasi dataset |
| `02_roi_and_timeframe` | Finalisasi area studi (ROI) dan rentang waktu |
| `03_literature_review` | Studi literatur |
| `04_data_availability_check` | Cek ketersediaan data pada area studi / coding citra satelit |
| `05_small_scale_method_testing` | Menguji beberapa metode di sampel/area kecil |
| `06_data_cleaning_algorithm` | Algoritma kebersihan data di area studi |
| `07_training_and_qc_stage1` | Training dan quality control permasalahan algoritma tahap 1 |
| `08_sample_evaluation` | Evaluasi pengambilan sampel data |
| `09_equations_and_parameters` | Persamaan dan parameter dalam bentuk coding |
| `10_study_area_implementation` | Implementasi metode ke area studi |
| `11_comparison_with_reference_paper` | Bandingkan hasil dengan paper acuan |
| `12_evaluation_stage2` | Evaluasi permasalahan algoritma tahap 2 |
| `13_time_series_implementation` | Implementasi ke tanggal dan bulan berbeda (time series) |

Folder pendukung: `data/` (raw, interim, processed), `src/` (kode), `notebooks/`, `results/`, `docs/`.

## Data utama (dari paper acuan)
- MODIS LST (reconstructed, 500 m, 2004-2024)
- Lokasi data center: DataCenterMap / Baxtel / datacenters.com
- Populasi: WorldPop 100 m (downscale ke 1 km)
- Opsional: Sentinel-2, Landsat (NDVI), ECOSTRESS LST

Lihat `docs/timeline.md` untuk jadwal dan `03_literature_review/notes/reading_list.md` untuk daftar bacaan.
