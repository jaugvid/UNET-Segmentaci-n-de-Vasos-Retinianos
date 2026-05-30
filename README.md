# Segmentación de Vasos Retinianos para Detección de Retinopatía Diabética usando U-Net

Este proyecto implementa una arquitectura U-Net personalizada en PyTorch para segmentación binaria de vasos retinianos en imágenes de fondo de ojo. El modelo se entrena sobre DRIVE y se evalúa tanto en DRIVE como en CHASE_DB1 para analizar la degradación por cambio de dominio. Además, se incluye una estrategia de mitigación basada en Test-Time Augmentation y una mejora de dominio externo mediante CLAHE.

## 1. Requisitos

El proyecto fue desarrollado en Python 3.10 o superior.

Dependencias principales:

- PyTorch
- torchvision
- NumPy
- pandas
- matplotlib
- scikit-learn
- scipy
- OpenCV
- Pillow
- tqdm
- Jupyter
- nbconvert

## 2. Instalación del entorno

Se recomienda crear un entorno virtual.

### Opción A: usando venv

```bash
python -m venv .venv
source .venv/bin/activate
pip install --upgrade pip
pip install -r requirements.txt

## 3. Ejecución

jupyter nbconvert --to notebook --execute UNet_Segmentacion_Vasos_Retinianos_PyTorchv6.ipynb --ExecutePreprocessor.timeout=-1 --output UNet_Segmentacion_Vasos_Retinianos_PyTorchv6_ejecutado.ipynb
