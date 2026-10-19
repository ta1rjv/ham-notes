# ADALM-Pluto hızlı notlar

| Özellik | Değer |
|---|---|
| RF çip | AD9363 |
| Resmi frekans aralığı | 325 – 3800 MHz |
| Resmi anlık bant genişliği | 20 MHz |
| ADC/DAC | 12 bit |
| Varsayılan IP (USB ağ) | 192.168.2.1 |
| Varsayılan SSH kullanıcısı | `root` / `analog` |

## AD9364 kapsamını açma (70 – 6000 MHz, 56 MHz)

Garanti dışıdır; çip AD9363 olarak test edilmiştir, kenar frekanslarda
performans düşer.

```sh
fw_setenv attr_name compatible
fw_setenv attr_val ad9364
reboot
```

## Kontrol

```sh
iio_info -u ip:192.168.2.1 | grep -i ad936
```
