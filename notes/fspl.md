# Serbest uzay yol kaybı (FSPL)

```
FSPL (dB) = 20·log10(d_km) + 20·log10(f_MHz) + 32,44
```

## Örnekler

| Bağlantı | Mesafe | Frekans | FSPL |
|---|---|---|---|
| QO-100 uplink | 36 000 km | 2400 MHz | ≈ 191,2 dB |
| QO-100 downlink | 36 000 km | 10 489 MHz | ≈ 204,0 dB |
| 2 m yer bağlantısı | 100 km | 145 MHz | ≈ 115,7 dB |
| 23 cm yer bağlantısı | 50 km | 1296 MHz | ≈ 128,7 dB |

## Basit bağlantı bütçesi

```
Alınan güç (dBm) = Pt (dBm) + Gt (dBi) − Lt (dB) − FSPL + Gr (dBi) − Lr (dB)
```

Hatırlatma: `dBm = dBW + 30`, `1 W = 30 dBm`, `100 W = 50 dBm`.
