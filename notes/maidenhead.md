# Maidenhead lokatörü

Dünya, boylam ve enlem için iç içe ızgaralara bölünür. Boylam 180 eklenerek,
enlem 90 eklenerek pozitif hale getirilir.

| Seviye | Karakter | Boylam adımı | Enlem adımı |
|---|---|---|---|
| Alan (field) | A–R | 20° | 10° |
| Kare (square) | 0–9 | 2° | 1° |
| Alt kare (subsquare) | a–x | 5′ | 2,5′ |

## Hesap

```
lon' = lon + 180      lat' = lat + 90
1. harf = A + floor(lon' / 20)
2. harf = A + floor(lat' / 10)
3. rakam = floor((lon' mod 20) / 2)
4. rakam = floor(lat' mod 10)
5. harf = a + floor((lon' mod 2) * 12)
6. harf = a + floor((lat' mod 1) * 24)
```

## Örnekler

| Yer | Konum | Lokatör (4 hane) |
|---|---|---|
| İstanbul | 41,01 K, 28,98 D | KN41 |
| Ankara | 39,93 K, 32,85 D | KM69 |
