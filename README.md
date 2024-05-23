To repozytorium zawiera wynik pracy nad pracą inżynierską "Biometryczna analiza podobieństwa śladów daktyloskopijnych opuszka boczno-górnego palca" zawiera wytrenowane modele architektury YOLOv5 wyspecjalizowane w wyszukiwaniu następujacych cech odcisików palców:
- rozwidlenia,
- zakończenia,
- odcinki,
- mostki,
- pory,

Do pustego projektu google colab należy wkleić i uruchomić w następującej kolejności:

## Skopiuj to repozytorium
```
!git clone https://github.com/skrzemien/yolov5-fingerprints
```

## Skopiuj repozytorium razem z wymaganymi bibliotekami
```
!git clone https://github.com/ultralytics/yolov5
%cd yolov5
%pip install -qr requirements.txt
%pip install -q roboflow

import torch
import os
from IPython.display import Image, clear_output

print('Setup complete. Using torch %s %s' % (torch.__version__, torch.cuda.get_device_properties(0) if torch.cuda.is_available() else 'CPU'))
```
