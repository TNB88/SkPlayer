# SkPlayer

Kho nay dung de cap nhat online cho Smart Karaoke Player PRO.

## File app dang doc

APK da duoc sua de doc 2 file raw GitHub nay:

- `version.txt`
- `version_rtd.txt`

Duong dan raw trong app:

- `https://raw.githubusercontent.com/TNB88/SkPlayer/refs/heads/main/version.txt`
- `https://raw.githubusercontent.com/TNB88/SkPlayer/refs/heads/main/version_rtd.txt`

## Dinh dang file update

Moi file chi can 1 dong:

```txt
versionCode;versionName;apkUrl
```

Vi du ban hien tai:

```txt
416;3.56;https://raw.githubusercontent.com/TNB88/SkPlayer/refs/heads/main/SmartKaraokePlayerPRO_v3.56_newkey_bgok_v13_github_photo_15s_exitfix.apk
```

Y nghia:

- `416`: ma phien ban. App dang cai co `versionCode=416`.
- `3.56`: ten phien ban hien tren app.
- Link cuoi: link tai file APK moi.

## Cach ra ban update moi

1. Build APK moi.
2. Doi ten file APK cho de nho, vi du:
   `SmartKaraokePlayerPRO_v3.57.apk`
3. Upload APK do len repo nay.
4. Sua `version.txt` va `version_rtd.txt`.
5. Tang so dau len lon hon ban cu.

Vi du muon app bao co ban moi:

```txt
417;3.57;https://raw.githubusercontent.com/TNB88/SkPlayer/refs/heads/main/SmartKaraokePlayerPRO_v3.57.apk
```

Neu so dau bang hoac nho hon app dang cai thi app se khong bao update.
Neu so dau lon hon app dang cai thi app se hien thong bao tai ban moi.

## Luu y

- Khong doi ten `version.txt` va `version_rtd.txt`, vi APK da gan cung 2 ten nay.
- Link APK nen la raw GitHub hoac link tai truc tiep ket thuc bang `.apk`.
- Neu chi co 1 ban APK, co the de `version.txt` va `version_rtd.txt` giong nhau.
- Ban fix cung `versionCode=416` se khong tu hien thong bao update tren may da cai ban 416. Neu may con popup ma kich hoat cu, hay cai tay APK moi trong repo mot lan.
- Ban hien tai doc anh nen tu repo `TNB88/photo_karaoke`: `1.jpg`, `2.jpg`, `3.jpg`, `4.jpg`.
- Anh nen doi moi khoang 15 giay sau khi anh truoc load xong.
- Ban hien tai: `SmartKaraokePlayerPRO_v3.56_newkey_bgok_v13_github_photo_15s_exitfix.apk`.
