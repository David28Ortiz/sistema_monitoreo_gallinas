# 🐔 Sistema de Monitoreo de Gallinas Ponedoras con Visión por Computadora

Este repositorio contiene el código fuente desarrollado para la tesis de grado titulada:

**"Sistema de monitoreo de gallinas ponedoras en la avícola 'El Triunfo' empleando redes neuronales profundas y visión por computadora"**

El sistema permite detectar y realizar seguimiento a gallinas en tiempo real utilizando modelos de detección como YOLO y seguimiento con algoritmos como ByteTrack.

# 🚀 Características implementadas

- Detección de gallinas en tiempo real
- Seguimiento de gallinas en tiempo real
- Conteo de gallinas
- Estimación de distancia recorrida y velocidad promedio por ave
- Visualización de resultados en video

# ⬇️Descarga de datos y modelo

Los archivos necesarios para entrenar y ejecutar el modelo están disponibles en Google Drive:

- 📁 [Carpeta con imágenes y etiquetas de 'train' y 'validation'](https://drive.google.com/file/d/1NRtM8FcAs_PjqvKGq4yR_r2_MWIJihgO/view?usp=drive_link)
- 📁 [Carpeta con imágenes y etiquetas de 'test'](https://drive.google.com/file/d/1KWgP9ra1Yayzjv5DUDaFv0tEj75a9yYh/view?usp=drive_link)
- 🧠 [Modelo entrenado (best.pt)](https://drive.google.com/file/d/1XIeJ2GTzas29GmC-lJwOyC-2xG-ytjGR/view?usp=drive_link)

### 🔧 Rutas que debes modificar

Asegúrate de actualizar las siguientes rutas de acceso en el archivo `main.ipynb` para que coincidan con tu estructura de carpetas en Google Drive:

📁 Carpetas de entrenamiento

- Imágenes de entrenamiento:
```python
train_folder = "/content/drive/MyDrive/Colab Notebooks/yolov8_tracking/yolov8_detection/hen_detection_dataset/train/images"
```
- Etiquetas de entrenamiento:
```python
label_folder = "/content/drive/MyDrive/Colab Notebooks/yolov8_tracking/yolov8_detection/hen_detection_dataset/train/labels"
```
📄 Configuración de data.yaml

- Actualiza el archivo `data.yaml` con sus respectivas rutas, junto con la siguiente línea de código:
```python
data = '/content/drive/MyDrive/Colab Notebooks/yolov8_tracking/yolov8_detection/data.yaml'
```
🖼️ Ruta de imágenes para test
```python
test_images_path = "/content/drive/MyDrive/Colab Notebooks/yolov8_tracking/yolov8_detection/test/images"
```
🧠 Modelo entrenado

- Ruta al modelo `best.pt`:
```python
model = YOLO("/content/drive/MyDrive/Colab Notebooks/yolov8_tracking/yolov8_detection/runs_model_x/weights/best.pt")
```

# 🎥 Demostraciones en video

A continuación, se presentan los resultados del sistema sobre diferentes cantidades de gallinas en ambiente real:

- 📹 Detección y seguimiento de 50 gallinas: https://youtube.com/shorts/FI7_R7hWhdk 
- 📹 Detección y seguimiento de 80 gallinas: https://youtu.be/198yBQseVfI 
- 📹 Detección y seguimiento de 90 gallinas: https://youtu.be/Xzh41JTrRmU
- 📹 Detección y seguimiento de 100 gallinas: https://youtu.be/OC4l9Vk5_OQ 
- 📹 Detección y seguimiento de 110 gallinas: https://youtube.com/shorts/xEZIuK2FKAw

# 🧠 Modelos utilizados

- [Grounding DINO](https://github.com/IDEA-Research/GroundingDINO)
- [YOLO](https://arxiv.org/abs/2310.01641)
- [YOLOv11 - Ultralytics](https://docs.ultralytics.com/es/models/yolo11/) 
- [ByteTrack](https://arxiv.org/abs/2110.06864)

# 📝 Autores
David Santiago Ortiz Ramos - Marcos Stevan Canchón Villamil

Estudiantes de Ingeniería Electrónica

Universidad Surcolombiana

# 📄 Licencia

Este proyecto se distribuye con fines académicos. Verifica las licencias de cada modelo en sus respectivos repositorios oficiales.
