
# Proyecto de Detección de Fechas de Expiración

Este repositorio contiene dos modelos de machine learning para la detección de fechas de expiración en productos:

1. **YOLOv5**: Un modelo de detección de objetos que se utiliza para localizar las cajas que contienen las fechas de expiración en las imágenes.
2. **OCR (Reconocimiento Óptico de Caracteres)**: Un modelo que extrae el texto de las cajas detectadas por YOLOv5 para identificar las fechas de expiración.

## Estructura del Repositorio

- **`data/`**: Contiene el dataset utilizado para entrenar el modelo OCR. Este conjunto de datos incluye imágenes con las fechas de expiración que el modelo OCR debe reconocer.
- **`dataset/`**: Contiene el dataset utilizado para entrenar el modelo YOLOv5, que está diseñado para detectar las cajas de las fechas de expiración en las imágenes.
- **`modelos/`**: Contiene el archivo `yolov5.pt`, que es el archivo de pesos del modelo YOLOv5 entrenado para detectar las cajas de fechas de expiración.
  
## Requisitos

Este proyecto requiere Python 3.11 y las siguientes dependencias, que se pueden instalar utilizando el archivo `requirements.txt`.

### Instalación
La versión recomendada de Python para este proyecto es Python 3.11.
1. Clona este repositorio en tu máquina local:
   ```bash
   git clone https://github.com/JuanMolina2001/ml-labels
   ```

2. Navega al directorio del proyecto:
   ```bash
   cd ml-labels
   ```

3. Crea un entorno virtual (opcional pero recomendado):
   ```bash
   python -m virtualenv venv
   ```

4. Activa el entorno virtual:
   - En Windows:
     ```bash
     venv\Scripts\activate
     ```
   - En macOS/Linux:
     ```bash
     source venv/bin/activate
     ```

5. Instala las dependencias:
   ```bash
   pip install -r requirements.txt
   ```
