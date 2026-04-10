## Technical Design
* **Model**: YOLOv8 Nano (optimized for edge deployment).
* **Dataset**: 1,300 images (80% Train, 20% Val).
* **Resolution**: 512x512 pixels.
* **Epochs**: 25.

## Results
The model successfully identifies crops and weeds to enable targeted pesticide application, reducing chemical waste and ensuring food safety.

## How to use
```python
from ultralytics import YOLO
model = YOLO('best.pt')
results = model.predict('your_image.jpg')
