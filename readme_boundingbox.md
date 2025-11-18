# PROGRAM RUN DETEKSI OBJEK BOUNDING BOX

## 🚀 Cara Menjalankan

### masuk ke direktori 

**Opsi 1, Jalanin kode ini kalau mau hasilnya ga kesave **
```
python3 detect.py --weights yuwandbest.pt --source fourth.mp4 --view-img --nosave
```
*Biarkan jalan, jangan ditutup*


### **Opsi 2 — Menjalankan Deteksi dari Kamera (contoh lain)**

```bash
python3 detect.py --weights <path_ke_file.pt> --source 0
```

* `--source 0` berarti menggunakan webcam.
* Ganti `<path_ke_file.pt>` dengan lokasi file weight milikmu.

---

## 📌 Catatan

* Pastikan file `.pt` sesuai dengan model yang sudah kamu latih.
* Format source bisa berupa:

  * Path video (`.mp4`)
  * Folder gambar
  * Webcam (`0` atau index kamera lainnya)
* Jika ingin menyimpan hasil, cukup **hapus** argumen `--nosave`.
