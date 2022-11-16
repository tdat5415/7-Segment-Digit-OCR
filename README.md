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

---

### Epoch-Loss Figure

![epoch_loss](https://user-images.githubusercontent.com/48349693/202092727-e00c3c61-bd46-4aa6-866e-adaa97b72d1b.jpg)

---

### Prediction Plot

![savef_plt](https://user-images.githubusercontent.com/48349693/202092779-28bd50eb-4d40-4603-9eef-6e6543984305.jpg)





