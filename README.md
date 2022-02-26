# XPT2046
## 接線

| Raspberri Pi  | <--> | XPT2046 |
| :------------ |:---------------:| -----:|
| SCLK_1 (GPIO21) | <--> | CLK |
| CS_1 (GPIO7) | <--> | CS |
| MOSI_1 (GPIO20) | <--> | DIN |
| MISO_1 (GPIO19) | <--> | DO |
| GPIO26 | <--> | IRQ |

```
sudo nano /boot/config.txt
```
### 增加下面指令
```
dtoverlay=spi1-3cs
```

### 重新開機

## Reference：[XPT2046-Python](https://github.com/Luca8991/XPT2046-Python)



