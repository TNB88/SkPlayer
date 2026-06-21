# Codex Notes - Smart Karaoke Player PRO

Ghi chu nay de lan sau mo Codex tren may khac van biet APK da sua nhung gi.

## Ban dang dung

- APK on dinh hien tai: `SmartKaraokePlayerPRO_v3.56_newkey_bgok_v14_github_photo_10x30s_nolatest.apk`
- Version trong APK: `versionCode=416`, `versionName=3.56`
- File update app doc:
  - `version.txt`
  - `version_rtd.txt`
- Link update hien tai dang tro ve ban v14:
  - `https://raw.githubusercontent.com/TNB88/SkPlayer/refs/heads/main/SmartKaraokePlayerPRO_v3.56_newkey_bgok_v14_github_photo_10x30s_nolatest.apk`

## Nhung viec da sua

1. Gan he thong kich hoat moi
   - Thay luong key/cu phan trial cu bang luong nhap ma kich hoat moi.
   - Ma hop le duoc kiem tra qua server/Worker rieng.
   - Khi ma hop le, app luu trang thai kich hoat den ngay het han.
   - Khong ghi ma kich hoat that vao repo public.

2. Don sach key/trial cu
   - Muc tieu la go cac cho con nhac "con X ngay het han" va popup kich hoat cu.
   - Neu may da cai ban cu va van bi nho du lieu cu, can cai ban `noold` moi hoac xoa data app mot lan.

3. Sua update online qua GitHub
   - App duoc patch de doc update tu repo `TNB88/SkPlayer`.
   - Hai file `version.txt` va `version_rtd.txt` co dinh dang:
     ```txt
     versionCode;versionName;apkUrl
     ```
   - Vi du hien tai:
     ```txt
     416;3.56;https://raw.githubusercontent.com/TNB88/SkPlayer/refs/heads/main/SmartKaraokePlayerPRO_v3.56_newkey_bgok_v2_noold_v9.apk
     ```

4. Sua loi background bai hat
   - Mot so ban patch truoc vao duoc app nhung background bi dung o nen "Smart Karaoke Player".
   - Ban v9 da test lai tren Android box `192.168.1.23`.
   - Ket qua test: background hien anh bai hat va tu doi anh sau khoang 25 giay.

5. Doi nen online qua GitHub
   - Ban v13 doc anh nen tu repo `TNB88/photo_karaoke`.
   - Ban v14 doc 10 file anh: `1.jpg` den `10.jpg`.
   - De doi anh sau nay, chi can thay file trong repo anh va giu dung ten file.
   - Da bo nhay anh MP3/local luc app moi mo.
   - Timer doi anh ban v14 dat 30 giay sau khi anh truoc load xong.
   - Vong anh chay theo thu tu `1 -> 10`, het `10` thi quay lai `1`.
   - Nut `Dong y` trong hop thoai thoat app da sua de thoat ve launcher.
   - Ban v14 an dong "phien ban moi nhat" tren man hinh mo app de tranh hien sai `3.56(2)`.

## Cach ra ban moi sau nay

1. Sua/build APK moi.
2. Dat ten file ro rang, vi du:
   ```txt
   SmartKaraokePlayerPRO_v3.56_newkey_bgok_v2_noold_v10.apk
   ```
3. Copy APK moi vao repo `SkPlayer`.
4. Sua ca hai file:
   - `version.txt`
   - `version_rtd.txt`
5. Neu muon app tu bao co update tren may da cai ban 416, phai tang `versionCode` len lon hon 416.
   - Vi du:
     ```txt
     417;3.57;https://raw.githubusercontent.com/TNB88/SkPlayer/refs/heads/main/SmartKaraokePlayerPRO_v3.57.apk
     ```
6. Commit va push len GitHub.
7. Test raw link tra `200 OK`.

## Lenh test hay dung

Kiem tra raw version:

```powershell
Invoke-WebRequest -UseBasicParsing https://raw.githubusercontent.com/TNB88/SkPlayer/refs/heads/main/version.txt
Invoke-WebRequest -UseBasicParsing https://raw.githubusercontent.com/TNB88/SkPlayer/refs/heads/main/version_rtd.txt
```

Ket noi box test:

```powershell
C:\Android\Sdk\platform-tools\adb.exe connect 192.168.1.23:5555
C:\Android\Sdk\platform-tools\adb.exe -s 192.168.1.23:5555 install -r -d .\SmartKaraokePlayerPRO_v3.56_newkey_bgok_v14_github_photo_10x30s_nolatest.apk
```

Chup man hinh test background:

```powershell
C:\Android\Sdk\platform-tools\adb.exe -s 192.168.1.23:5555 shell screencap -p /sdcard/sk_screen.png
C:\Android\Sdk\platform-tools\adb.exe -s 192.168.1.23:5555 pull /sdcard/sk_screen.png .
```

## Luu y

- `versionCode=416` giong ban cu nen may da cai 416 co the khong tu hien thong bao update.
- Truong hop do, cai tay APK moi tu raw link GitHub.
- Khong dua ma kich hoat that, token, mat khau hoac thong tin rieng vao repo public.
