# ar9331-i2s-alsa
I2S alsa device drivers for the popular MIPS ar9331 SOC (Carambola2, Arduino Yun...)

It is implemented as a openwrt package and can be compiled with Linux Kernel Ver. 3.14.xx.

cd ~/Chaos_Calme/package/kernel

git clone https://github.com/sonnyyu/ar9331-i2s-alsa.git

cd ~/Chaos_Calme/

make menuconfig

PACKAGE_kmod-ath79-pcm

PACKAGE_kmod-ath79-i2s

PACKAGE_kmod-ath79-i2s-dev

PACKAGE_kmod-ath79-wm8727

PACKAGE_kmod-ath79-carambola2

make sure above module select.

make  -j 5  V=s 

