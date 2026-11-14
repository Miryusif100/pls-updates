# PLS — yeniləmələr

PLS Consulting-in e-taxes.gov.az üçün Chrome genişlənməsinin **imzalı** versiyaları.
Bu repoda yalnız quraşdırılan paketlər saxlanır; kod gizli repodadır.

## Quraşdırma (yeni kompüter)
1. [`installer/PLS-Qurasdirici.zip`](installer/PLS-Qurasdirici.zip) faylını yükləyin və açın (Extract all).
2. `PLS-Qurasdir.cmd` faylını iki dəfə klikləyin.
3. Ekrandakı son addımı edin: Chrome → `chrome://extensions` → Developer mode → **Load unpacked** → göstərilən qovluq.

Bundan sonra yeniləmələr avtomatikdir: Windows açılanda və hər saat yoxlanılır.
Hər paket PLS açarı ilə imzalanıb; imzası düzgün olmayan paket quraşdırılmır.

| Fayl | Məzmun |
|---|---|
| `latest.json` | Son versiya, faylın SHA-256 hash-i və imzası |
| `releases/` | Versiya paketləri |
| `installer/` | Quraşdırıcı |

## Kanallar və saxlama
- **Stabil kanal:** `latest.json` + `releases/` — bütün istifadəçilər. Yalnız sahibin `PLS-Burax` / «2-HAMIYA-GONDER» düyməsi ilə yenilənir.
- **Test kanalı:** `test/latest.json` + `test/releases/` — yalnız sahibin test rejimindəki kompüterləri.
- `releases/`-də yalnız son stabil paket və geri qaytarma üçün əvvəlki 2 paket saxlanır, qalanları silinir.
- Fayllar avtomatik yazılır (GitHub Actions); əl ilə dəyişməyin. Paket imzası yoxlanılmasa quraşdırılmır.
- Kod və qərarlar gizli repodadır; bu repoda yalnız paketlər var.
