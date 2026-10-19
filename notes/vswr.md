# VSWR, yansıma katsayısı ve dönüş kaybı

```
|Γ| = (VSWR − 1) / (VSWR + 1)
Dönüş kaybı RL (dB) = −20·log10(|Γ|)
Uyumsuzluk kaybı ML (dB) = −10·log10(1 − |Γ|²)
Yansıyan güç oranı = |Γ|²
```

| VSWR | \|Γ\| | RL | Yansıyan güç | ML |
|---|---|---|---|---|
| 1,1 | 0,048 | 26,4 dB | %0,2 | 0,01 dB |
| 1,5 | 0,200 | 14,0 dB | %4,0 | 0,18 dB |
| 2,0 | 0,333 | 9,5 dB | %11,1 | 0,51 dB |
| 3,0 | 0,500 | 6,0 dB | %25,0 | 1,25 dB |

Ölçüm notu: Uzun ve kayıplı kabloda verici ucunda ölçülen VSWR, anten ucundakinden
daha iyi görünür (kablo kaybı yansımayı iki kez zayıflatır).

## Anten kazancı birimleri

```
dBi = dBd + 2,15
```
