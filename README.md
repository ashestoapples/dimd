# dimd - v0.1
# Duplicate IMage Detector

Qt5 GUI fronted visually similar image finder with sqlite  database support. The current supported image formats are PNG, JPG, JPEG, and BMP. Both Windows and Linux compatible.

The hashing algorithm is based off of this article: http://blog.iconfinder.com/detecting-duplicate-images-using-python/

I figured I'd make something usefull for myself (and hopefully others) with it. 

# Screenshots
![alt tag](http://i.imgur.com/HdEPvQU.png)
![alt tag](http://i.imgur.com/vphiTh4.png)

# Dependencies
pillow -- python 3 imaging library

sqlite3

pyqt5

Windows binaries can be found easily on the internet.

For linux just use your package manager for pyqt5 and sqlite3. PILLOW can be obtained from the AUR for arch users.

# TODO:
Preferred directories
Autoselect by size
