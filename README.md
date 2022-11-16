# 7-Segment-Digit-OCR
Red 7 segment digit OCR.

---

### Install

```
git clone https://github.com/tdat97/7-Segment-Digit-OCR.git
cd 7-Segment-Digit-OCR
pip install -r requirments.txt
```

---

### Example

```python
from utils.ocr import OcrEngine
import matplotlib.pyplot as plt
```

```python
img = plt.imread("./temp/test_digit.jpg")
plt.imshow(img)
```

![test_digit](https://user-images.githubusercontent.com/48349693/202092183-00ac7c3f-cdd3-4df2-83d4-194dfbf0d0b2.jpg)

```python
ocr_engine = OcrEngine("./models/7seg_ocr.h5")
print(ocr_engine(img)) # '267'
```
