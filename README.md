# Flipper Zero — Xal'Morak

Хувийн Flipper Zero төхөөрлөлт:
- Төхөөрийн **хувийн нэр**: `Xal'Morak`
- **Дэлгэцийн анимаци** (нэр харуулсан idle screen)

Репо: https://github.com/XalMorak/flipper-zero-xalmorak

## 1. Төхөөрийн нэр солих

Flipper дээр:

1. **Settings → Desktop → Name** (эсвэл **Settings → System → Device Name** — firmware-ээс шалтгаана)
2. Нэрийг **`Xal'Morak`** болго
3. Passport дээр харах: Desktop дээр **RIGHT** дарах

`name/device_name.txt` дотор хадгалалтыг байна.

Bluetooth / USB дээр төхөөр **Xal'Morak** гэж харагдана.

## 2. Дэлгэцийн анимац суулгах

### Official / Unleashed / RogueMaster (энгийн SD `dolphin`)

1. `sd/dolphin/XalMorak_128x64/` хавтасыг Flipper-ийн SD дээрхий **`/ext/dolphin/`** руу хуулна.
2. `sd/dolphin/manifest.txt` доторх мөрүү мөрүү оршин файлын төгсгөөд нэмэх, эсвэл одоогийн `manifest.txt` дээр дараах блокыг **нэмж** оруулна:

```
Name: XalMorak_128x64
Min butthurt: 0
Max butthurt: 14
Min level: 1
Max level: 3
Weight: 8
```

3. Flipper-ийг **reboot**.

### Momentum / CFW asset pack

`sd/asset_packs/XalMorak/` хавтасыг SD-ийн **`/ext/asset_packs/XalMorak/`** руу хуулна. Settings дээр asset pack-ийг сонгоно.

## 3. Файлын бүтэц

```
name/device_name.txt          ← төхөөрийн нэр
sd/dolphin/XalMorak_128x64/   ← дэлгэцийн код (meta + frames)
sd/dolphin/manifest.txt
sd/asset_packs/XalMorak/
```

`meta.txt` бол дэлгэц хэрээн зурах код. `frame_0.png` … нэгээд харуулсан зураг.  
SD дээр шууд ажиллахын тулд `.png`-ийг `.bm` руу хөрвүүлнэ (энгийнсэн CFW эсвэл Flipper Animation Tool).

## Анхаар

Энэ пак зөвхөн хувийн нэр + idle дэлгэц. Exploit / payload байхгүй.
