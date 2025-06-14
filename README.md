# Chat with Capri

AI assistant packaged with love.


### Capri in Action

[![Capri in Action](https://img.youtube.com/vi/9fVhCuODB-Y/maxresdefault.jpg)](https://www.youtube.com/watch?v=9fVhCuODB-Y)


### Code Overview

[![Code Overview](https://img.youtube.com/vi/CvIQZK1HIvY/maxresdefault.jpg)](https://www.youtube.com/watch?v=CvIQZK1HIvY)



# Get started

> python3 -m venv venv

> source venv/bin/activate

> pip3 install -r requirements.txt

> python3 capri.py


## Generate the .dmg file (MacOS)

> pyinstaller --onefile --windowed capri.py

> mkdir -p Capri.app/Contents/MacOS/

> mkdir -p Capri.app/Contents/Resources/

> cp -f dist/capri Capri.app/Contents/MacOS/Capri

> hdiutil create -volname "Capri" -srcfolder Capri.app -ov -format UDZO Capri-1.0.dmg

### One liner

> pyinstaller --onefile --windowed capri.py && hdiutil create -volname "Capri" -srcfolder Capri.app -ov -format UDZO Capri-1.0.dmg


## Generate the .deb file (Linux)

> pyinstaller --onefile --windowed capri.py

> mkdir -p capri-1.0/usr/local/bin/

> cp -f dist/capri capri-1.0/usr/local/bin/Capri

> dpkg-deb --build capri-1.0



### One liner:
> pyinstaller --onefile --windowed capri.py && mkdir -p capri-1.0/usr/local/bin/ && cp -f dist/capri capri-1.0/usr/local/bin/Capri && dpkg-deb --build capri-1.0



## Install (Linux)

> Install: capri-1.0.deb by double clicking on it.

> Uninstall: sudo apt remove capri 
