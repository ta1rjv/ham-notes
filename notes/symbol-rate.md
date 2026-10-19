# Sembol hızı, bant genişliği ve bit hızı

## Kapladığı bant genişliği

```
BW ≈ SR × (1 + α)
```

`SR` sembol hızı (sembol/s), `α` roll-off (DVB-S2: 0,35 / 0,25 / 0,20).

| SR | α = 0,35 | α = 0,25 | α = 0,20 |
|---|---|---|---|
| 333 kS/s | 450 kHz | 416 kHz | 400 kHz |
| 1 MS/s | 1,35 MHz | 1,25 MHz | 1,20 MHz |
| 2 MS/s | 2,70 MHz | 2,50 MHz | 2,40 MHz |

## Yaklaşık faydalı bit hızı

```
R ≈ SR × log2(M) × kod oranı × η
```

`M` takımyıldız büyüklüğü (QPSK = 4, 8PSK = 8), `η` çerçeve, BCH ve pilot
ek yükü için düzeltme (DVB-S2'de tipik olarak 0,95–0,99).

Örnek: 1 MS/s, QPSK 2/3 → 1 × 2 × 0,667 × ≈0,98 ≈ **1,3 Mbit/s** TS.
