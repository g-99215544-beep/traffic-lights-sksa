# Traffic Light SKSA

Aplikasi **Lampu Isyarat Kefahaman** untuk kegunaan guru dan murid SKSA.

## Fungsi utama

- Murid pilih kelas sahaja.
- Aplikasi memuatkan **murid yang hadir pada hari semasa** daripada Firebase Realtime Database.
- Setiap murid dipaparkan dalam satu kotak.
- Status awal murid ialah **?**.
- Murid tekan kotak nama sendiri dan pilih:
  - 🟢 Hijau — Faham
  - 🟡 Kuning — Kurang faham
  - 🔴 Merah — Tak faham
- Paparan guru dikemas kini secara **live**.
- Guru boleh melihat jumlah hijau, kuning, merah, belum jawab, serta majoriti kelas.
- Respons disimpan mengikut tarikh dan kelas.

## Firebase

Aplikasi menggunakan projek Firebase kehadiran sedia ada:

- Project ID: `kehadiran-murid-6ece0`
- Realtime Database: `kehadiran-murid-6ece0-default-rtdb.asia-southeast1.firebasedatabase.app`

Path yang digunakan:

- `config/classes/classData`
- `kehadiran/YYYY-MM-DD/<kelas>`
- `absenceStatus/YYYY-MM-DD/<kelas>`
- `trafficLight/YYYY-MM-DD/<kelas>`

## Fail

`index.html` — aplikasi utama.

## Nota

Pastikan Firebase Realtime Database Rules membenarkan bacaan data kelas/kehadiran dan penulisan ke path `trafficLight` untuk aplikasi berfungsi secara live.
