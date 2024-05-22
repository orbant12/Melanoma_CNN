# Skin Cancer Binary Classification( Malignant or Bening ) 

## 1.) Dataset
### Collected Images from isic cli - Shared on my google drive
https://drive.google.com/drive/folders/1RdlCSJl6IwPfvVNwzX6PDbz1KCXHwysM?usp=sharing

![download](https://github.com/orbant12/Melanoma_CNN/assets/124793231/0231e8d1-3819-4bd6-b26a-f8c2afa18b50)
![download (1)](https://github.com/orbant12/Melanoma_CNN/assets/124793231/05478550-40ca-4fbb-b948-0aa267aaa8ee)
![download (2)](https://github.com/orbant12/Melanoma_CNN/assets/124793231/81c84d53-4336-4332-aba5-24c7346592d8)

---

## 2.) Simple Image Decoding
<code>def decode_image(filepath, label):
    img = tf.io.read_file(filepath)
    img = tf.image.decode_jpeg(img)
    img = tf.image.resize(img, [224, 224])
    img = tf.cast(img, tf.float32) / 255.0
    return img, label</code>

---

## 3.) Model Architecture

![Screenshot 2024-05-22 at 17 24 32](https://github.com/orbant12/Melanoma_CNN/assets/124793231/c80aa69d-4379-4b55-b96e-853d9bac2222)


---

## 4.) Results
### Loss
![download (3)](https://github.com/orbant12/Melanoma_CNN/assets/124793231/1b28e47d-81a2-4f6b-8849-cbeceec71901)

### Accuracy - 0.92
![download (4)](https://github.com/orbant12/Melanoma_CNN/assets/124793231/88a5d3c5-381d-40ba-9b6b-d17a5b41b4f3)
