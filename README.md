# GoodFitLCDshow35onRaspbian64

How to make GoodFit LCD-show 3.5 work on Raspbian 64

git clone https://github.com/goodtft/LCD-show.git

chmod -R 755 LCD-show

cd LCD-show

sudo ./LCD35-show

sudo nano /boot/firmware/cmdline.txt

# Move your cursor to the very end of the line, add a single space, and type :

fbcon=map:10 fbcon=font:VGA8x8

# ctrl+x and save

sudo cp ~/LCD-show/usr/tft35a-overlay.dtb /boot/firmware/overlays/tft35a.dtbo


