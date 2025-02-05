```python
!pip install ultralytics
```

```
Collecting ultralytics
  Downloading ultralytics-8.3.29-py3-none-any.whl.metadata (35 kB)
Requirement already satisfied: numpy>=1.23.0 in /usr/local/lib/python3.10/dist-packages (from ultralytics) (1.26.4)
Requirement already satisfied: matplotlib>=3.3.0 in /usr/local/lib/python3.10/dist-packages (from ultralytics) (3.8.0)
Requirement already satisfied: opencv-python>=4.6.0 in /usr/local/lib/python3.10/dist-packages (from ultralytics) (4.10.0.84)
Requirement already satisfied: pillow>=7.1.2 in /usr/local/lib/python3.10/dist-packages (from ultralytics) (10.4.0)
Requirement already satisfied: pyyaml>=5.3.1 in /usr/local/lib/python3.10/dist-packages (from ultralytics) (6.0.2)
Requirement already satisfied: requests>=2.23.0 in /usr/local/lib/python3.10/dist-packages (from ultralytics) (2.32.3)
Requirement already satisfied: scipy>=1.4.1 in /usr/local/lib/python3.10/dist-packages (from ultralytics) (1.13.1)
Requirement already satisfied: torch>=1.8.0 in /usr/local/lib/python3.10/dist-packages (from ultralytics) (2.5.0+cu121)
Requirement already satisfied: torchvision>=0.9.0 in /usr/local/lib/python3.10/dist-packages (from ultralytics) (0.20.0+cu121)
Requirement already satisfied: tqdm>=4.64.0 in /usr/local/lib/python3.10/dist-packages (from ultralytics) (4.66.6)
Requirement already satisfied: psutil in /usr/local/lib/python3.10/dist-packages (from ultralytics) (5.9.5)
Requirement already satisfied: py-cpuinfo in /usr/local/lib/python3.10/dist-packages (from ultralytics) (9.0.0)
Requirement already satisfied: pandas>=1.1.4 in /usr/local/lib/python3.10/dist-packages (from ultralytics) (2.2.2)
Requirement already satisfied: seaborn>=0.11.0 in /usr/local/lib/python3.10/dist-packages (from ultralytics) (0.13.2)
Collecting ultralytics-thop>=2.0.0 (from ultralytics)
  Downloading ultralytics_thop-2.0.11-py3-none-any.whl.metadata (9.4 kB)
Requirement already satisfied: contourpy>=1.0.1 in /usr/local/lib/python3.10/dist-packages (from matplotlib>=3.3.0->ultralytics) (1.3.0)
Requirement already satisfied: cycler>=0.10 in /usr/local/lib/python3.10/dist-packages (from matplotlib>=3.3.0->ultralytics) (0.12.1)
Requirement already satisfied: fonttools>=4.22.0 in /usr/local/lib/python3.10/dist-packages (from matplotlib>=3.3.0->ultralytics) (4.54.1)
Requirement already satisfied: kiwisolver>=1.0.1 in /usr/local/lib/python3.10/dist-packages (from matplotlib>=3.3.0->ultralytics) (1.4.7)
Requirement already satisfied: packaging>=20.0 in /usr/local/lib/python3.10/dist-packages (from matplotlib>=3.3.0->ultralytics) (24.1)
Requirement already satisfied: pyparsing>=2.3.1 in /usr/local/lib/python3.10/dist-packages (from matplotlib>=3.3.0->ultralytics) (3.2.0)
Requirement already satisfied: python-dateutil>=2.7 in /usr/local/lib/python3.10/dist-packages (from matplotlib>=3.3.0->ultralytics) (2.8.2)
Requirement already satisfied: pytz>=2020.1 in /usr/local/lib/python3.10/dist-packages (from pandas>=1.1.4->ultralytics) (2024.2)
Requirement already satisfied: tzdata>=2022.7 in /usr/local/lib/python3.10/dist-packages (from pandas>=1.1.4->ultralytics) (2024.2)
Requirement already satisfied: charset-normalizer<4,>=2 in /usr/local/lib/python3.10/dist-packages (from requests>=2.23.0->ultralytics) (3.4.0)
Requirement already satisfied: idna<4,>=2.5 in /usr/local/lib/python3.10/dist-packages (from requests>=2.23.0->ultralytics) (3.10)
Requirement already satisfied: urllib3<3,>=1.21.1 in /usr/local/lib/python3.10/dist-packages (from requests>=2.23.0->ultralytics) (2.2.3)
Requirement already satisfied: certifi>=2017.4.17 in /usr/local/lib/python3.10/dist-packages (from requests>=2.23.0->ultralytics) (2024.8.30)
Requirement already satisfied: filelock in /usr/local/lib/python3.10/dist-packages (from torch>=1.8.0->ultralytics) (3.16.1)
Requirement already satisfied: typing-extensions>=4.8.0 in /usr/local/lib/python3.10/dist-packages (from torch>=1.8.0->ultralytics) (4.12.2)
Requirement already satisfied: networkx in /usr/local/lib/python3.10/dist-packages (from torch>=1.8.0->ultralytics) (3.4.2)
Requirement already satisfied: jinja2 in /usr/local/lib/python3.10/dist-packages (from torch>=1.8.0->ultralytics) (3.1.4)
Requirement already satisfied: fsspec in /usr/local/lib/python3.10/dist-packages (from torch>=1.8.0->ultralytics) (2024.10.0)
Requirement already satisfied: sympy==1.13.1 in /usr/local/lib/python3.10/dist-packages (from torch>=1.8.0->ultralytics) (1.13.1)
Requirement already satisfied: mpmath<1.4,>=1.1.0 in /usr/local/lib/python3.10/dist-packages (from sympy==1.13.1->torch>=1.8.0->ultralytics) (1.3.0)
Requirement already satisfied: six>=1.5 in /usr/local/lib/python3.10/dist-packages (from python-dateutil>=2.7->matplotlib>=3.3.0->ultralytics) (1.16.0)
Requirement already satisfied: MarkupSafe>=2.0 in /usr/local/lib/python3.10/dist-packages (from jinja2->torch>=1.8.0->ultralytics) (3.0.2)
Downloading ultralytics-8.3.29-py3-none-any.whl (883 kB)
[2K   [90m━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━[0m [32m883.8/883.8 kB[0m [31m21.2 MB/s[0m eta [36m0:00:00[0m
[?25hDownloading ultralytics_thop-2.0.11-py3-none-any.whl (26 kB)
Installing collected packages: ultralytics-thop, ultralytics
Successfully installed ultralytics-8.3.29 ultralytics-thop-2.0.11

```

```python
# Disable warnings in the notebook to maintain clean output cells
import warnings
warnings.filterwarnings('ignore')

# Import necessary libraries
import os
import shutil
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
import random
import cv2
import yaml
from PIL import Image
from collections import deque
from ultralytics import YOLO
from IPython.display import Video
```

```
Creating new Ultralytics Settings v0.0.6 file ✅ 
View Ultralytics Settings with 'yolo settings' or at '/root/.config/Ultralytics/settings.json'
Update Settings with 'yolo settings key=value', i.e. 'yolo settings runs_dir=path/to/dir'. For help see https://docs.ultralytics.com/quickstart/#ultralytics-settings.

```

```python
# Configure the visual appearance of Seaborn plots
sns.set(rc={'axes.facecolor': '#ffe4de'}, style='darkgrid')
```

Step2

```python
# Load the pre-trained YOLOv8 nano segmentation model
model = YOLO('yolov8n-seg.pt')
```

**LOADING THE DATASET TO GOOGLE DRIVE**

```python
from google.colab import drive
import os

drive.mount('/content/drive')

# Define the path in Google Drive where you want to save the dataset
dataset_drive_path = '/content/drive/MyDrive/pothole_detection_dataset'
# drive.mount(dataset_drive_path)

# Step 2: Create the destination folder if it doesn't exist
import os
if not os.path.exists(dataset_drive_path):
    os.makedirs(dataset_drive_path)  # Create the directory if it doesn't exist

# Step 3: Install and use Roboflow to download the dataset if the directory is empty
if not os.listdir(dataset_drive_path):  # Check if folder is empty
    !pip install roboflow
    from roboflow import Roboflow
    rf = Roboflow(api_key="2KxikbypwSdgdSQ570S0")
    project = rf.workspace("farzad").project("pothole_segmentation_yolov8")
    version = project.version(1)

    # Download the dataset and specify the directory in Google Drive as the destination
    dataset = version.download("tensorflow", location=dataset_drive_path)
    print("Dataset downloaded and saved to Google Drive.")
else:
    print("Dataset already exists in Google Drive. Skipping download.")

# Step 4: Verify and list files to ensure the dataset was saved
dataset_path = dataset_drive_path
print("Dataset path:", dataset_path)

# List all files in the dataset directory to confirm successful download
print("Files in dataset directory:", os.listdir(dataset_path))

# If no files appear, check if the downloaded data is saved under nested directories
for root, dirs, files in os.walk(dataset_drive_path):
    for name in files:
        print(os.path.join(root, name))

```

```
Mounted at /content/drive
Collecting roboflow
  Downloading roboflow-1.1.49-py3-none-any.whl.metadata (9.7 kB)
Requirement already satisfied: certifi in /usr/local/lib/python3.10/dist-packages (from roboflow) (2024.8.30)
Collecting idna==3.7 (from roboflow)
  Downloading idna-3.7-py3-none-any.whl.metadata (9.9 kB)
Requirement already satisfied: cycler in /usr/local/lib/python3.10/dist-packages (from roboflow) (0.12.1)
Requirement already satisfied: kiwisolver>=1.3.1 in /usr/local/lib/python3.10/dist-packages (from roboflow) (1.4.7)
Requirement already satisfied: matplotlib in /usr/local/lib/python3.10/dist-packages (from roboflow) (3.8.0)
Requirement already satisfied: numpy>=1.18.5 in /usr/local/lib/python3.10/dist-packages (from roboflow) (1.26.4)
Requirement already satisfied: opencv-python-headless==4.10.0.84 in /usr/local/lib/python3.10/dist-packages (from roboflow) (4.10.0.84)
Requirement already satisfied: Pillow>=7.1.2 in /usr/local/lib/python3.10/dist-packages (from roboflow) (10.4.0)
Requirement already satisfied: python-dateutil in /usr/local/lib/python3.10/dist-packages (from roboflow) (2.8.2)
Collecting python-dotenv (from roboflow)
  Downloading python_dotenv-1.0.1-py3-none-any.whl.metadata (23 kB)
Requirement already satisfied: requests in /usr/local/lib/python3.10/dist-packages (from roboflow) (2.32.3)
Requirement already satisfied: six in /usr/local/lib/python3.10/dist-packages (from roboflow) (1.16.0)
Requirement already satisfied: urllib3>=1.26.6 in /usr/local/lib/python3.10/dist-packages (from roboflow) (2.2.3)
Requirement already satisfied: tqdm>=4.41.0 in /usr/local/lib/python3.10/dist-packages (from roboflow) (4.66.6)
Requirement already satisfied: PyYAML>=5.3.1 in /usr/local/lib/python3.10/dist-packages (from roboflow) (6.0.2)
Requirement already satisfied: requests-toolbelt in /usr/local/lib/python3.10/dist-packages (from roboflow) (1.0.0)
Collecting filetype (from roboflow)
  Downloading filetype-1.2.0-py2.py3-none-any.whl.metadata (6.5 kB)
Requirement already satisfied: contourpy>=1.0.1 in /usr/local/lib/python3.10/dist-packages (from matplotlib->roboflow) (1.3.0)
Requirement already satisfied: fonttools>=4.22.0 in /usr/local/lib/python3.10/dist-packages (from matplotlib->roboflow) (4.54.1)
Requirement already satisfied: packaging>=20.0 in /usr/local/lib/python3.10/dist-packages (from matplotlib->roboflow) (24.1)
Requirement already satisfied: pyparsing>=2.3.1 in /usr/local/lib/python3.10/dist-packages (from matplotlib->roboflow) (3.2.0)
Requirement already satisfied: charset-normalizer<4,>=2 in /usr/local/lib/python3.10/dist-packages (from requests->roboflow) (3.4.0)
Downloading roboflow-1.1.49-py3-none-any.whl (80 kB)
[2K   [90m━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━[0m [32m80.9/80.9 kB[0m [31m5.2 MB/s[0m eta [36m0:00:00[0m
[?25hDownloading idna-3.7-py3-none-any.whl (66 kB)
[2K   [90m━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━[0m [32m66.8/66.8 kB[0m [31m2.7 MB/s[0m eta [36m0:00:00[0m
[?25hDownloading filetype-1.2.0-py2.py3-none-any.whl (19 kB)
Downloading python_dotenv-1.0.1-py3-none-any.whl (19 kB)
Installing collected packages: filetype, python-dotenv, idna, roboflow
  Attempting uninstall: idna
    Found existing installation: idna 3.10
    Uninstalling idna-3.10:
      Successfully uninstalled idna-3.10
Successfully installed filetype-1.2.0 idna-3.7 python-dotenv-1.0.1 roboflow-1.1.49
loading Roboflow workspace...
loading Roboflow project...
Dataset downloaded and saved to Google Drive.
Dataset path: /content/drive/MyDrive/pothole_detection_dataset
Files in dataset directory: []

```

```python
from google.colab import drive
drive.mount('/content/drive')
```

```
Mounted at /content/drive

```

```python
!pip install roboflow
from roboflow import Roboflow
rf = Roboflow(api_key="2KxikbypwSdgdSQ570S0")
project = rf.workspace("farzad").project("pothole_segmentation_yolov8")
version = project.version(1)
dataset = version.download("tensorflow")
```

```
Requirement already satisfied: roboflow in /usr/local/lib/python3.10/dist-packages (1.1.49)
Requirement already satisfied: certifi in /usr/local/lib/python3.10/dist-packages (from roboflow) (2024.8.30)
Requirement already satisfied: idna==3.7 in /usr/local/lib/python3.10/dist-packages (from roboflow) (3.7)
Requirement already satisfied: cycler in /usr/local/lib/python3.10/dist-packages (from roboflow) (0.12.1)
Requirement already satisfied: kiwisolver>=1.3.1 in /usr/local/lib/python3.10/dist-packages (from roboflow) (1.4.7)
Requirement already satisfied: matplotlib in /usr/local/lib/python3.10/dist-packages (from roboflow) (3.8.0)
Requirement already satisfied: numpy>=1.18.5 in /usr/local/lib/python3.10/dist-packages (from roboflow) (1.26.4)
Requirement already satisfied: opencv-python-headless==4.10.0.84 in /usr/local/lib/python3.10/dist-packages (from roboflow) (4.10.0.84)
Requirement already satisfied: Pillow>=7.1.2 in /usr/local/lib/python3.10/dist-packages (from roboflow) (10.4.0)
Requirement already satisfied: python-dateutil in /usr/local/lib/python3.10/dist-packages (from roboflow) (2.8.2)
Requirement already satisfied: python-dotenv in /usr/local/lib/python3.10/dist-packages (from roboflow) (1.0.1)
Requirement already satisfied: requests in /usr/local/lib/python3.10/dist-packages (from roboflow) (2.32.3)
Requirement already satisfied: six in /usr/local/lib/python3.10/dist-packages (from roboflow) (1.16.0)
Requirement already satisfied: urllib3>=1.26.6 in /usr/local/lib/python3.10/dist-packages (from roboflow) (2.2.3)
Requirement already satisfied: tqdm>=4.41.0 in /usr/local/lib/python3.10/dist-packages (from roboflow) (4.66.6)
Requirement already satisfied: PyYAML>=5.3.1 in /usr/local/lib/python3.10/dist-packages (from roboflow) (6.0.2)
Requirement already satisfied: requests-toolbelt in /usr/local/lib/python3.10/dist-packages (from roboflow) (1.0.0)
Requirement already satisfied: filetype in /usr/local/lib/python3.10/dist-packages (from roboflow) (1.2.0)
Requirement already satisfied: contourpy>=1.0.1 in /usr/local/lib/python3.10/dist-packages (from matplotlib->roboflow) (1.3.0)
Requirement already satisfied: fonttools>=4.22.0 in /usr/local/lib/python3.10/dist-packages (from matplotlib->roboflow) (4.54.1)
Requirement already satisfied: packaging>=20.0 in /usr/local/lib/python3.10/dist-packages (from matplotlib->roboflow) (24.1)
Requirement already satisfied: pyparsing>=2.3.1 in /usr/local/lib/python3.10/dist-packages (from matplotlib->roboflow) (3.2.0)
Requirement already satisfied: charset-normalizer<4,>=2 in /usr/local/lib/python3.10/dist-packages (from requests->roboflow) (3.4.0)
loading Roboflow workspace...
loading Roboflow project...

```

```
Downloading Dataset Version Zip in Pothole_Segmentation_YOLOv8-1 to tensorflow:: 100%|██████████| 54436/54436 [00:02<00:00, 21976.06it/s]
```

```


```

```

Extracting Dataset Version Zip to Pothole_Segmentation_YOLOv8-1 in tensorflow:: 100%|██████████| 786/786 [00:00<00:00, 4031.47it/s]

```

```python
import shutil

# Define source and destination paths
source_path = '/content/Pothole_Segmentation_YOLOv8-1'
destination_path = '/content/drive/MyDrive/pothole_detection_dataset/MyDrive'

# Move the folder from source to destination
shutil.move(source_path, destination_path)
print(f"Folder moved from {source_path} to {destination_path}")


```

```
Folder moved from /content/Pothole_Segmentation_YOLOv8-1 to /content/drive/MyDrive/pothole_detection_dataset/MyDrive

```

**MOVING TRAINING IMAGES TO IMAGES FOLDER**

```python
import os
import shutil

# Define paths for the dataset
source_images_dir = '/content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/train'  # Original folder with images
destination_images_dir = '/content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/train/images'  # New folder to move images

# Ensure the destination directory exists
os.makedirs(destination_images_dir, exist_ok=True)

# List all the files in the source directory
all_files = os.listdir(source_images_dir)

# Move the image files
for file_name in all_files:
    # Only move image files (optional: check for image extensions like .jpg, .png)
    if file_name.lower().endswith(('.png', '.jpg', '.jpeg', '.bmp', '.tiff')):
        # Define full file paths
        source_path = os.path.join(source_images_dir, file_name)
        destination_path = os.path.join(destination_images_dir, file_name)

        # Ensure the file exists before moving
        if os.path.exists(source_path):
            shutil.move(source_path, destination_path)
            print(f"Moved: {file_name}")
        else:
            print(f"File {file_name} not found in {source_images_dir}")

print("All images have been moved successfully.")
```

```
Moved: pic-300-_jpg.rf.84ff02582ef46f86d24bc848af4be07b.jpg
Moved: pic-9-_jpg.rf.10d9db0c8fac4eb5b01de9fc71dd19da.jpg
Moved: pic-122-_jpg.rf.727dc87f7e5fb44ce14cf3878f669aa7.jpg
Moved: pic-182-_jpg.rf.0689172bca1eeb50732cceb0a2d2dbc7.jpg
Moved: pic-23-_jpg.rf.4152b4c3ac522f79019ca14cc242eb95.jpg
Moved: pic-141-_jpg.rf.fc3d1df38a5c4e68febeb45b2a132f4a.jpg
Moved: pic-181-_jpg.rf.d2e46218aa9286f174c99c772f1c1758.jpg
Moved: pic-4-_jpg.rf.f52085b2d1744eeb56ed5a4b8ba0fb0f.jpg
Moved: pic-210-_jpg.rf.7d87d7b5337a40b2c80ce816e643376a.jpg
Moved: pic-54-_jpg.rf.7cc54c3290a15bece4443e1f76a5800c.jpg
Moved: pic-86-_jpg.rf.6ba43a8fea8b523c5647b5148ccc4c48.jpg
Moved: pic-134-_jpg.rf.517c7c3c07571b10697a58b567940b58.jpg
Moved: pic-218-_jpg.rf.d9c8cdd8aea8314208624edb692b09cb.jpg
Moved: pic-81-_jpg.rf.682981671ea574a72479e1763164f07b.jpg
Moved: pic-182-_jpg.rf.236dc9bd798d6f8c56dbfdc5754e3b68.jpg
Moved: pic-274-_jpg.rf.ce4479c25a7c7d6c8b8d001c488a4f6d.jpg
Moved: pic-90-_jpg.rf.240ef6f5fe43b76b41bda46a16cb5718.jpg
Moved: pic-188-_jpg.rf.dcd45e3458a07cec9ba93918315d2eaf.jpg
Moved: pic-39-_jpg.rf.c50896cfc9b1facb5cd4234bb9be07b6.jpg
Moved: pic-237-_jpg.rf.f81c589abb7f7593acd9a66bd74c5d7f.jpg
Moved: pic-15-_jpg.rf.5331a19ad3f6b2b37894ae4f0072cea0.jpg
Moved: pic-153-_jpg.rf.c2e6d6e3806754b1713a36a954367a60.jpg
Moved: pic-19-_jpg.rf.8ec9e835434bab69526356b80fb94588.jpg
Moved: pic-275-_jpg.rf.cd2ef0884568491ec2ce61a16f085324.jpg
Moved: pic-146-_jpg.rf.05122d9316fa0be439f878d8aa337d3d.jpg
Moved: pic-249-_jpg.rf.6184619642f841a8598f0fee9f9cb770.jpg
Moved: pic-147-_jpg.rf.890438ae2f4d1bb94198abdd6c181ec8.jpg
Moved: pic-199-_jpg.rf.08d902c95a9a00f33f6a031a3ce86eaf.jpg
Moved: pic-98-_jpg.rf.87c1a2590b120c4cb812f9702e6bc851.jpg
Moved: pic-286-_jpg.rf.e2281030be53c236e0e2f7731df0f5b3.jpg
Moved: pic-242-_jpg.rf.42f875819ed5ac0facfa51b46a123fc2.jpg
Moved: pic-286-_jpg.rf.51113a90d61bab00d4fe0edcd5e45d9b.jpg
Moved: pic-258-_jpg.rf.5dc1fecc0c1bd209ca05c88618583504.jpg
Moved: pic-207-_jpg.rf.b4c0b6220ddb190aee07dfd59ffd4277.jpg
Moved: pic-276-_jpg.rf.85ffbef727ecf81dbdc795cf0071fde4.jpg
Moved: pic-108-_jpg.rf.0a11aa9e03c7bce050328b7bb2341bad.jpg
Moved: pic-224-_jpg.rf.bd5f146daa5ac308b6b501d1c6f1d33d.jpg
Moved: pic-109-_jpg.rf.04274b3be06ee972e8900a1875f45611.jpg
Moved: pic-283-_jpg.rf.e5da98374205a9ad95cb1355a5d30d9a.jpg
Moved: pic-64-_jpg.rf.2c59f391b25c97761914413f17802e9d.jpg
Moved: pic-107-_jpg.rf.3553f8919ce95633136ebe837864a734.jpg
Moved: pic-16-_jpg.rf.0d031ce3c207297977b4c60a77d278da.jpg
Moved: pic-93-_jpg.rf.d1fd0f49bc38e1f7395f550a40ffda27.jpg
Moved: pic-227-_jpg.rf.d1dd38a0e09eda8c0d4239a5bdedd0d5.jpg
Moved: pic-47-_jpg.rf.e7a3996bac750b9ba88cc570c1aad418.jpg
Moved: pic-294-_jpg.rf.03cbcc554416b49037040fba4614781a.jpg
Moved: pic-226-_jpg.rf.14efc266ef488a27f59064a50d804ca0.jpg
Moved: pic-68-_jpg.rf.23e729ce0e5380e419377888f247b0ec.jpg
Moved: pic-158-_jpg.rf.bb32e2985b2c29e77029a0452ab20bac.jpg
Moved: pic-180-_jpg.rf.edbdd29c7a063d66218221470a7e44f5.jpg
Moved: pic-210-_jpg.rf.d00f21d9a21dd0244263a64b8bda2348.jpg
Moved: pic-246-_jpg.rf.93663c16c298ed591b91eadfc6e144ae.jpg
Moved: pic-174-_jpg.rf.5ec8f9ecd96971def7f6e5074c5e0373.jpg
Moved: pic-104-_jpg.rf.117ec7cfcc77d6e6f80130934b1d5aa1.jpg
Moved: pic-293-_jpg.rf.152a3d1b716ce34ef95d003bf13d19e3.jpg
Moved: pic-141-_jpg.rf.dc5bb23e947044e6c4a4572abc3e8213.jpg
Moved: pic-57-_jpg.rf.7d1b62f97cac4df979e6f394117d04d1.jpg
Moved: pic-5-_jpg.rf.ead443dd9f37ce2e29069e9049d804e7.jpg
Moved: pic-145-_jpg.rf.01b4f283d7eaa74981edcc0259ef43cb.jpg
Moved: pic-38-_jpg.rf.dba8be87e1cad6fbbc6f68728f95a85d.jpg
Moved: pic-134-_jpg.rf.e15dd6f2f2bc285d64fef68fb2d92164.jpg
Moved: pic-101-_jpg.rf.4abe48a3d2a5e556908bf4286446e5ce.jpg
Moved: pic-47-_jpg.rf.07110750200ea396e69160ea5e20ce7c.jpg
Moved: pic-231-_jpg.rf.2f5901a40332f282bcafe34b90f4f5ec.jpg
Moved: pic-150-_jpg.rf.0f181e46348e6b83b3a218d5ea72eef2.jpg
Moved: pic-59-_jpg.rf.d3fc5f4680f6e28784c2f686b25736bd.jpg
Moved: pic-29-_jpg.rf.56803c885d93883808e18e5177fb7bfc.jpg
Moved: pic-82-_jpg.rf.96fb5070300f4d0838ba9d84df193cb3.jpg
Moved: pic-247-_jpg.rf.0f4643d64aafaa72e5e291cb8bdfae57.jpg
Moved: pic-32-_jpg.rf.e9cd27fe43663beff58ee6e1f8f7f3d2.jpg
Moved: pic-196-_jpg.rf.812d218445763c3ed203a0f9458291f9.jpg
Moved: pic-166-_jpg.rf.33cf824f2784fd32a3bb22c67f3fdabc.jpg
Moved: pic-76-_jpg.rf.72e4e540e160870c4756c500e80e40b1.jpg
Moved: pic-214-_jpg.rf.74655743f4f3d67bb2e21be9727a7946.jpg
Moved: pic-219-_jpg.rf.9f723a6b8ef272c7a5899faf7f892aee.jpg
Moved: pic-8-_jpg.rf.22de640e2560bddb13ff49abfccbc8d6.jpg
Moved: pic-217-_jpg.rf.de0280b56ab0a3f21fab3b5986a16080.jpg
Moved: pic-194-_jpg.rf.0e60f4ceb45a85c359677ee01c088045.jpg
Moved: pic-232-_jpg.rf.1494a9c164c52d1cd9b45dda0e1b5bab.jpg
Moved: pic-240-_jpg.rf.8dee3d4ab5ccd2161b6e520c20a0f812.jpg
Moved: pic-295-_jpg.rf.d32464e992476781dea9e98988a24869.jpg
Moved: pic-118-_jpg.rf.aa2953e739d235b2eddafdea4a1dab6e.jpg
Moved: pic-12-_jpg.rf.f538915b42230d73cd5e22bcb4b06ce6.jpg
Moved: pic-12-_jpg.rf.3145a5860685e71bb38756743d8c5132.jpg
Moved: pic-146-_jpg.rf.18a3fc9b3f915028b7246fba6b56fd11.jpg
Moved: pic-32-_jpg.rf.4aea4d06478697bd7b70b72cd80d1546.jpg
Moved: pic-66-_jpg.rf.2d3138a80a414a75ab0117408153227b.jpg
Moved: pic-244-_jpg.rf.7ebc863c89590ff2a83f607dcbc68e34.jpg
Moved: pic-21-_jpg.rf.b341c07e4c85101f52a39109ebb299b0.jpg
Moved: pic-41-_jpg.rf.5e808c2edeb8c3db416e41b5cf956575.jpg
Moved: pic-38-_jpg.rf.da02919be110cad52f54add553bf8ff6.jpg
Moved: pic-77-_jpg.rf.61a63f92522c3558c8dc33ecae183ed2.jpg
Moved: pic-147-_jpg.rf.0f296124b79e86f38cda27b6fe05d742.jpg
Moved: pic-83-_jpg.rf.6067035f09c5b1b4a82debfac50b8b68.jpg
Moved: pic-9-_jpg.rf.06f81aab8edc8a1beb3269f379c8e4a8.jpg
Moved: pic-279-_jpg.rf.aeb00c47b3179ead074b8f7b52971655.jpg
Moved: pic-176-_jpg.rf.8d87b09b011bb4b479cea2d472354334.jpg
Moved: pic-247-_jpg.rf.cbf21b0811a22af9d7b2ebaffbd1d938.jpg
Moved: pic-196-_jpg.rf.7ea9f287f872540f14495fae6d91e4e6.jpg
Moved: pic-260-_jpg.rf.76bee172574bbacef55e6935f031bf20.jpg
Moved: pic-215-_jpg.rf.ff49694bdd544a47be71713dc6c46593.jpg
Moved: pic-255-_jpg.rf.5b8acd3a5f571d5d7e245e1f950b92cc.jpg
Moved: pic-124-_jpg.rf.5e69150b156446dbd25a1ba55e83d665.jpg
Moved: pic-180-_jpg.rf.544e62b6d885e8e5cc375189b6c13233.jpg
Moved: pic-100-_jpg.rf.ebc3af260e989e6f9e1e9221b9dff6b0.jpg
Moved: pic-92-_jpg.rf.f3247194c884aec0a806958acbda7b38.jpg
Moved: pic-143-_jpg.rf.eab223bbca50b3ff5899899213a6292d.jpg
Moved: pic-212-_jpg.rf.e36dc9e60b7e977f6e7d2d1a323b9c73.jpg
Moved: pic-75-_jpg.rf.01e2ff81bb8754692afe9b2bb2fda48a.jpg
Moved: pic-124-_jpg.rf.e75e7815306ccb81e78d7f8b63857483.jpg
Moved: pic-63-_jpg.rf.75d85a055ab217101c1e32000dd5826b.jpg
Moved: pic-298-_jpg.rf.eb89bc0d42a73c41261305e01a9138f8.jpg
Moved: pic-56-_jpg.rf.41ab69bbd0dab6a5f9693448b7cf2cd1.jpg
Moved: pic-179-_jpg.rf.ca0b41b2475176a03280e24fc5d3da7b.jpg
Moved: pic-282-_jpg.rf.0dbe6d0d6778748a85926379c5f2e9e2.jpg
Moved: pic-199-_jpg.rf.cedbf41ae88b4faa6ca4e3f9907c9678.jpg
Moved: pic-14-_jpg.rf.5795a6265ed32db2ca7965aa7e0174b1.jpg
Moved: pic-278-_jpg.rf.161161ebb6d47b347f2c6012b1c88898.jpg
Moved: pic-162-_jpg.rf.69c191909f6cc1a946105b08efab6224.jpg
Moved: pic-62-_jpg.rf.7863aa2444a65c631e8af7c5b9ac8edb.jpg
Moved: pic-87-_jpg.rf.071c1cfadf7d9959341091d7c27f0caa.jpg
Moved: pic-218-_jpg.rf.1becdc6413b7b22fdf55ade9f266316e.jpg
Moved: pic-82-_jpg.rf.cdb1fbbb88686147ca6fd7393e9a1053.jpg
Moved: pic-86-_jpg.rf.fe15af9f424efc111e4bab1ead9b76cc.jpg
Moved: pic-48-_jpg.rf.68853a3577e0a03df1d073ae0713d353.jpg
Moved: pic-198-_jpg.rf.4a69d95662fb642c674f26ff0ef0a5a9.jpg
Moved: pic-43-_jpg.rf.dfa9d788bc69cea17fc9c3308d1668a7.jpg
Moved: pic-207-_jpg.rf.4facc206ce5e1fac516bd765c34f7972.jpg
Moved: pic-29-_jpg.rf.5220d64d0af700ca8a131e4a7015591a.jpg
Moved: pic-128-_jpg.rf.0ac3472d1668a73f904ec562bcfc43ff.jpg
Moved: pic-15-_jpg.rf.390f967469ceb20da60cbb99af7e2c16.jpg
Moved: pic-163-_jpg.rf.2677c0fd3f9bec65c04ee82b7d8a000a.jpg
Moved: pic-238-_jpg.rf.73b9192a4cd0112e00efe9158aff9459.jpg
Moved: pic-55-_jpg.rf.d55ddba83fd6401d17e234092ab2a378.jpg
Moved: pic-83-_jpg.rf.8d1e38d4c07d51717c500ae1145d7108.jpg
Moved: pic-296-_jpg.rf.4842e778156eb9f2ba5cf237fe3e4a62.jpg
Moved: pic-250-_jpg.rf.fa08a66eed53518165efed59a5ab8eb4.jpg
Moved: pic-268-_jpg.rf.c49fc76803dd19f43665c0ced1377750.jpg
Moved: pic-121-_jpg.rf.6550c19d889288f83dca4f4c57545348.jpg
Moved: pic-195-_jpg.rf.66e723938cac897ced6246535fe9da8a.jpg
Moved: pic-186-_jpg.rf.6df069fb0a914f27571234fbc1aa446b.jpg
Moved: pic-63-_jpg.rf.f4fd8956206d712c6b9964dfbfe1567e.jpg
Moved: pic-117-_jpg.rf.8e6e071e8f8e9e9d6f84a1f35766ebf0.jpg
Moved: pic-246-_jpg.rf.554ed8a1140e2e47539b5825358f3491.jpg
Moved: pic-113-_jpg.rf.59ab5bd4ba9f0202cd15f82e7109fc77.jpg
Moved: pic-223-_jpg.rf.04b3324ec3044431090e8b9359b88bf7.jpg
Moved: pic-318-_jpg.rf.2940a75b7dd32070029f18fa382ebdc5.jpg
Moved: pic-167-_jpg.rf.307e87780d9f502b50e422c4a80d38c9.jpg
Moved: pic-208-_jpg.rf.2a110ddd516f4ba59951afbf405d42a5.jpg
Moved: pic-245-_jpg.rf.17df77133740bc613a4696554928cd5c.jpg
Moved: pic-182-_jpg.rf.4b148a54550e9eeccfacda80024037b1.jpg
Moved: pic-143-_jpg.rf.216b82e37fe7bf7ace28e129f406915c.jpg
Moved: pic-148-_jpg.rf.5a781d389cff26a6e2ee08ce9b0498e7.jpg
Moved: pic-235-_jpg.rf.c953bfbb7502053e8a904197dc52e925.jpg
Moved: pic-156-_jpg.rf.3b94cd14bdbf92f4cd57497def72b167.jpg
Moved: pic-211-_jpg.rf.4eb10110d12e7623cb7be8caf4f66c5a.jpg
Moved: pic-108-_jpg.rf.1dee3ebe35fda326931fb1a1a3162f56.jpg
Moved: pic-137-_jpg.rf.eec8497f7279810ff44902d6eca0121b.jpg
Moved: pic-181-_jpg.rf.4c915083eb98e45fee4d4f707f89406a.jpg
Moved: pic-185-_jpg.rf.b060d919f03803a454f2c92fb25e51ec.jpg
Moved: pic-289-_jpg.rf.948fb2d38ed70096fb1c644ab1e89973.jpg
Moved: pic-282-_jpg.rf.f00b26bc9e0e6d37dfc28fb9dcca8d31.jpg
Moved: pic-108-_jpg.rf.539074c8d5134b846ed4b34e66362766.jpg
Moved: pic-158-_jpg.rf.21962dcea10b8f2209ae3fdb9797b6c6.jpg
Moved: pic-245-_jpg.rf.9e660e4d87ccc3b8a3bb1d2bf2745aa8.jpg
Moved: pic-135-_jpg.rf.9cee00f51ec30b4e0f591b2da2007a10.jpg
Moved: pic-282-_jpg.rf.842cdce727f91b17dbe3c3da0eb40f53.jpg
Moved: pic-195-_jpg.rf.0bbee8fd461407d8eded3b0ea8e80b4c.jpg
Moved: pic-255-_jpg.rf.93cf2350f3e2eb8b0e28c90904582e06.jpg
Moved: pic-221-_jpg.rf.a2e98283cbb1e83a8af07620af2cb3d6.jpg
Moved: pic-74-_jpg.rf.4599969de001cd1935d28ed812d1dd90.jpg
Moved: pic-84-_jpg.rf.79ea02211ed732335af4650b0977b9ad.jpg
Moved: pic-119-_jpg.rf.efb59ea51e49ee98c39fcda52e3b6389.jpg
Moved: pic-190-_jpg.rf.531db54959dd774f8f60dee6d86da08e.jpg
Moved: pic-37-_jpg.rf.fef279db67c02cffe5e03d2f062e76c7.jpg
Moved: pic-103-_jpg.rf.26017e20e92320bcde575710389353b1.jpg
Moved: pic-231-_jpg.rf.15d03eb1f1aea5ae78f46547ddb947b5.jpg
Moved: pic-237-_jpg.rf.b4c9d0f7d582f53d9355532af217097e.jpg
Moved: pic-78-_jpg.rf.a51a0e1d7624e72d7257934cefd3d410.jpg
Moved: pic-71-_jpg.rf.dd6b8e67c19a5c53bb6f91b55e593a13.jpg
Moved: pic-80-_jpg.rf.8988aa50fb872401bc29ab7830281e22.jpg
Moved: pic-222-_jpg.rf.159340ca71da523b0e2a61122f85d352.jpg
Moved: pic-150-_jpg.rf.e47d187e86dd6eb504660921449a7883.jpg
Moved: pic-170-_jpg.rf.f6e9c0883eac1443308f4f424ae60db4.jpg
Moved: pic-179-_jpg.rf.ff0320a37ee1d098eb9aed6036758287.jpg
Moved: pic-166-_jpg.rf.2f4d36fff66d603c99b22043abc562ba.jpg
Moved: pic-26-_jpg.rf.50fba6db0c31398bb0ad36b22f1cf88f.jpg
Moved: pic-287-_jpg.rf.9ebbae06b203eacb7891199e3ae03e78.jpg
Moved: pic-124-_jpg.rf.5f9ee27d0fe8571af0685b1746b9d7fc.jpg
Moved: pic-215-_jpg.rf.40ad961da5aeef8f6c97d772ee2b618e.jpg
Moved: pic-280-_jpg.rf.44efc10266e3c4cb78efde437755b21f.jpg
Moved: pic-279-_jpg.rf.387d558e33ac4c0afd2b684708d66271.jpg
Moved: pic-106-_jpg.rf.ac62ec1fab28b4344978edf35e9d2f3b.jpg
Moved: pic-153-_jpg.rf.61b165d52cdeea1e1a674f2e8e3912d5.jpg
Moved: pic-186-_jpg.rf.124fb81faf74b03398e066e6d7cbc9eb.jpg
Moved: pic-1-_jpg.rf.49882cdb272111f43a6656b1494a4918.jpg
Moved: pic-80-_jpg.rf.e5fc6c140371201fb051fc7100769b0b.jpg
Moved: pic-301-_jpg.rf.b5aea8cb48e0a04950551fd41e277ea6.jpg
Moved: pic-222-_jpg.rf.a5ea9340a3f317eab9bc842a8d252835.jpg
Moved: pic-239-_jpg.rf.755180833958d9091b3bb6a24b34f8c9.jpg
Moved: pic-227-_jpg.rf.e6fd78cbf2dc3c11a24ccdc8ddc5ee25.jpg
Moved: pic-167-_jpg.rf.5d211f0e20e55adab672af34f9df1940.jpg
Moved: pic-289-_jpg.rf.b0bf8384c5c25bbefa58c5f1e0893b5d.jpg
Moved: pic-97-_jpg.rf.405aad85024f81d93922f28864ca1554.jpg
Moved: pic-127-_jpg.rf.4aebae9cb49eac155acea198eb8d4649.jpg
Moved: pic-96-_jpg.rf.de1c39ae1a6f184297eac1814e66ca80.jpg
Moved: pic-18-_jpg.rf.146c5b1af3190071c88676c409c4dad1.jpg
Moved: pic-223-_jpg.rf.9d3f63dd5136bc8b5e16b4fdf3e5b5e7.jpg
Moved: pic-177-_jpg.rf.4b35b04139ea1742026f65aa3e2730fe.jpg
Moved: pic-126-_jpg.rf.4d5c28bfd2ec83debd1fa97e86bbddb4.jpg
Moved: pic-136-_jpg.rf.28112df3106c2b4485053cd6371a47ef.jpg
Moved: pic-34-_jpg.rf.3cc5232b879d313c05dc30ad7b066f99.jpg
Moved: pic-241-_jpg.rf.8288a409c841a344ed2174080fddc6a5.jpg
Moved: pic-44-_jpg.rf.a71dc55407736290b223f5ac71e8f714.jpg
Moved: pic-94-_jpg.rf.385cffc613c080827eaa7d1176be5ae3.jpg
Moved: pic-127-_jpg.rf.513297c58b670dfbcee0c02f22a76c9f.jpg
Moved: pic-121-_jpg.rf.ca379af880817bcbc914bac8fd00d7e6.jpg
Moved: pic-112-_jpg.rf.3d443fe242b14e97a21264faecffde8c.jpg
Moved: pic-297-_jpg.rf.84f5afae7a869cf8e987823d48ac52ea.jpg
Moved: pic-9-_jpg.rf.62204b022d0e43f1804769f4fc142c28.jpg
Moved: pic-98-_jpg.rf.b2a2cf125087b692dbc9ea11ae97ddd4.jpg
Moved: pic-293-_jpg.rf.a9b5278454dd0e6b846f8f5b345c8c0a.jpg
Moved: pic-41-_jpg.rf.74ff92157ffacab71cc6f120cb5663a6.jpg
Moved: pic-280-_jpg.rf.1cfd00374439fd72effee65dee2cfbf3.jpg
Moved: pic-118-_jpg.rf.8beeeda1ce5f8d0cf75e8634f45e6e7e.jpg
Moved: pic-277-_jpg.rf.e2e29a600dcb8450df911104cf88b38d.jpg
Moved: pic-70-_jpg.rf.4bee9afd2a93c4eec1a251f641521c4c.jpg
Moved: pic-272-_jpg.rf.002253fdb0ed4584e018df6ffa261117.jpg
Moved: pic-166-_jpg.rf.77f1227905045ad65f8fda0d6427dbe5.jpg
Moved: pic-14-_jpg.rf.3e2f11367531d04d10e9132cf6fe9b8f.jpg
Moved: pic-164-_jpg.rf.31facecf28467c64106a888177c293c4.jpg
Moved: pic-284-_jpg.rf.684fdc990a5a35d7a5d296857475e65d.jpg
Moved: pic-233-_jpg.rf.64732a7585f4f1dc942fda7dce11b947.jpg
Moved: pic-92-_jpg.rf.453e3b0d19f45cc3adda8b6c2fd35f78.jpg
Moved: pic-174-_jpg.rf.2f427bf4f80837fb0387c3ee0c38e172.jpg
Moved: pic-63-_jpg.rf.81a9ac78e24a93573acdd933a0dd3b2a.jpg
Moved: pic-89-_jpg.rf.280b8654e1d942e9843333a4a630a473.jpg
Moved: pic-169-_jpg.rf.ab0a07cd761c2739c0051926b50b0593.jpg
Moved: pic-10-_jpg.rf.1d433d21e11d000b6b498eacb88fe4a9.jpg
Moved: pic-160-_jpg.rf.acf7ae50b1e59b9e6e4bbf150e8055a9.jpg
Moved: pic-296-_jpg.rf.71c7e5d6a9c5da8e4043d68da5539b8e.jpg
Moved: pic-256-_jpg.rf.aa2fce633443ee1d8c81896a8ea32dae.jpg
Moved: pic-54-_jpg.rf.a5904fe5b078b76264e6bf4b9a026627.jpg
Moved: pic-4-_jpg.rf.d3357165b543f6d3e0f729dfa3373855.jpg
Moved: pic-285-_jpg.rf.2bdafbee1a88e6d2a7fdf3367073e72e.jpg
Moved: pic-25-_jpg.rf.deadb4c9f8357cd2f7d51f91cb1da866.jpg
Moved: pic-256-_jpg.rf.7019bcfb7ed85d62a0068bb4d90894d6.jpg
Moved: pic-276-_jpg.rf.8d4273fdb3b241213a5685129666cde6.jpg
Moved: pic-243-_jpg.rf.d864bfac7ff1440f8c98557209aa3c0f.jpg
Moved: pic-176-_jpg.rf.24dea194a3e0e25703a25e481c89dc9c.jpg
Moved: pic-128-_jpg.rf.145c4607840c2bcac86b2f76c28a7750.jpg
Moved: pic-258-_jpg.rf.fcdd3609bc1d58a34086a5a3e6ce2097.jpg
Moved: pic-242-_jpg.rf.0a72277f1c31da47eb26ecbb3b7e6296.jpg
Moved: pic-19-_jpg.rf.3427acf9ec34ef05f6fe4a10e7280478.jpg
Moved: pic-19-_jpg.rf.5b617b77a960e3e18ff122c7c17a3a90.jpg
Moved: pic-301-_jpg.rf.2b21a6093d6fa16efa900074dc3542cd.jpg
Moved: pic-128-_jpg.rf.e9d874018c8eb5296749630aca5603e6.jpg
Moved: pic-26-_jpg.rf.9be8ea96b8bb643747babec0e006e3a8.jpg
Moved: pic-117-_jpg.rf.23537a5a480ec24a62b83163a80c4db3.jpg
Moved: pic-82-_jpg.rf.24e5bbbd60206e18fc16880bfeaad9aa.jpg
Moved: pic-206-_jpg.rf.4213f6cdf3dee589a56e5aad14500784.jpg
Moved: pic-272-_jpg.rf.0a7c7409d5dc54a17f739f3fcc1dfbfb.jpg
Moved: pic-177-_jpg.rf.86d64524dfd317ff89ce31ff39a3fa83.jpg
Moved: pic-57-_jpg.rf.935c3e2cd37b84d8f63043ca26ebb402.jpg
Moved: pic-252-_jpg.rf.1d994545861b8acd262681fa0d99058b.jpg
Moved: pic-203-_jpg.rf.8dd21e07b004f7c29a8d4f97e0a3283b.jpg
Moved: pic-148-_jpg.rf.e2bb2aecbf0577a45e672425acfed876.jpg
Moved: pic-93-_jpg.rf.7a97c10314fb3e87620c30001a1ebda8.jpg
Moved: pic-51-_jpg.rf.38b94f88de5e174741f7f535773d0c40.jpg
Moved: pic-32-_jpg.rf.17b7362dd7e828ab11f01d0a23db3a50.jpg
Moved: pic-37-_jpg.rf.dbb4e5f29da50d7f69800bd02df7cd28.jpg
Moved: pic-295-_jpg.rf.f66059d5449c804a491dfe941e69a338.jpg
Moved: pic-115-_jpg.rf.1da712be935af009c0a9e04f0276f225.jpg
Moved: pic-6-_jpg.rf.cbd6e701a750684661efc0363bd607aa.jpg
Moved: pic-18-_jpg.rf.42022b7bc105da3fc5d269c32db8dbcf.jpg
Moved: pic-84-_jpg.rf.875df442d5750a19dce18e532e06b8fe.jpg
Moved: pic-29-_jpg.rf.75b74368c26af7be08174514a5e86a35.jpg
Moved: pic-35-_jpg.rf.e87935b40ac72eeef1e183a1b784e3e9.jpg
Moved: pic-186-_jpg.rf.6dfa17e72f379782ec0b743ba60b8543.jpg
Moved: pic-51-_jpg.rf.f708e8dd61e5d6c7f0417a6e7befa47d.jpg
Moved: pic-68-_jpg.rf.6d010af44edfa998adc338038f167ac6.jpg
Moved: pic-2-_jpg.rf.1db425f6267df87504430ef5a0e23709.jpg
Moved: pic-104-_jpg.rf.f986cb78d75fc164de95ac33c56d9474.jpg
Moved: pic-226-_jpg.rf.a751fa82eb82745f4b5f94656b4d1455.jpg
Moved: pic-240-_jpg.rf.8f0271d2f7004b60ecb8bceed3c799c6.jpg
Moved: pic-248-_jpg.rf.a889a66f2a2a27646c6d2102e5b2fb17.jpg
Moved: pic-188-_jpg.rf.892956f0dc513250fbe68acd8c8b91e1.jpg
Moved: pic-35-_jpg.rf.3a6cb54980b1b14196158b140c277034.jpg
Moved: pic-84-_jpg.rf.f2555c00b7ca574dd2f6b119f2849651.jpg
Moved: pic-268-_jpg.rf.323d61640ba6fcc13042b787260e36bb.jpg
Moved: pic-208-_jpg.rf.a7d61ad38189d19f47b2407d4c2455fb.jpg
Moved: pic-235-_jpg.rf.149b89f603991e65409d2c817ffa8def.jpg
Moved: pic-86-_jpg.rf.c7c369033df047926786fd0bbc131cf5.jpg
Moved: pic-43-_jpg.rf.1e8c9b6d903b795ead837d1334fbe4ff.jpg
Moved: pic-179-_jpg.rf.c4a7f4f1cff2653d7d2fbc85d91bddca.jpg
Moved: pic-252-_jpg.rf.60c38b7dd52f66a6bf7fd05386915aef.jpg
Moved: pic-301-_jpg.rf.821c1245c0e331fa2bf691e53b6d5d99.jpg
Moved: pic-12-_jpg.rf.40ca7474661c6928638675cb6b4f648f.jpg
Moved: pic-185-_jpg.rf.e5609451b471c39a9c9eaf5ff7b3ac94.jpg
Moved: pic-219-_jpg.rf.aa439f808046db1dd790b1dd73aec45f.jpg
Moved: pic-259-_jpg.rf.d407eb770f6e539c7d1021089da068bc.jpg
Moved: pic-64-_jpg.rf.9d88ef6a6cc16ef8eec9b1688a9d598e.jpg
Moved: pic-201-_jpg.rf.e3dd8c6c5c18f97d98bdf92b1ce043b9.jpg
Moved: pic-283-_jpg.rf.40eb24734e3476c926a4c70fd547500c.jpg
Moved: pic-149-_jpg.rf.e58bb252f96f5f83d1d3290b4e6b8041.jpg
Moved: pic-62-_jpg.rf.d2884b15285690c8542d7391ee04de10.jpg
Moved: pic-21-_jpg.rf.e193c5d94e2cc8ef9b365e8d95e806b1.jpg
Moved: pic-102-_jpg.rf.cd0b0b3a64e3a11005884c98c1f6c3aa.jpg
Moved: pic-139-_jpg.rf.68c4e347a47e89fb46aedd298c2c3e5c.jpg
Moved: pic-170-_jpg.rf.3571a1273709f941c4936d6ee8b32214.jpg
Moved: pic-231-_jpg.rf.1ef52a6b450c206cfdcc425311a07859.jpg
Moved: pic-167-_jpg.rf.f15ca9251a252759a4206b00e88066ea.jpg
Moved: pic-47-_jpg.rf.b5c407806790722e3104e1521d054f67.jpg
Moved: pic-80-_jpg.rf.d08231a7b3ed0079786a5cc588acb6a8.jpg
Moved: pic-298-_jpg.rf.58b2ce2cbcbc68eb15a507b2cf8643e2.jpg
Moved: pic-101-_jpg.rf.8380b58f6540ec91db66934b342f7f9e.jpg
Moved: pic-90-_jpg.rf.9b8c41e2268c9abdc95c18b3567fb764.jpg
Moved: pic-96-_jpg.rf.462bc937bdab51c156a191ebd1cfc9c2.jpg
Moved: pic-162-_jpg.rf.7352a1a695f0ce198ca67b3f1c186fd6.jpg
Moved: pic-137-_jpg.rf.374184952caf59cfa399166b0111b640.jpg
Moved: pic-246-_jpg.rf.7b2fd4f45f1134c636d1a6fe51744d46.jpg
Moved: pic-78-_jpg.rf.6e55ada23b1148608d6daddc7d6d7e27.jpg
Moved: pic-280-_jpg.rf.a7c2022cd08be88cf40fb7473457b1bd.jpg
Moved: pic-242-_jpg.rf.61dffd0851eee83ef24f448d88ffeebe.jpg
Moved: pic-220-_jpg.rf.50845450b158301ab47748beb98fcf79.jpg
Moved: pic-197-_jpg.rf.76da5b1b10db8580430d527ce9cc2ac3.jpg
Moved: pic-130-_jpg.rf.0f6726c68af9fe60c2249e2349f8c049.jpg
Moved: pic-127-_jpg.rf.762e69fb9b1c80f586c501b5b9c515db.jpg
Moved: pic-23-_jpg.rf.e7e49a6cb4809947d14a95047f49964e.jpg
Moved: pic-48-_jpg.rf.5f35e42f4f2abf32c388f70cd219d8cb.jpg
Moved: pic-253-_jpg.rf.2d65914b2455aaeff16e8ef4321a9ae2.jpg
Moved: pic-104-_jpg.rf.e4efc52e048da0b6918c135b1bd39962.jpg
Moved: pic-107-_jpg.rf.03fc77860b4af0df70c5ab46db783441.jpg
Moved: pic-233-_jpg.rf.59141047e39ac5b57f2f9b1f6a763936.jpg
Moved: pic-39-_jpg.rf.916c6c1f6b88b55f48b08e48481fe26f.jpg
Moved: pic-110-_jpg.rf.ddb9b30f00ca7dfad4235fcd67610a9b.jpg
Moved: pic-94-_jpg.rf.2aabac75e10d9308647adbe3285a5498.jpg
Moved: pic-279-_jpg.rf.eb289e54650f25791d195ce8f1936cf8.jpg
Moved: pic-142-_jpg.rf.8658b3f74ded0b4631ae8fb8215d1f97.jpg
Moved: pic-226-_jpg.rf.b4fc5446d26d4211eece93e58f12ae73.jpg
Moved: pic-249-_jpg.rf.6e835a0b390d9b7815c33f5834b17a42.jpg
Moved: pic-13-_jpg.rf.b5e4ccd6fb004ba11f36c902116a6dfa.jpg
Moved: pic-41-_jpg.rf.4d2787d8d27bef19c2759899a13581ad.jpg
Moved: pic-185-_jpg.rf.4bf9653396b984986c36623ca51a9b89.jpg
Moved: pic-159-_jpg.rf.1ed8251ec141db216fc5041d7838f5e1.jpg
Moved: pic-136-_jpg.rf.af169e1464071ae718f22b5baebe13a6.jpg
Moved: pic-238-_jpg.rf.43a237ef9bd9dd28d4f798a87853f1fa.jpg
Moved: pic-253-_jpg.rf.1ddbaa9733534658408a1a14372ef0b9.jpg
Moved: pic-285-_jpg.rf.e85f33f618c8853f1b77a75be13c5a95.jpg
Moved: pic-131-_jpg.rf.9506d58945bc1f6e0cd0b6810ca40ad5.jpg
Moved: pic-235-_jpg.rf.caa8259752f70e86575c84bdc5a6ac3d.jpg
Moved: pic-162-_jpg.rf.f847c9d3c6c04f210e5e2f3e8eb444d4.jpg
Moved: pic-130-_jpg.rf.2326fd752be4eb885ad113b533f9ac5c.jpg
Moved: pic-272-_jpg.rf.9c136160d287bbdaaaa5e6027f75ba97.jpg
Moved: pic-267-_jpg.rf.9bb1142dec3532e4e8b716d3a438ac05.jpg
Moved: pic-4-_jpg.rf.4db592c400a3bacb104e601c50c1fcd0.jpg
Moved: pic-274-_jpg.rf.5205af7f7d0021ecd8ac84b895d7be99.jpg
Moved: pic-143-_jpg.rf.f94e3b194754043332e4361c80e7d3db.jpg
Moved: pic-118-_jpg.rf.cf3c2b75ffec6c9e27d18a6b98b67bf9.jpg
Moved: pic-11-_jpg.rf.7bf3ce1997b0a5d878ad6fabe1e5772a.jpg
Moved: pic-89-_jpg.rf.f60ba1af20cc526575b9ddab3e79052d.jpg
Moved: pic-250-_jpg.rf.a3ea467a7cc80896f04d44bea680785d.jpg
Moved: pic-241-_jpg.rf.c898c9588e06414254eb3a8101ade893.jpg
Moved: pic-113-_jpg.rf.dfebb14b79daa214f3f87995192a85ae.jpg
Moved: pic-164-_jpg.rf.34bf0aa5f308144c68fb1b5f9a1b9423.jpg
Moved: pic-79-_jpg.rf.b8083f42dac8ce2a5d303479dc967792.jpg
Moved: pic-48-_jpg.rf.88ad29d468c207f23e22f16b5129a5fe.jpg
Moved: pic-277-_jpg.rf.d1a4a881471530c27e8e6acefaae408d.jpg
Moved: pic-281-_jpg.rf.364ad6841f1f703e567868636d3c5d9d.jpg
Moved: pic-111-_jpg.rf.748bde6c84a85700fe3e4a8ad8e5c83c.jpg
Moved: pic-266-_jpg.rf.43407daa6e772a254285f6bf1098a9b2.jpg
Moved: pic-3-_jpg.rf.1f39da1d67e7044320a0a602d9819741.jpg
Moved: pic-91-_jpg.rf.d541de11cd8503ce68f73abd1fb02717.jpg
Moved: pic-224-_jpg.rf.bc36d7a2ab5872952f3237e3cb9a0b06.jpg
Moved: pic-251-_jpg.rf.2fdb4a020ffa343ae74099d9d2876c41.jpg
Moved: pic-244-_jpg.rf.9beb79771a7b6709183e6cca511ff830.jpg
Moved: pic-244-_jpg.rf.1cc262720c9af6dae71db8520773160b.jpg
Moved: pic-264-_jpg.rf.1d9a2cc87b0162c31ffde047cca87a81.jpg
Moved: pic-24-_jpg.rf.5c0e8c26b2a5c454bf448e0b6f2ecd97.jpg
Moved: pic-18-_jpg.rf.f4e625f77be483b3db88308e516192a1.jpg
Moved: pic-206-_jpg.rf.5e77130a98b6e44f7347f3fa12d59989.jpg
Moved: pic-296-_jpg.rf.8761505829f0631199e1d3daa72bea42.jpg
Moved: pic-275-_jpg.rf.d21f3ba7cea2b4ce92516d08a7ea0c6d.jpg
Moved: pic-300-_jpg.rf.4ef818f9e780452ddfb899a2a2b6b03a.jpg
Moved: pic-138-_jpg.rf.07fa25bc5fbd7c2711b9ce8ac28ad6a2.jpg
Moved: pic-135-_jpg.rf.1ee928d9f772b66ef1a56bc9ddc702b2.jpg
Moved: pic-112-_jpg.rf.a0296021fd4252e341077743b0990cb8.jpg
Moved: pic-85-_jpg.rf.c5fc2aff67696bb00ec93f0e00d6b41d.jpg
Moved: pic-265-_jpg.rf.98e8661b5363f6c6bcf399738c291cf2.jpg
Moved: pic-171-_jpg.rf.a81f6e206e422229e3021b0dfb06752f.jpg
Moved: pic-250-_jpg.rf.90193421f8c21ded95e0cbf404f513dd.jpg
Moved: pic-208-_jpg.rf.b11d7439f1c22388eac3f6705cb9e9e4.jpg
Moved: pic-73-_jpg.rf.00116918149ac51697ae5249644ef144.jpg
Moved: pic-203-_jpg.rf.0a2080c87c7d3188f8356357203b0e56.jpg
Moved: pic-107-_jpg.rf.f0ad7fbe0407cb85527525e503913079.jpg
Moved: pic-207-_jpg.rf.0b505406debb2b509daccf0ebbb62d42.jpg
Moved: pic-40-_jpg.rf.0b69a3e42d0f31491655adaa801c3160.jpg
Moved: pic-70-_jpg.rf.be12246c53c37bcff9d671a1052b23bb.jpg
Moved: pic-115-_jpg.rf.a808c9e7b2121bd93dbc59332a6d12cb.jpg
Moved: pic-318-_jpg.rf.d35f113f002fcda07300a87c4953d158.jpg
Moved: pic-220-_jpg.rf.0ec6700cefc477019e71e49c69ad09c0.jpg
Moved: pic-197-_jpg.rf.ca567ffa1d1798025a45cf933eb8a5ba.jpg
Moved: pic-141-_jpg.rf.94b5851bcded6830d88bef9ed5001cc4.jpg
Moved: pic-302-_jpg.rf.b78c512c8993fd44bdb300776d9dc3f4.jpg
Moved: pic-139-_jpg.rf.87bfef6ce65eb5df5b6053523e6b4954.jpg
Moved: pic-223-_jpg.rf.f7b0fe3cd7b84157379a0c10372ef0fc.jpg
Moved: pic-160-_jpg.rf.8ac19617548efc70a9281d8dc3794dfd.jpg
Moved: pic-318-_jpg.rf.fb982b0515cfdf43b2ced2b2b087b90d.jpg
Moved: pic-149-_jpg.rf.c349f70d3d136c391a0458b64dd56ebe.jpg
Moved: pic-98-_jpg.rf.9f186514621bd6868261aefd8bd19a66.jpg
Moved: pic-1-_jpg.rf.8d95dd1d29760a2634a45cc7fdd84b31.jpg
Moved: pic-34-_jpg.rf.add0f9e0bd6d5cd8a32bde8eac8b1c9f.jpg
Moved: pic-155-_jpg.rf.a0f2c54c02aec34c0ca6138b4635c155.jpg
Moved: pic-102-_jpg.rf.bb6db5bdb59d1a6af15b0a0b565a3cdb.jpg
Moved: pic-149-_jpg.rf.a45f79f8033191bd09e9ef31736ca58e.jpg
Moved: pic-131-_jpg.rf.30c2f70058a6fad525c31f57d3952d4d.jpg
Moved: pic-23-_jpg.rf.dfe14e39a7d78d0edb998700007564e1.jpg
Moved: pic-168-_jpg.rf.ad622f815165a84798a7922e02a02876.jpg
Moved: pic-52-_jpg.rf.d8822e3b6a7c8fe4c73543cd7d7ae9cd.jpg
Moved: pic-251-_jpg.rf.38a2bdb803b4ab772ebd6e40119129f8.jpg
Moved: pic-7-_jpg.rf.65c5742cced68822528a322492f2652d.jpg
Moved: pic-3-_jpg.rf.17e79b0608bc082d9380d713fb69f5ef.jpg
Moved: pic-100-_jpg.rf.8c9076ee84698f90f04765f4e794a819.jpg
Moved: pic-52-_jpg.rf.def4f32d6ba09bcb7a22b8a34a7c8115.jpg
Moved: pic-239-_jpg.rf.27ea296703d09cf2fc0438826eb25216.jpg
Moved: pic-221-_jpg.rf.6280cd42dfe06a2d66148f5b5af6eb1b.jpg
Moved: pic-138-_jpg.rf.766c3d35632f4641ce9d5207a3cadd70.jpg
Moved: pic-103-_jpg.rf.4fa35472ae606aca56d49966dc91b5b6.jpg
Moved: pic-284-_jpg.rf.56d84fad76218d5963847d758616e653.jpg
Moved: pic-46-_jpg.rf.ce935f81e259f69e3b8930f080141ac5.jpg
Moved: pic-57-_jpg.rf.98eff15743815f755fd3722f3836c850.jpg
Moved: pic-31-_jpg.rf.1174887817ec51f80c793c0f75927824.jpg
Moved: pic-10-_jpg.rf.500c683a687e403f4cdade4826a84b5b.jpg
Moved: pic-243-_jpg.rf.d07142e52129da403acd41a7a03fabae.jpg
Moved: pic-216-_jpg.rf.456e08f670a110afa6a40b982a029cba.jpg
Moved: pic-169-_jpg.rf.ce08674b1ae95506239ffe1d5e92d8a1.jpg
Moved: pic-220-_jpg.rf.577cbbb4c72285178adaa8c046e4f59d.jpg
Moved: pic-245-_jpg.rf.f64415f2a4f04934c63eb9e6ddc58b03.jpg
Moved: pic-2-_jpg.rf.bb6da014663463596e9cdcb39bfa3d40.jpg
Moved: pic-281-_jpg.rf.20f2248677b69cd0b78705416c578c8f.jpg
Moved: pic-194-_jpg.rf.0347198a0674c89124a169b3ede8d1b8.jpg
Moved: pic-105-_jpg.rf.0b52d3fe11f0b249a5eb2f14a8f0a14f.jpg
Moved: pic-87-_jpg.rf.9c686985ca1aaf482818536bad3a52d2.jpg
Moved: pic-76-_jpg.rf.3908b60fc10504b5de5ceb2ba0cddcb1.jpg
Moved: pic-168-_jpg.rf.470ca7ba7c3aed3a3ff0ca36725fadb6.jpg
Moved: pic-139-_jpg.rf.738912a20f4c9753a555bf9e7a468851.jpg
Moved: pic-96-_jpg.rf.24d21cef4cfb4d0f7bd6bcc6bc047d4c.jpg
Moved: pic-265-_jpg.rf.4c610d0dfdc177368e2334a82ff5513a.jpg
Moved: pic-112-_jpg.rf.565a4282cf6d23cbb37f3ee73567ec2b.jpg
Moved: pic-77-_jpg.rf.83c80a807ca47eb0192cb129ebc8cb41.jpg
Moved: pic-212-_jpg.rf.19e0e3168e988c6c8f8829f34c68003b.jpg
Moved: pic-85-_jpg.rf.02b3ed7783bfa794dcb56d483821c20c.jpg
Moved: pic-133-_jpg.rf.8dc9e79be10c01f6f279b4c27266ab65.jpg
Moved: pic-109-_jpg.rf.b84c3f664bd7ae818c9af8fb6bc95a9c.jpg
Moved: pic-252-_jpg.rf.9cb2afb0020b7d0e4220ed2f05fc3014.jpg
Moved: pic-233-_jpg.rf.8497a34a9e5ae4ee66830f050bbd69ac.jpg
Moved: pic-198-_jpg.rf.5bfd105d64b4c14a88672ff3fdefc4ea.jpg
Moved: pic-190-_jpg.rf.dbf09b649249bd7101e280f5a14957c6.jpg
Moved: pic-302-_jpg.rf.d633fdb04731410dc8d1d1da15a1363a.jpg
Moved: pic-110-_jpg.rf.c9150ba543315705a5bb08654144ccf9.jpg
Moved: pic-299-_jpg.rf.d1996e7e3608d23e5111b7e3f95a5353.jpg
Moved: pic-268-_jpg.rf.87ee237323b54bf65900f2fe8742e27b.jpg
Moved: pic-59-_jpg.rf.6f4e81b1ca5d29168033fa69c92c6e24.jpg
Moved: pic-15-_jpg.rf.988cf6bc7c8911ed0169be801328edb7.jpg
Moved: pic-122-_jpg.rf.a7402de11b1c3f7af0cc32933211e3f6.jpg
Moved: pic-159-_jpg.rf.2dcc275359fb301602e6957a56e13dc7.jpg
Moved: pic-174-_jpg.rf.7ffbfba8e5d63b5f4577f701ca5f7105.jpg
Moved: pic-34-_jpg.rf.40b75b0e55a33c21bc33826831384287.jpg
Moved: pic-299-_jpg.rf.ffefe6a973c89146c61be0770eed07c3.jpg
Moved: pic-81-_jpg.rf.2c871f142112a2de4e78f5730d77bf73.jpg
Moved: pic-215-_jpg.rf.d190a911a9e6195bd2a9e3c67869064a.jpg
Moved: pic-224-_jpg.rf.aa73fb95553763a3d73a6b849fa4aa11.jpg
Moved: pic-203-_jpg.rf.3377a5ba4a0dc953bac7e48a7a02c227.jpg
Moved: pic-30-_jpg.rf.50f47f18cb6f3fb3650fe72d391d9187.jpg
Moved: pic-189-_jpg.rf.cf414d706efddcb1fd32a8b42bcfd9a7.jpg
Moved: pic-164-_jpg.rf.9248a616cb0e3d24aa2bb44288e019ce.jpg
Moved: pic-49-_jpg.rf.ea29a2566cbd0e48094adae5b4cf7087.jpg
Moved: pic-66-_jpg.rf.2025b0c631dbf0d3277e7d8f95bbf6e8.jpg
Moved: pic-187-_jpg.rf.725f375e91986c9cc15b8f0b2b708cb9.jpg
Moved: pic-297-_jpg.rf.72ed26dca533a7e479c08103a5569c8f.jpg
Moved: pic-260-_jpg.rf.3af45c18af9183dbab32f9e489034912.jpg
Moved: pic-278-_jpg.rf.81490c823fe0f5ba5fc351b36c4fab79.jpg
Moved: pic-56-_jpg.rf.18ade0de978aa6c6068402dd80642ccf.jpg
Moved: pic-214-_jpg.rf.27fc3b4425584f6404f2f0feb976f621.jpg
Moved: pic-196-_jpg.rf.66a50a098577b349d7bee13dc9640c2e.jpg
Moved: pic-53-_jpg.rf.540025fd1af3f0c105d5a5f489e307da.jpg
Moved: pic-75-_jpg.rf.a4fb54bd2e21373bc7b34ffadb02d9eb.jpg
Moved: pic-260-_jpg.rf.b88fd61a801b35b27593f7fcbfed4f1b.jpg
Moved: pic-219-_jpg.rf.a0b3e7cf4174b760f731630a0d8ffcda.jpg
Moved: pic-171-_jpg.rf.f536cb9ac4138da71c6af4d8a3492050.jpg
Moved: pic-115-_jpg.rf.2ac2c551c23ad08dd5599f320c8dd310.jpg
Moved: pic-49-_jpg.rf.7566ef76e82dccc357ff1691393cdff8.jpg
Moved: pic-187-_jpg.rf.8978c4919b51dcb2843c4d992a0bc5f6.jpg
Moved: pic-46-_jpg.rf.b885bd57535b8adc199e02edae6a24e9.jpg
Moved: pic-119-_jpg.rf.8c7abcd78dd1d16256589acaf80a4182.jpg
Moved: pic-92-_jpg.rf.495b1e2e681aaf8bd9ec84f29044ff68.jpg
Moved: pic-298-_jpg.rf.cd5aa1c41d3e62814135dde19300f171.jpg
Moved: pic-111-_jpg.rf.39065e4e7f12e6c9d4e829f9df001cec.jpg
Moved: pic-201-_jpg.rf.95832ba3432d34d8935a2aa3290fcccc.jpg
Moved: pic-281-_jpg.rf.91f845ebe6009e9c3be546fa34f1fb62.jpg
Moved: pic-133-_jpg.rf.24a41f4b91e68f7e35f7d2feff83054d.jpg
Moved: pic-210-_jpg.rf.4b2ea541aa7fb1277177d6b23ebb385d.jpg
Moved: pic-156-_jpg.rf.a3c099766b4b6cb736f460bf8f3b8377.jpg
Moved: pic-180-_jpg.rf.16f8930512bc55a715ff702283ede87f.jpg
Moved: pic-211-_jpg.rf.4f06bc1e4c4ca8189e8136ed45695acc.jpg
Moved: pic-64-_jpg.rf.5a0e8d02278b5430fa7bd514f437f041.jpg
Moved: pic-234-_jpg.rf.bc29e6e5e745094cb40ab4d9023e2ad3.jpg
Moved: pic-238-_jpg.rf.28fccf586765c2246d9b66e5eb8f3584.jpg
Moved: pic-100-_jpg.rf.17047bb032a49c96643c5f2108bb99dd.jpg
Moved: pic-216-_jpg.rf.9b0074a18a22ac4ecb7f30b6dabe3fa5.jpg
Moved: pic-159-_jpg.rf.12b33adab537f585de7b3d85b848618e.jpg
Moved: pic-97-_jpg.rf.f126b87cc73c733f34169b87ffbe0a52.jpg
Moved: pic-264-_jpg.rf.6219b6cecf8a84cc4bd3139144ade94f.jpg
Moved: pic-227-_jpg.rf.bfb22269f25cce0b5e7ff3054f61734b.jpg
Moved: pic-237-_jpg.rf.fa5cabd66a044525bb74f3c49acf54fe.jpg
Moved: pic-153-_jpg.rf.f7752000f79cfa2acc35f9a7149ee56d.jpg
Moved: pic-21-_jpg.rf.31dc8d894956f53d54a5cec0f94c5e79.jpg
Moved: pic-6-_jpg.rf.dcd3fa3c9b81035067fbcb5e4998db50.jpg
Moved: pic-56-_jpg.rf.8c8d4aebd0f2fb128a231b7b798bd669.jpg
Moved: pic-275-_jpg.rf.98225472f61e9de4245a1da0fc036230.jpg
Moved: pic-218-_jpg.rf.da6e0c0a3dd3854e5710bcbe50478725.jpg
Moved: pic-287-_jpg.rf.87156b9d129afc59b232dcc6247af143.jpg
Moved: pic-44-_jpg.rf.c7dd071d0249ce1a01f71938c20eec2e.jpg
Moved: pic-37-_jpg.rf.141623e970a3b93aa37e180a3efb32b8.jpg
Moved: pic-286-_jpg.rf.e5f176bec46993c0c6cda6588e9d5ecf.jpg
Moved: pic-106-_jpg.rf.0cbfb7193cdb49723d65f538678e22d2.jpg
Moved: pic-261-_jpg.rf.2b6a7b01bb03728cc1c166db16e462e5.jpg
Moved: pic-212-_jpg.rf.d80a26f98663f0c2a92282a15fbf262b.jpg
Moved: pic-49-_jpg.rf.a2d3901d28aa5d5a7040913eaffb5011.jpg
Moved: pic-2-_jpg.rf.f0b15cd48578f75fff175242f1d8d9d0.jpg
Moved: pic-146-_jpg.rf.6d367895786517cfe865fb065be076a5.jpg
Moved: pic-26-_jpg.rf.cd93dd54b669257758fd0cdafe4f0032.jpg
Moved: pic-300-_jpg.rf.3600a16f8f27cc0334db7f049f787eb1.jpg
Moved: pic-24-_jpg.rf.c4aa15eeb12eb5d97a7d89fc47d7cca6.jpg
Moved: pic-195-_jpg.rf.ace8dee3ec0fba3d7a33c3de2c315f0a.jpg
Moved: pic-283-_jpg.rf.c2b4badba5de7ededb5266fa40bff815.jpg
Moved: pic-122-_jpg.rf.c136dab4f56b39061798109d2420b61f.jpg
Moved: pic-11-_jpg.rf.489d3c93901c3240d87b78333702d26c.jpg
Moved: pic-130-_jpg.rf.573aa03e77804ed419f1fd0a190ba13a.jpg
Moved: pic-172-_jpg.rf.171729c8713c604e4d2371b546dfa09f.jpg
Moved: pic-274-_jpg.rf.46a9e2047dced3e94c4fa2aab121859b.jpg
Moved: pic-155-_jpg.rf.424bbc028685f5de7e9cc866eb988b1e.jpg
Moved: pic-158-_jpg.rf.7c67c2036a30fd93eed5361cc2f4f1c8.jpg
Moved: pic-145-_jpg.rf.8c8e224f08327d871ec0791f80a0d43a.jpg
Moved: pic-59-_jpg.rf.e6834834f2f355ae4e8d55f881695099.jpg
Moved: pic-188-_jpg.rf.635564dad2da056faf9127525b2b6cb4.jpg
Moved: pic-160-_jpg.rf.046afe1498d1564227421d54b7abdcaa.jpg
Moved: pic-55-_jpg.rf.ab51f5f29c2cabd3037a7f562d7c3a48.jpg
Moved: pic-126-_jpg.rf.260cc574c3efc137da742a912741a3fb.jpg
Moved: pic-44-_jpg.rf.7bb3eef4deaf2aa9c2fb506c168e3f77.jpg
Moved: pic-261-_jpg.rf.998892ecacb90555cc17a10e7717e639.jpg
Moved: pic-189-_jpg.rf.6ecb9b14009286fba81f2e83e3b7f1e1.jpg
Moved: pic-75-_jpg.rf.f73e19df2feadf86dbc38f4eb690d204.jpg
Moved: pic-148-_jpg.rf.8e92fc1a329453e782f06e741d1fc52f.jpg
Moved: pic-147-_jpg.rf.a31a26433609129cbb67d23fcb851296.jpg
Moved: pic-285-_jpg.rf.c3f2aadaa48b640a80c3ab44e41ffb04.jpg
Moved: pic-105-_jpg.rf.0ce0939aec2bb2ab235addf64d130914.jpg
Moved: pic-89-_jpg.rf.88d2db98329fc9ad290d1f559d3c8c76.jpg
Moved: pic-138-_jpg.rf.8b1343ad71a58c8daf99e2311627f0c8.jpg
Moved: pic-181-_jpg.rf.e0d1623b0c6c69da4a967af45bebbdbd.jpg
Moved: pic-10-_jpg.rf.5a901c212d899a7dc7dc78be7de892c0.jpg
Moved: pic-65-_jpg.rf.be4b7862a50c7fd0105a6a47ea0f48b9.jpg
Moved: pic-259-_jpg.rf.47ec4246b71311c95725c8e5c02049a3.jpg
Moved: pic-255-_jpg.rf.58d537e75af0a9fe40651c5c9e5c6f10.jpg
Moved: pic-74-_jpg.rf.753bab7893e8644b71fea76010278698.jpg
Moved: pic-30-_jpg.rf.881c629f5ecaecfe726c74a522b8decb.jpg
Moved: pic-24-_jpg.rf.6f72a29392e37293dead7ab866cff716.jpg
Moved: pic-97-_jpg.rf.5fdb2665d8114a571692b42b87a9da50.jpg
Moved: pic-289-_jpg.rf.3b5e34d314c7ded93c3733fce130b12a.jpg
Moved: pic-155-_jpg.rf.ba6a2e4e1abc6f5aa893e46932e4df4f.jpg
Moved: pic-293-_jpg.rf.521af54aebbf6c4a9777b1a21b2aa1a6.jpg
Moved: pic-191-_jpg.rf.f1ecc5629bdf5860ae57d7d27dafb299.jpg
Moved: pic-249-_jpg.rf.2909e1821a38907edf8d4f9d87cfa7fa.jpg
Moved: pic-103-_jpg.rf.e204fd0f4f80094ec52c54c31ab06db0.jpg
Moved: pic-51-_jpg.rf.bc4a2c2beca4c0a398dbc10fc7efc934.jpg
Moved: pic-74-_jpg.rf.16da87d5105f997141b5538f74203204.jpg
Moved: pic-137-_jpg.rf.5b5d603ae481652805ea93e3698ea609.jpg
Moved: pic-68-_jpg.rf.20cbf511ac305a699cd432846cbb264f.jpg
Moved: pic-189-_jpg.rf.7a11114bc4c2fe1c330b2eff3ec1b609.jpg
Moved: pic-16-_jpg.rf.946ec84ddfa3a53b7b2d407349f08e62.jpg
Moved: pic-79-_jpg.rf.be47d8798d6f806389366b2c6e3a3dd1.jpg
Moved: pic-91-_jpg.rf.d4d38cce067db39408794242a91f0efa.jpg
Moved: pic-248-_jpg.rf.a3cbf0b1296da7cd3ea5d46525c3b5ad.jpg
Moved: pic-3-_jpg.rf.9fea650aedf412fa2559d06c40de20b9.jpg
Moved: pic-251-_jpg.rf.9841cb1e9b954b905fb2c6573c987199.jpg
Moved: pic-191-_jpg.rf.722924f292c69c3948e42a9759882f26.jpg
Moved: pic-247-_jpg.rf.5b9be4976067ff481a06a5d7f1916133.jpg
Moved: pic-87-_jpg.rf.f695dc4e18d8786274de900672c1e629.jpg
Moved: pic-222-_jpg.rf.1dbe9dca4ca6a1f1f88b41787b9a691c.jpg
Moved: pic-287-_jpg.rf.e2570badb95698d083c54eec726d833c.jpg
Moved: pic-278-_jpg.rf.102a71b41c699ef91c98ee9acb233241.jpg
Moved: pic-277-_jpg.rf.ec1e5c4b6a23a9196e33d1937e2fddcf.jpg
Moved: pic-117-_jpg.rf.a5e887bf3c2428e83a81dc48e4f80b0e.jpg
Moved: pic-136-_jpg.rf.d694cf94912347ceff66727b95ecb05a.jpg
Moved: pic-214-_jpg.rf.d45b506908081039adeb183e4ca51da8.jpg
Moved: pic-54-_jpg.rf.f0c232122401c2974af21cab0c286439.jpg
Moved: pic-299-_jpg.rf.b9479d0a39352215db193b6877e389ff.jpg
Moved: pic-142-_jpg.rf.0879365f4e7e435dba77c82134cc5623.jpg
Moved: pic-217-_jpg.rf.6bb67326dc3fab2b66c9c65a3364504c.jpg
Moved: pic-211-_jpg.rf.9de311e1f9663a4ed2159ebc521295e7.jpg
Moved: pic-259-_jpg.rf.4a53c38246579af08ffa2398e0d809aa.jpg
Moved: pic-40-_jpg.rf.c8d57f2324c265fbe81623987f86e3d8.jpg
Moved: pic-172-_jpg.rf.b732ca94d029e82283eed3228fae8625.jpg
Moved: pic-240-_jpg.rf.6cf12918112f73e428cb65a891665604.jpg
Moved: pic-71-_jpg.rf.0f9bcdab2065fee694fefca6af561329.jpg
Moved: pic-295-_jpg.rf.a8c2971b57a19e0180c662e4263aa9b5.jpg
Moved: pic-119-_jpg.rf.4871608ed18b586f1e4e5f2e440b1320.jpg
Moved: pic-216-_jpg.rf.ad6fbe4b6c5100ec699f1262c74a5988.jpg
Moved: pic-276-_jpg.rf.792c2b69462ae79fca0cca74330fe0e7.jpg
Moved: pic-199-_jpg.rf.89fa1c3f06bec1dfef2b96f692db78b6.jpg
Moved: pic-126-_jpg.rf.c72b1826e8aaa63d8f1713c2957e93e5.jpg
Moved: pic-13-_jpg.rf.6ada3c0e80b409618278df949cd6b7e5.jpg
Moved: pic-294-_jpg.rf.a69a7de19ef308ef7ee254d1016bbc97.jpg
Moved: pic-53-_jpg.rf.7815bad4623e4bb70645806ea5a77a47.jpg
Moved: pic-31-_jpg.rf.f773855cfccc522535461bb0d18add8a.jpg
Moved: pic-134-_jpg.rf.a84bccc6824f607509bb701d8ccd3c87.jpg
Moved: pic-121-_jpg.rf.292a7daa7fa877194720b879161d8c40.jpg
Moved: pic-176-_jpg.rf.be38366f2703b44711a2e9486cc677d3.jpg
Moved: pic-191-_jpg.rf.eecd3cdfc404f62988bc698f87ae2e4e.jpg
Moved: pic-239-_jpg.rf.8f2076aea9dd8405d1992210d01df6ef.jpg
Moved: pic-83-_jpg.rf.658f94a0e7d008ff38e85a627d6f699e.jpg
Moved: pic-81-_jpg.rf.f826102d59ca692fc6a7cd93131a448e.jpg
Moved: pic-198-_jpg.rf.3fd6176b3671e235690487a5759a10f9.jpg
Moved: pic-25-_jpg.rf.2d988998b2a995bdee0f0282803e4801.jpg
Moved: pic-25-_jpg.rf.0c7a3fd9a3840f28576edfe095f5b2c8.jpg
Moved: pic-302-_jpg.rf.37977cf11bbe714965571c19d72ffee0.jpg
Moved: pic-76-_jpg.rf.4062413067c04acc387e651210b12921.jpg
Moved: pic-169-_jpg.rf.f326f486b62b79f5bc791704fabd90e8.jpg
Moved: pic-297-_jpg.rf.1d4e40786715d3c83bace206f962c042.jpg
Moved: pic-156-_jpg.rf.9e41f44435259c8fa4baadcdbc5f0f7f.jpg
Moved: pic-234-_jpg.rf.c7c54a2bd8c106f1e8959e88238d0f3c.jpg
Moved: pic-234-_jpg.rf.6e6834e9f26a64c34edc2093c2133e77.jpg
Moved: pic-8-_jpg.rf.f2cd6b29cbaf9efb1f836b4c78aca3f9.jpg
Moved: pic-101-_jpg.rf.1e32a49f89a38974ded11bba8dd3e56b.jpg
Moved: pic-55-_jpg.rf.87cabcde97c75c9068793716694ef1c5.jpg
Moved: pic-109-_jpg.rf.de4b44ded5874999731e65adcf907536.jpg
Moved: pic-197-_jpg.rf.0216ae6ebea5c3912f51c76bdbae6d19.jpg
Moved: pic-217-_jpg.rf.f71278c900f04d9ef934d1671e450fbf.jpg
Moved: pic-265-_jpg.rf.55be0618279efba17a40682b25ec9fab.jpg
Moved: pic-102-_jpg.rf.df35bf045672f19a05f84a8c365dab3a.jpg
Moved: pic-40-_jpg.rf.7047af1ffe9d3d01ef41591660a7bd37.jpg
Moved: pic-266-_jpg.rf.97039c9e51a9baa0832be4ebd044110d.jpg
Moved: pic-132-_jpg.rf.955ee641285edaa97d368881f70563fd.jpg
Moved: pic-1-_jpg.rf.e238c9bf3fe82e8ac55b0014a27fc529.jpg
Moved: pic-194-_jpg.rf.15feb8e01893318219d223a82a97d069.jpg
Moved: pic-190-_jpg.rf.a8973074639f95f416ad6ba0ccbbb03e.jpg
Moved: pic-7-_jpg.rf.7400b47430ca61631409d5ec433fbf79.jpg
Moved: pic-46-_jpg.rf.c5a8cb20f04ee8a90e2295b8e74a9dd1.jpg
Moved: pic-73-_jpg.rf.30b9fb02402e11d9d73579c9c007e6f1.jpg
Moved: pic-66-_jpg.rf.ad992ba43ecdd6892307c96e01da1afa.jpg
Moved: pic-132-_jpg.rf.797a01efcb3ccc31edc05fbd79854344.jpg
Moved: pic-65-_jpg.rf.e602ed35d690902722b26561dd3f9684.jpg
Moved: pic-39-_jpg.rf.99d4097fac96d5f035d066f05bd3dcac.jpg
Moved: pic-38-_jpg.rf.f986b908d11e3ccfab5acb989bc9aa7b.jpg
Moved: pic-168-_jpg.rf.d6e69d2d4e07bc489d1f95b357e47d26.jpg
Moved: pic-5-_jpg.rf.f3d79095cd22dd76dc99c447f82e50d0.jpg
Moved: pic-77-_jpg.rf.5d2577e0f9e471d4b9dcfce00a96d034.jpg
Moved: pic-106-_jpg.rf.e4becd5b84615a7550986c2835dc285e.jpg
Moved: pic-5-_jpg.rf.5fbe76ea8a76e35b41970ccb6f5e4730.jpg
Moved: pic-16-_jpg.rf.47407d69db6694be4d9fa4b3c032d235.jpg
Moved: pic-13-_jpg.rf.f7751cf8a51dd62c4e458caa96bc1906.jpg
Moved: pic-135-_jpg.rf.d3d07ce395c3562793390b1003e99d1f.jpg
Moved: pic-53-_jpg.rf.1ee5c3ca066d62d6b4aed03d3575b5ea.jpg
Moved: pic-206-_jpg.rf.72255834e8accc349443c0b769bd3cfc.jpg
Moved: pic-261-_jpg.rf.a966d2dffd8b171b302656a73d5b9d35.jpg
Moved: pic-78-_jpg.rf.51b8d15858f724437e1ce83b1f7a76a0.jpg
Moved: pic-294-_jpg.rf.1de461b1d76feb49d4f027f59f73b1ff.jpg
Moved: pic-248-_jpg.rf.b57094138ac0e7270328a9956b2f616e.jpg
Moved: pic-201-_jpg.rf.4b6780fd03079cb3617f1b6c3893f081.jpg
Moved: pic-253-_jpg.rf.fe9146427e9147a64aa2edd89579fa80.jpg
Moved: pic-132-_jpg.rf.17911c1b0d9ce482c109ce1e784940b4.jpg
Moved: pic-232-_jpg.rf.848346f3e53f08683c1c17d6f1f7437e.jpg
Moved: pic-31-_jpg.rf.0940348a848c8c97f3fff9383cb3cdc8.jpg
Moved: pic-71-_jpg.rf.c09149434e1578a21379b1ec049c97e2.jpg
Moved: pic-8-_jpg.rf.b4762871ab415292cd35f6ee6e2059a5.jpg
Moved: pic-113-_jpg.rf.b8d031ce65af24e0b5e80cab8723335b.jpg
Moved: pic-91-_jpg.rf.fdcc03fa51403644168dfca373c9ee0c.jpg
Moved: pic-267-_jpg.rf.4e80309c7e97b759c02f198b4f8258e0.jpg
Moved: pic-171-_jpg.rf.2de27493e9ea7ae685e6a868e05dff51.jpg
Moved: pic-52-_jpg.rf.f05e2cd157034e39c0eb9db8e7f09bb5.jpg
Moved: pic-65-_jpg.rf.7fa7e133ba0c2210d5075b0795e6815d.jpg
Moved: pic-133-_jpg.rf.7aa442a433a0074d31ec5ba2de39c2a4.jpg
Moved: pic-111-_jpg.rf.3a38a17ad93dbe166ddcc54aae67d206.jpg
Moved: pic-221-_jpg.rf.4210790f4f714436b3d5ee9671a99005.jpg
Moved: pic-256-_jpg.rf.e7df3aab64f144506e0d276e972a5f73.jpg
Moved: pic-258-_jpg.rf.821cd6dd9ff8fdcc6286183f5688755a.jpg
Moved: pic-90-_jpg.rf.f684f3079bfb74c1078e8f8dc7e6fd35.jpg
Moved: pic-7-_jpg.rf.75ec4611f8576a0f7706a3767986d5fa.jpg
Moved: pic-131-_jpg.rf.7a54a7e1ad2243629779c48a41b94ca1.jpg
Moved: pic-110-_jpg.rf.c61b825409e38c7651bca32e1d9680b5.jpg
Moved: pic-187-_jpg.rf.cc1cf985fedc5bc6d7b3fda53980e6f3.jpg
Moved: pic-177-_jpg.rf.c2ece8aa91efbc0843296da9f0892b5b.jpg
Moved: pic-79-_jpg.rf.fa63c47cf0aa776aec75efb4df84f724.jpg
Moved: pic-105-_jpg.rf.859bee21c8abeda9bc4ef41da6d2d0bf.jpg
Moved: pic-85-_jpg.rf.a64446b223ce0bba88626d3b9688cb5f.jpg
Moved: pic-142-_jpg.rf.d06e1261d14a5a908632f7f9984b1533.jpg
Moved: pic-11-_jpg.rf.39503b2272330e0dd57ffe9fc6ed720e.jpg
Moved: pic-267-_jpg.rf.a52b175e07343220015b707b9886e0e1.jpg
Moved: pic-94-_jpg.rf.ba3925642e2ccb4869665efacd0c7649.jpg
Moved: pic-73-_jpg.rf.08280c0eeb6772c510479ba1a84a6778.jpg
Moved: pic-35-_jpg.rf.d7c110298e8deb6c82e6a13278880bc1.jpg
Moved: pic-93-_jpg.rf.13ed0023300da63a2f33a803df745530.jpg
Moved: pic-30-_jpg.rf.370eca9f98e828703d153a162dba5233.jpg
Moved: pic-266-_jpg.rf.5924896fbc8c112511de0c67db59435b.jpg
Moved: pic-241-_jpg.rf.3432cc48d4f6e7d8002d6eb4642495ce.jpg
Moved: pic-232-_jpg.rf.f4098546b7c8b3af5f3463c6f63950dd.jpg
Moved: pic-43-_jpg.rf.dbbb1c368f5ada95ebf45d45838b1bd7.jpg
Moved: pic-150-_jpg.rf.80838b8e9f59a59d85e9727727b31fd7.jpg
Moved: pic-145-_jpg.rf.ea068320394add8a6ff90b4396b79923.jpg
Moved: pic-172-_jpg.rf.96d2ff93572de0ce5bd564113ece7ad0.jpg
Moved: pic-170-_jpg.rf.a8d1a4654900167fc8106a1f6144ceff.jpg
Moved: pic-243-_jpg.rf.0df6511df9c5cff60f86c536ab1635a1.jpg
Moved: pic-163-_jpg.rf.d56b832482912f0e78e017e95747fdea.jpg
Moved: pic-62-_jpg.rf.d50db2cc8bb871fd0925592de1923193.jpg
Moved: pic-6-_jpg.rf.20fe5b2f0851cc97b06f4a9d68881330.jpg
Moved: pic-284-_jpg.rf.123096f07316bdbbb775d4e0edbfcb5e.jpg
Moved: pic-14-_jpg.rf.0cf42e6b552e8f867e76237f36e7eadc.jpg
Moved: pic-163-_jpg.rf.75e0f6d481468e27710dc5bec3a78ea2.jpg
Moved: pic-264-_jpg.rf.b1224cd0b28b41a38580f8f73315e5be.jpg
Moved: pic-70-_jpg.rf.3fa842cfa55b39d094c6e4be45aaf994.jpg
All images have been moved successfully.

```

**MAKING LABELS FOR TRAIN FOLDER**

```python
import os
import pandas as pd
import yaml
from PIL import Image

# Define paths for the dataset
csv_path = '/content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/train/_annotations.csv'  # Path to your CSV file
images_dir = '/content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/train/images'  # Directory where images are stored
labels_dir = '/content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/train/labels'  # Directory to save YOLO labels
train_images_path = '/content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/train/images'
val_images_path = '/content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images'
yaml_path = '/content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/dataset.yaml'

# Ensure the labels directory exists
os.makedirs(labels_dir, exist_ok=True)

# Load CSV file
df = pd.read_csv(csv_path)

# Define class mappings
class_mapping = {"Pothole": 0}  # YOLO requires class ids; assign 0 for Pothole

# Helper function to convert bounding boxes to YOLO format
def convert_bbox_to_yolo(img_width, img_height, xmin, ymin, xmax, ymax):
    dw = 1. / img_width
    dh = 1. / img_height
    x_center = (xmin + xmax) / 2.0 * dw
    y_center = (ymin + ymax) / 2.0 * dh
    width = (xmax - xmin) * dw
    height = (ymax - ymin) * dh
    return (x_center, y_center, width, height)

# Convert annotations in the CSV to YOLO format
for index, row in df.iterrows():
    # Get the image name and path
    image_name = row['filename']  # Update if your CSV uses a different column name for the image file name
    image_path = os.path.join(images_dir, image_name)

    # Ensure the image exists
    if not os.path.exists(image_path):
        print(f"Image {image_path} not found. Skipping.")
        continue

    # Read image dimensions
    img = Image.open(image_path)
    img_width, img_height = img.size

    # Extract bounding box details
    xmin, ymin, xmax, ymax = row['xmin'], row['ymin'], row['xmax'], row['ymax']
    class_id = class_mapping.get(row['class'], 0)  # Map class to a numeric ID

    # Convert to YOLO format
    x_center, y_center, width, height = convert_bbox_to_yolo(img_width, img_height, xmin, ymin, xmax, ymax)

    # Save YOLO annotation
    label_file = os.path.join(labels_dir, os.path.splitext(image_name)[0] + '.txt')
    with open(label_file, 'a') as f:  # 'a' mode appends for multiple objects per image
        f.write(f"{class_id} {x_center} {y_center} {width} {height}\n")

print("YOLO annotations generated successfully.")

# Create the dataset.yaml file
data_config = {
    'train': train_images_path,
    'val': val_images_path,
    'names': {i: name for i, name in enumerate(class_mapping.keys())}
}

# Save the configuration to dataset.yaml
with open(yaml_path, 'w') as f:
    yaml.dump(data_config, f)

print(f"dataset.yaml created at: {yaml_path}")
```

```
YOLO annotations generated successfully.
dataset.yaml created at: /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/dataset.yaml

```

**MOVING VALIDATING IMAGES TO IMAGE FOLDER**

```python
import os
import shutil

# Define paths for the dataset
source_images_dir = '/content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid'  # Original folder with images
destination_images_dir = '/content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images'  # New folder to move images

# Ensure the destination directory exists
os.makedirs(destination_images_dir, exist_ok=True)

# List all the files in the source directory
all_files = os.listdir(source_images_dir)

# Move the image files
for file_name in all_files:
    # Only move image files (optional: check for image extensions like .jpg, .png)
    if file_name.lower().endswith(('.png', '.jpg', '.jpeg', '.bmp', '.tiff')):
        # Define full file paths
        source_path = os.path.join(source_images_dir, file_name)
        destination_path = os.path.join(destination_images_dir, file_name)

        # Ensure the file exists before moving
        if os.path.exists(source_path):
            shutil.move(source_path, destination_path)
            print(f"Moved: {file_name}")
        else:
            print(f"File {file_name} not found in {source_images_dir}")

print("All images have been moved successfully.")
```

```
Moved: pic-42-_jpg.rf.28b626ac5e887c92feeed1a3c5e85b64.jpg
Moved: pic-33-_jpg.rf.143c56d136e3245555b26b4d5108a4e1.jpg
Moved: pic-273-_jpg.rf.36d10c68fb23799bd0a58e48e0b995ce.jpg
Moved: pic-114-_jpg.rf.a0f30e06b3b96d7879d5f55a7012433c.jpg
Moved: pic-290-_jpg.rf.bcf58ab867c40a607759aec5666fece4.jpg
Moved: pic-183-_jpg.rf.277cfed19f046acc63dc9640b239f1df.jpg
Moved: pic-151-_jpg.rf.45a82558c583efe9dda4ea02e294595a.jpg
Moved: pic-228-_jpg.rf.4dcc6aa7dfc0c9a59a7f033e2ed12413.jpg
Moved: pic-178-_jpg.rf.2e27d006aec1544f1eec88d9170fd6ce.jpg
Moved: pic-292-_jpg.rf.f3d0a40ac5190529f4dd4886d6f5e5d0.jpg
Moved: pic-165-_jpg.rf.82b3db37518b15aa73be6e4093deaf46.jpg
Moved: pic-161-_jpg.rf.1cff77d21f54b7ed9234e896abcf0f5b.jpg
Moved: pic-144-_jpg.rf.61a3b886f058ed3a4788426cfa7c4988.jpg
Moved: pic-20-_jpg.rf.4b34591f154f226347c9ca9dfb33b2e4.jpg
Moved: pic-95-_jpg.rf.eca25439e9e1dd31f29df105f4faa122.jpg
Moved: pic-193-_jpg.rf.4520ff34079afc8e9f9b50a633c08876.jpg
Moved: pic-72-_jpg.rf.82c8314917ff5284106bd3428cff5792.jpg
Moved: pic-28-_jpg.rf.fe8316c392940899d9211be3305c9ab6.jpg
Moved: pic-140-_jpg.rf.430bfe74decf2b904377d127914f2092.jpg
Moved: pic-173-_jpg.rf.73512294c1b7b5c500eac27a0fb669f7.jpg
Moved: pic-269-_jpg.rf.196b54c0db633b6b02612f69072abb99.jpg
Moved: pic-36-_jpg.rf.13a668c4003681c4631508465eef5a9f.jpg
Moved: pic-262-_jpg.rf.02970860794f859699c9f743bc0fd7d1.jpg
Moved: pic-99-_jpg.rf.28d287fa96c09a12f2511e1b4df7e5a1.jpg
Moved: pic-123-_jpg.rf.385ae3fbcdabda81f72ddf11f6a4b93d.jpg
Moved: pic-116-_jpg.rf.ddcb9d0e0bcf2a1a5096c4f04e6b7f9e.jpg
Moved: pic-125-_jpg.rf.3d316e9144cb7438021e01065de91057.jpg
Moved: pic-175-_jpg.rf.9fc746d4865c11f38047cf383baa30a6.jpg
Moved: pic-308-_jpg.rf.8f5b6dc0b616365d05bce17bf30eff39.jpg
Moved: pic-205-_jpg.rf.cf4be807bced55552b98c208585d2c56.jpg
Moved: pic-61-_jpg.rf.72ad391fcf2334c24de5ed48dda25001.jpg
Moved: pic-225-_jpg.rf.38cc0deddb897c98814f644451130bb7.jpg
Moved: pic-45-_jpg.rf.8e102a986584d47797dc92558c2af624.jpg
Moved: pic-152-_jpg.rf.510fb0040c8523bb66ec10b0fe67b4b4.jpg
Moved: pic-230-_jpg.rf.ffe557c4b95e23f1a4323cf7768060f2.jpg
Moved: pic-27-_jpg.rf.b4cd8eb26d6941eabfc17280f03bca69.jpg
Moved: pic-22-_jpg.rf.aec225ee7ab2b5f7791d6579b213600b.jpg
Moved: pic-192-_jpg.rf.e0b55409488785e7156677026d372c23.jpg
Moved: pic-67-_jpg.rf.663b4f930bb764609355101fbce07ab1.jpg
Moved: pic-60-_jpg.rf.4e715308cc8dc7455b767414cda028ab.jpg
Moved: pic-270-_jpg.rf.2a0793533346a7355bbeb34291b4a067.jpg
Moved: pic-88-_jpg.rf.1cb5c1768861244cf01d2c5691bb3e08.jpg
Moved: pic-254-_jpg.rf.2b5c3b2efce3960f4f29319ebaa1d220.jpg
Moved: pic-202-_jpg.rf.8c64ec46a9e120007c12c2e4841c9555.jpg
Moved: pic-288-_jpg.rf.26f8da57a5a023907e5e061dbd0a5632.jpg
Moved: pic-129-_jpg.rf.d307956eee8ac32fbe793335e87c7b67.jpg
Moved: pic-204-_jpg.rf.c3990b25e295bfd6b4605c6305cce37c.jpg
Moved: pic-236-_jpg.rf.34f38065b7233d8b9c03b746ffc9a780.jpg
Moved: pic-50-_jpg.rf.cb41506e84f6cac629bd55e40e329834.jpg
Moved: pic-17-_jpg.rf.0d172b6accedf4c52a3868d9b690d48b.jpg
Moved: pic-257-_jpg.rf.09cb9983a70f1bd7ba096c252b64f909.jpg
Moved: pic-58-_jpg.rf.8f585bdabd7d6e5b0285121867659f37.jpg
Moved: pic-154-_jpg.rf.a9e6b534da24b1c1815902210ab23be9.jpg
Moved: pic-303-_jpg.rf.236ed95889a91baf47b304faa7cbae01.jpg
Moved: pic-184-_jpg.rf.cb753b5f714073fc4a8c2de602386399.jpg
Moved: pic-157-_jpg.rf.2247b000d655232fbf8a58b5add102ca.jpg
Moved: pic-69-_jpg.rf.0fcb6cd22beb140d931a387036b7eab6.jpg
Moved: pic-263-_jpg.rf.47073e3fbc426b15c3caa7e8daa66719.jpg
Moved: pic-209-_jpg.rf.533a84bcc43e29e16c0f80069ee7f8df.jpg
Moved: pic-271-_jpg.rf.0210435cf32159dca447e61250afb67f.jpg
All images have been moved successfully.

```

**MAKING LABELS FOR VALID FOLDER**

```python
import os
import pandas as pd
import yaml
from PIL import Image

# Define paths for the dataset
csv_path = '/content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/_annotations.csv'  # Path to your CSV file
images_dir = '/content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images'  # Directory where images are stored
labels_dir = '/content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/labels'  # Directory to save YOLO labels
train_images_path = '/content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/train/images'
val_images_path = '/content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images'
yaml_path = '/content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/dataset.yaml'

# Ensure the labels directory exists
os.makedirs(labels_dir, exist_ok=True)

# Load CSV file
df = pd.read_csv(csv_path)

# Define class mappings
class_mapping = {"Pothole": 0}  # YOLO requires class ids; assign 0 for Pothole

# Helper function to convert bounding boxes to YOLO format
def convert_bbox_to_yolo(img_width, img_height, xmin, ymin, xmax, ymax):
    dw = 1. / img_width
    dh = 1. / img_height
    x_center = (xmin + xmax) / 2.0 * dw
    y_center = (ymin + ymax) / 2.0 * dh
    width = (xmax - xmin) * dw
    height = (ymax - ymin) * dh
    return (x_center, y_center, width, height)

# Convert annotations in the CSV to YOLO format
for index, row in df.iterrows():
    # Get the image name and path
    image_name = row['filename']  # Update if your CSV uses a different column name for the image file name
    image_path = os.path.join(images_dir, image_name)

    # Ensure the image exists
    if not os.path.exists(image_path):
        print(f"Image {image_path} not found. Skipping.")
        continue

    # Read image dimensions
    img = Image.open(image_path)
    img_width, img_height = img.size

    # Extract bounding box details
    xmin, ymin, xmax, ymax = row['xmin'], row['ymin'], row['xmax'], row['ymax']
    class_id = class_mapping.get(row['class'], 0)  # Map class to a numeric ID

    # Convert to YOLO format
    x_center, y_center, width, height = convert_bbox_to_yolo(img_width, img_height, xmin, ymin, xmax, ymax)

    # Save YOLO annotation
    label_file = os.path.join(labels_dir, os.path.splitext(image_name)[0] + '.txt')
    with open(label_file, 'a') as f:  # 'a' mode appends for multiple objects per image
        f.write(f"{class_id} {x_center} {y_center} {width} {height}\n")

print("YOLO annotations generated successfully.")

# Create the dataset.yaml file
data_config = {
    'train': train_images_path,
    'val': val_images_path,
    'names': {i: name for i, name in enumerate(class_mapping.keys())}
}

# Save the configuration to dataset.yaml
with open(yaml_path, 'w') as f:
    yaml.dump(data_config, f)

print(f"dataset.yaml created at: {yaml_path}")
```

```
YOLO annotations generated successfully.
dataset.yaml created at: /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/dataset.yaml

```

```python
import os
import yaml

# Define the path to the YAML file directly
yaml_file_path = '/content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/dataset.yaml'

# Load and print the contents of the YAML file
with open(yaml_file_path, 'r') as file:
    yaml_content = yaml.load(file, Loader=yaml.FullLoader)
    print(yaml.dump(yaml_content, default_flow_style=False))
```

```
names:
  0: Pothole
train: /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/train/images
val: /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images


```

**PRINTING THE NUMBER OF TRAINING AND VALIDATION IMAGES**

```python
import yaml
from PIL import Image

# Define the base dataset path
dataset_path = '/content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1'  # Update with your actual dataset path

# Set paths for training and validation image sets
train_images_path = os.path.join(dataset_path, 'train', 'images')
valid_images_path = os.path.join(dataset_path, 'valid', 'images')


# Set paths for training and validation image sets
train_images_path = os.path.join(dataset_path, 'train', 'images')
valid_images_path = os.path.join(dataset_path, 'valid', 'images')

# Initialize counters for the number of images
num_train_images = 0
num_valid_images = 0

# Initialize sets to hold the unique sizes of images
train_image_sizes = set()
valid_image_sizes = set()

# Check train images sizes and count
for filename in os.listdir(train_images_path):
    if filename.endswith('.jpg'):
        num_train_images += 1
        image_path = os.path.join(train_images_path, filename)
        with Image.open(image_path) as img:
            train_image_sizes.add(img.size)

# Check validation images sizes and count
for filename in os.listdir(valid_images_path):
    if filename.endswith('.jpg'):
        num_valid_images += 1
        image_path = os.path.join(valid_images_path, filename)
        with Image.open(image_path) as img:
            valid_image_sizes.add(img.size)

# Print the results
print(f"Number of training images: {num_train_images}")
print(f"Number of validation images: {num_valid_images}")

# Check if all images in training set have the same size
if len(train_image_sizes) == 1:
    print(f"All training images have the same size: {train_image_sizes.pop()}")
else:
    print("Training images have varying sizes.")

# Check if all images in validation set have the same size
if len(valid_image_sizes) == 1:
    print(f"All validation images have the same size: {valid_image_sizes.pop()}")
else:
    print("Validation images have varying sizes.")
```

**RANDOM IMAGE SELECTION**

```python
# Set the seed for the random number generator
random.seed(0)

# Create a list of image files
image_files = [f for f in os.listdir(train_images_path) if f.endswith('.jpg')]

# Randomly select 15 images
random_images = random.sample(image_files, 15)

# Create a new figure
plt.figure(figsize=(19, 12))

# Loop through each image and display it in a 3x5 grid
for i, image_file in enumerate(random_images):
    image_path = os.path.join(train_images_path, image_file)
    image = Image.open(image_path)
    plt.subplot(3, 5, i + 1)
    plt.imshow(image)
    plt.axis('off')

# Add a suptitle
plt.suptitle('Random Selection of Dataset Images', fontsize=24)

# Show the plot
plt.tight_layout()
plt.show()

# Deleting unnecessary variable to free up memory
del image_files
```

```
<Figure size 1900x1200 with 15 Axes>
```

**TRAINING THE MODEL**

```python
# Train the model on our custom dataset
model = YOLO('yolov8n.pt')
results = model.train(
    data='/content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/dataset.yaml',     # Path to the dataset configuration file
    epochs=50,              # Number of epochs to train for
    imgsz=640,               # Size of input images as integer
    patience=10,             # Epochs to wait for no observable improvement for early stopping of training
    batch=16,                # Number of images per batch
    optimizer='auto',        # Optimizer to use, choices=[SGD, Adam, Adamax, AdamW, NAdam, RAdam, RMSProp, auto]
    lr0=0.0001,              # Initial learning rate
    lrf=0.01,                # Final learning rate (lr0 * lrf)
    dropout=0.25,            # Use dropout regularization
    device=0,                # Device to run on, i.e. cuda device=0
    seed=42                  # Random seed for reproducibility
)
```

```
Ultralytics 8.3.28 🚀 Python-3.10.12 torch-2.5.0+cu121 CUDA:0 (Tesla T4, 15102MiB)
[34m[1mengine/trainer: [0mtask=detect, mode=train, model=yolov8n.pt, data=/content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/dataset.yaml, epochs=50, time=None, patience=10, batch=16, imgsz=640, save=True, save_period=-1, cache=False, device=0, workers=8, project=None, name=train2, exist_ok=False, pretrained=True, optimizer=auto, verbose=True, seed=42, deterministic=True, single_cls=False, rect=False, cos_lr=False, close_mosaic=10, resume=False, amp=True, fraction=1.0, profile=False, freeze=None, multi_scale=False, overlap_mask=True, mask_ratio=4, dropout=0.25, val=True, split=val, save_json=False, save_hybrid=False, conf=None, iou=0.7, max_det=300, half=False, dnn=False, plots=True, source=None, vid_stride=1, stream_buffer=False, visualize=False, augment=False, agnostic_nms=False, classes=None, retina_masks=False, embed=None, show=False, save_frames=False, save_txt=False, save_conf=False, save_crop=False, show_labels=True, show_conf=True, show_boxes=True, line_width=None, format=torchscript, keras=False, optimize=False, int8=False, dynamic=False, simplify=True, opset=None, workspace=4, nms=False, lr0=0.0001, lrf=0.01, momentum=0.937, weight_decay=0.0005, warmup_epochs=3.0, warmup_momentum=0.8, warmup_bias_lr=0.1, box=7.5, cls=0.5, dfl=1.5, pose=12.0, kobj=1.0, label_smoothing=0.0, nbs=64, hsv_h=0.015, hsv_s=0.7, hsv_v=0.4, degrees=0.0, translate=0.1, scale=0.5, shear=0.0, perspective=0.0, flipud=0.0, fliplr=0.5, bgr=0.0, mosaic=1.0, mixup=0.0, copy_paste=0.0, copy_paste_mode=flip, auto_augment=randaugment, erasing=0.4, crop_fraction=1.0, cfg=None, tracker=botsort.yaml, save_dir=runs/detect/train2
Overriding model.yaml nc=80 with nc=1

                   from  n    params  module                                       arguments                     
  0                  -1  1       464  ultralytics.nn.modules.conv.Conv             [3, 16, 3, 2]                 
  1                  -1  1      4672  ultralytics.nn.modules.conv.Conv             [16, 32, 3, 2]                
  2                  -1  1      7360  ultralytics.nn.modules.block.C2f             [32, 32, 1, True]             
  3                  -1  1     18560  ultralytics.nn.modules.conv.Conv             [32, 64, 3, 2]                
  4                  -1  2     49664  ultralytics.nn.modules.block.C2f             [64, 64, 2, True]             
  5                  -1  1     73984  ultralytics.nn.modules.conv.Conv             [64, 128, 3, 2]               
  6                  -1  2    197632  ultralytics.nn.modules.block.C2f             [128, 128, 2, True]           
  7                  -1  1    295424  ultralytics.nn.modules.conv.Conv             [128, 256, 3, 2]              
  8                  -1  1    460288  ultralytics.nn.modules.block.C2f             [256, 256, 1, True]           
  9                  -1  1    164608  ultralytics.nn.modules.block.SPPF            [256, 256, 5]                 
 10                  -1  1         0  torch.nn.modules.upsampling.Upsample         [None, 2, 'nearest']          
 11             [-1, 6]  1         0  ultralytics.nn.modules.conv.Concat           [1]                           
 12                  -1  1    148224  ultralytics.nn.modules.block.C2f             [384, 128, 1]                 
 13                  -1  1         0  torch.nn.modules.upsampling.Upsample         [None, 2, 'nearest']          
 14             [-1, 4]  1         0  ultralytics.nn.modules.conv.Concat           [1]                           
 15                  -1  1     37248  ultralytics.nn.modules.block.C2f             [192, 64, 1]                  
 16                  -1  1     36992  ultralytics.nn.modules.conv.Conv             [64, 64, 3, 2]                
 17            [-1, 12]  1         0  ultralytics.nn.modules.conv.Concat           [1]                           
 18                  -1  1    123648  ultralytics.nn.modules.block.C2f             [192, 128, 1]                 
 19                  -1  1    147712  ultralytics.nn.modules.conv.Conv             [128, 128, 3, 2]              
 20             [-1, 9]  1         0  ultralytics.nn.modules.conv.Concat           [1]                           
 21                  -1  1    493056  ultralytics.nn.modules.block.C2f             [384, 256, 1]                 
 22        [15, 18, 21]  1    751507  ultralytics.nn.modules.head.Detect           [1, [64, 128, 256]]           
Model summary: 225 layers, 3,011,043 parameters, 3,011,027 gradients, 8.2 GFLOPs

Transferred 319/355 items from pretrained weights
[34m[1mTensorBoard: [0mStart with 'tensorboard --logdir runs/detect/train2', view at http://localhost:6006/
Freezing layer 'model.22.dfl.conv.weight'
[34m[1mAMP: [0mrunning Automatic Mixed Precision (AMP) checks...
[34m[1mAMP: [0mchecks passed ✅

```

```
[34m[1mtrain: [0mScanning /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/train/labels.cache... 720 images, 0 backgrounds, 0 corrupt: 100%|██████████| 720/720 [00:00<?, ?it/s]
```

```
[34m[1malbumentations: [0mBlur(p=0.01, blur_limit=(3, 7)), MedianBlur(p=0.01, blur_limit=(3, 7)), ToGray(p=0.01, num_output_channels=3, method='weighted_average'), CLAHE(p=0.01, clip_limit=(1.0, 4.0), tile_grid_size=(8, 8))

```

```

[34m[1mval: [0mScanning /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/labels.cache... 60 images, 0 backgrounds, 0 corrupt: 100%|██████████| 60/60 [00:00<?, ?it/s]
```

```
[34m[1mval: [0mWARNING ⚠️ /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-114-_jpg.rf.a0f30e06b3b96d7879d5f55a7012433c.jpg: 1 duplicate labels removed
[34m[1mval: [0mWARNING ⚠️ /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-116-_jpg.rf.ddcb9d0e0bcf2a1a5096c4f04e6b7f9e.jpg: 10 duplicate labels removed
[34m[1mval: [0mWARNING ⚠️ /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-123-_jpg.rf.385ae3fbcdabda81f72ddf11f6a4b93d.jpg: 1 duplicate labels removed
[34m[1mval: [0mWARNING ⚠️ /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-125-_jpg.rf.3d316e9144cb7438021e01065de91057.jpg: 9 duplicate labels removed
[34m[1mval: [0mWARNING ⚠️ /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-129-_jpg.rf.d307956eee8ac32fbe793335e87c7b67.jpg: 1 duplicate labels removed
[34m[1mval: [0mWARNING ⚠️ /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-140-_jpg.rf.430bfe74decf2b904377d127914f2092.jpg: 5 duplicate labels removed
[34m[1mval: [0mWARNING ⚠️ /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-144-_jpg.rf.61a3b886f058ed3a4788426cfa7c4988.jpg: 1 duplicate labels removed
[34m[1mval: [0mWARNING ⚠️ /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-151-_jpg.rf.45a82558c583efe9dda4ea02e294595a.jpg: 1 duplicate labels removed
[34m[1mval: [0mWARNING ⚠️ /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-152-_jpg.rf.510fb0040c8523bb66ec10b0fe67b4b4.jpg: 15 duplicate labels removed
[34m[1mval: [0mWARNING ⚠️ /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-154-_jpg.rf.a9e6b534da24b1c1815902210ab23be9.jpg: 1 duplicate labels removed
[34m[1mval: [0mWARNING ⚠️ /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-157-_jpg.rf.2247b000d655232fbf8a58b5add102ca.jpg: 14 duplicate labels removed
[34m[1mval: [0mWARNING ⚠️ /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-161-_jpg.rf.1cff77d21f54b7ed9234e896abcf0f5b.jpg: 1 duplicate labels removed
[34m[1mval: [0mWARNING ⚠️ /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-165-_jpg.rf.82b3db37518b15aa73be6e4093deaf46.jpg: 1 duplicate labels removed
[34m[1mval: [0mWARNING ⚠️ /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-17-_jpg.rf.0d172b6accedf4c52a3868d9b690d48b.jpg: 2 duplicate labels removed
[34m[1mval: [0mWARNING ⚠️ /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-173-_jpg.rf.73512294c1b7b5c500eac27a0fb669f7.jpg: 2 duplicate labels removed
[34m[1mval: [0mWARNING ⚠️ /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-175-_jpg.rf.9fc746d4865c11f38047cf383baa30a6.jpg: 2 duplicate labels removed
[34m[1mval: [0mWARNING ⚠️ /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-178-_jpg.rf.2e27d006aec1544f1eec88d9170fd6ce.jpg: 2 duplicate labels removed
[34m[1mval: [0mWARNING ⚠️ /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-183-_jpg.rf.277cfed19f046acc63dc9640b239f1df.jpg: 1 duplicate labels removed
[34m[1mval: [0mWARNING ⚠️ /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-184-_jpg.rf.cb753b5f714073fc4a8c2de602386399.jpg: 8 duplicate labels removed
[34m[1mval: [0mWARNING ⚠️ /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-192-_jpg.rf.e0b55409488785e7156677026d372c23.jpg: 1 duplicate labels removed
[34m[1mval: [0mWARNING ⚠️ /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-193-_jpg.rf.4520ff34079afc8e9f9b50a633c08876.jpg: 1 duplicate labels removed
[34m[1mval: [0mWARNING ⚠️ /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-20-_jpg.rf.4b34591f154f226347c9ca9dfb33b2e4.jpg: 4 duplicate labels removed
[34m[1mval: [0mWARNING ⚠️ /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-202-_jpg.rf.8c64ec46a9e120007c12c2e4841c9555.jpg: 1 duplicate labels removed
[34m[1mval: [0mWARNING ⚠️ /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-204-_jpg.rf.c3990b25e295bfd6b4605c6305cce37c.jpg: 5 duplicate labels removed
[34m[1mval: [0mWARNING ⚠️ /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-205-_jpg.rf.cf4be807bced55552b98c208585d2c56.jpg: 2 duplicate labels removed
[34m[1mval: [0mWARNING ⚠️ /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-209-_jpg.rf.533a84bcc43e29e16c0f80069ee7f8df.jpg: 3 duplicate labels removed
[34m[1mval: [0mWARNING ⚠️ /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-22-_jpg.rf.aec225ee7ab2b5f7791d6579b213600b.jpg: 1 duplicate labels removed
[34m[1mval: [0mWARNING ⚠️ /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-225-_jpg.rf.38cc0deddb897c98814f644451130bb7.jpg: 1 duplicate labels removed
[34m[1mval: [0mWARNING ⚠️ /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-228-_jpg.rf.4dcc6aa7dfc0c9a59a7f033e2ed12413.jpg: 1 duplicate labels removed
[34m[1mval: [0mWARNING ⚠️ /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-230-_jpg.rf.ffe557c4b95e23f1a4323cf7768060f2.jpg: 4 duplicate labels removed
[34m[1mval: [0mWARNING ⚠️ /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-236-_jpg.rf.34f38065b7233d8b9c03b746ffc9a780.jpg: 1 duplicate labels removed
[34m[1mval: [0mWARNING ⚠️ /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-254-_jpg.rf.2b5c3b2efce3960f4f29319ebaa1d220.jpg: 3 duplicate labels removed
[34m[1mval: [0mWARNING ⚠️ /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-257-_jpg.rf.09cb9983a70f1bd7ba096c252b64f909.jpg: 1 duplicate labels removed
[34m[1mval: [0mWARNING ⚠️ /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-262-_jpg.rf.02970860794f859699c9f743bc0fd7d1.jpg: 2 duplicate labels removed
[34m[1mval: [0mWARNING ⚠️ /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-263-_jpg.rf.47073e3fbc426b15c3caa7e8daa66719.jpg: 1 duplicate labels removed
[34m[1mval: [0mWARNING ⚠️ /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-269-_jpg.rf.196b54c0db633b6b02612f69072abb99.jpg: 1 duplicate labels removed
[34m[1mval: [0mWARNING ⚠️ /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-27-_jpg.rf.b4cd8eb26d6941eabfc17280f03bca69.jpg: 8 duplicate labels removed
[34m[1mval: [0mWARNING ⚠️ /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-270-_jpg.rf.2a0793533346a7355bbeb34291b4a067.jpg: 1 duplicate labels removed
[34m[1mval: [0mWARNING ⚠️ /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-271-_jpg.rf.0210435cf32159dca447e61250afb67f.jpg: 4 duplicate labels removed
[34m[1mval: [0mWARNING ⚠️ /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-273-_jpg.rf.36d10c68fb23799bd0a58e48e0b995ce.jpg: 1 duplicate labels removed
[34m[1mval: [0mWARNING ⚠️ /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-28-_jpg.rf.fe8316c392940899d9211be3305c9ab6.jpg: 5 duplicate labels removed
[34m[1mval: [0mWARNING ⚠️ /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-288-_jpg.rf.26f8da57a5a023907e5e061dbd0a5632.jpg: 1 duplicate labels removed
[34m[1mval: [0mWARNING ⚠️ /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-290-_jpg.rf.bcf58ab867c40a607759aec5666fece4.jpg: 9 duplicate labels removed
[34m[1mval: [0mWARNING ⚠️ /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-292-_jpg.rf.f3d0a40ac5190529f4dd4886d6f5e5d0.jpg: 1 duplicate labels removed
[34m[1mval: [0mWARNING ⚠️ /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-303-_jpg.rf.236ed95889a91baf47b304faa7cbae01.jpg: 1 duplicate labels removed
[34m[1mval: [0mWARNING ⚠️ /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-308-_jpg.rf.8f5b6dc0b616365d05bce17bf30eff39.jpg: 2 duplicate labels removed
[34m[1mval: [0mWARNING ⚠️ /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-33-_jpg.rf.143c56d136e3245555b26b4d5108a4e1.jpg: 3 duplicate labels removed
[34m[1mval: [0mWARNING ⚠️ /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-36-_jpg.rf.13a668c4003681c4631508465eef5a9f.jpg: 15 duplicate labels removed
[34m[1mval: [0mWARNING ⚠️ /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-42-_jpg.rf.28b626ac5e887c92feeed1a3c5e85b64.jpg: 5 duplicate labels removed
[34m[1mval: [0mWARNING ⚠️ /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-45-_jpg.rf.8e102a986584d47797dc92558c2af624.jpg: 1 duplicate labels removed
[34m[1mval: [0mWARNING ⚠️ /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-50-_jpg.rf.cb41506e84f6cac629bd55e40e329834.jpg: 2 duplicate labels removed
[34m[1mval: [0mWARNING ⚠️ /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-58-_jpg.rf.8f585bdabd7d6e5b0285121867659f37.jpg: 1 duplicate labels removed
[34m[1mval: [0mWARNING ⚠️ /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-60-_jpg.rf.4e715308cc8dc7455b767414cda028ab.jpg: 2 duplicate labels removed
[34m[1mval: [0mWARNING ⚠️ /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-61-_jpg.rf.72ad391fcf2334c24de5ed48dda25001.jpg: 1 duplicate labels removed
[34m[1mval: [0mWARNING ⚠️ /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-67-_jpg.rf.663b4f930bb764609355101fbce07ab1.jpg: 1 duplicate labels removed
[34m[1mval: [0mWARNING ⚠️ /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-69-_jpg.rf.0fcb6cd22beb140d931a387036b7eab6.jpg: 11 duplicate labels removed
[34m[1mval: [0mWARNING ⚠️ /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-72-_jpg.rf.82c8314917ff5284106bd3428cff5792.jpg: 1 duplicate labels removed
[34m[1mval: [0mWARNING ⚠️ /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-88-_jpg.rf.1cb5c1768861244cf01d2c5691bb3e08.jpg: 5 duplicate labels removed
[34m[1mval: [0mWARNING ⚠️ /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-95-_jpg.rf.eca25439e9e1dd31f29df105f4faa122.jpg: 4 duplicate labels removed
[34m[1mval: [0mWARNING ⚠️ /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-99-_jpg.rf.28d287fa96c09a12f2511e1b4df7e5a1.jpg: 5 duplicate labels removed

```

```


```

```
Plotting labels to runs/detect/train2/labels.jpg... 
[34m[1moptimizer:[0m 'optimizer=auto' found, ignoring 'lr0=0.0001' and 'momentum=0.937' and determining best 'optimizer', 'lr0' and 'momentum' automatically... 
[34m[1moptimizer:[0m AdamW(lr=0.002, momentum=0.9) with parameter groups 57 weight(decay=0.0), 64 weight(decay=0.0005), 63 bias(decay=0.0)
[34m[1mTensorBoard: [0mmodel graph visualization added ✅
Image sizes 640 train, 640 val
Using 2 dataloader workers
Logging results to [1mruns/detect/train2[0m
Starting training for 50 epochs...

      Epoch    GPU_mem   box_loss   cls_loss   dfl_loss  Instances       Size

```

```
       1/50      4.78G      1.502      2.398      1.485         77        640: 100%|██████████| 45/45 [00:19<00:00,  2.30it/s]
                 Class     Images  Instances      Box(P          R      mAP50  mAP50-95): 100%|██████████| 2/2 [00:00<00:00,  2.51it/s]
```

```
                   all         60        201       0.73     0.0896      0.281      0.133

```

```


```

```

      Epoch    GPU_mem   box_loss   cls_loss   dfl_loss  Instances       Size

```

```
       2/50       2.4G      1.502      1.904      1.491         51        640: 100%|██████████| 45/45 [00:17<00:00,  2.54it/s]
                 Class     Images  Instances      Box(P          R      mAP50  mAP50-95): 100%|██████████| 2/2 [00:01<00:00,  1.56it/s]
```

```
                   all         60        201      0.208      0.179      0.115      0.047

```

```


```

```

      Epoch    GPU_mem   box_loss   cls_loss   dfl_loss  Instances       Size

```

```
       3/50       2.4G      1.553      1.908      1.556         79        640: 100%|██████████| 45/45 [00:17<00:00,  2.52it/s]
                 Class     Images  Instances      Box(P          R      mAP50  mAP50-95): 100%|██████████| 2/2 [00:00<00:00,  2.46it/s]
```

```
                   all         60        201      0.428      0.383      0.329       0.12

```

```


```

```

      Epoch    GPU_mem   box_loss   cls_loss   dfl_loss  Instances       Size

```

```
       4/50      2.46G      1.559       1.76      1.511         80        640: 100%|██████████| 45/45 [00:17<00:00,  2.51it/s]
                 Class     Images  Instances      Box(P          R      mAP50  mAP50-95): 100%|██████████| 2/2 [00:00<00:00,  2.12it/s]
```

```
                   all         60        201      0.219      0.224      0.173     0.0703

```

```


```

```

      Epoch    GPU_mem   box_loss   cls_loss   dfl_loss  Instances       Size

```

```
       5/50      2.42G      1.528      1.709       1.52         43        640: 100%|██████████| 45/45 [00:17<00:00,  2.52it/s]
                 Class     Images  Instances      Box(P          R      mAP50  mAP50-95): 100%|██████████| 2/2 [00:00<00:00,  2.93it/s]
```

```
                   all         60        201      0.564      0.328      0.331      0.153

```

```


```

```

      Epoch    GPU_mem   box_loss   cls_loss   dfl_loss  Instances       Size

```

```
       6/50      2.42G      1.527      1.632      1.537         68        640: 100%|██████████| 45/45 [00:18<00:00,  2.49it/s]
                 Class     Images  Instances      Box(P          R      mAP50  mAP50-95): 100%|██████████| 2/2 [00:00<00:00,  2.88it/s]
```

```
                   all         60        201      0.547      0.592      0.547      0.288

```

```


```

```

      Epoch    GPU_mem   box_loss   cls_loss   dfl_loss  Instances       Size

```

```
       7/50       2.4G      1.489      1.565      1.497         78        640: 100%|██████████| 45/45 [00:19<00:00,  2.37it/s]
                 Class     Images  Instances      Box(P          R      mAP50  mAP50-95): 100%|██████████| 2/2 [00:00<00:00,  2.70it/s]
```

```
                   all         60        201      0.422      0.597      0.473      0.233

```

```


```

```

      Epoch    GPU_mem   box_loss   cls_loss   dfl_loss  Instances       Size

```

```
       8/50      2.45G      1.464       1.49      1.452         50        640: 100%|██████████| 45/45 [00:17<00:00,  2.64it/s]
                 Class     Images  Instances      Box(P          R      mAP50  mAP50-95): 100%|██████████| 2/2 [00:00<00:00,  2.51it/s]
```

```
                   all         60        201      0.536      0.468      0.438      0.206

```

```


```

```

      Epoch    GPU_mem   box_loss   cls_loss   dfl_loss  Instances       Size

```

```
       9/50       2.4G      1.439       1.45      1.448         79        640: 100%|██████████| 45/45 [00:17<00:00,  2.59it/s]
                 Class     Images  Instances      Box(P          R      mAP50  mAP50-95): 100%|██████████| 2/2 [00:00<00:00,  2.87it/s]
```

```
                   all         60        201      0.562      0.567      0.583      0.295

```

```


```

```

      Epoch    GPU_mem   box_loss   cls_loss   dfl_loss  Instances       Size

```

```
      10/50       2.4G      1.397       1.38      1.435         80        640: 100%|██████████| 45/45 [00:22<00:00,  2.03it/s]
                 Class     Images  Instances      Box(P          R      mAP50  mAP50-95): 100%|██████████| 2/2 [00:01<00:00,  1.29it/s]
```

```
                   all         60        201      0.658      0.518      0.556        0.3

```

```


```

```

      Epoch    GPU_mem   box_loss   cls_loss   dfl_loss  Instances       Size

```

```
      11/50       2.4G      1.423       1.36      1.441         69        640: 100%|██████████| 45/45 [00:17<00:00,  2.63it/s]
                 Class     Images  Instances      Box(P          R      mAP50  mAP50-95): 100%|██████████| 2/2 [00:01<00:00,  1.59it/s]
```

```
                   all         60        201      0.559      0.617      0.606      0.317

```

```


```

```

      Epoch    GPU_mem   box_loss   cls_loss   dfl_loss  Instances       Size

```

```
      12/50       2.4G      1.362      1.319      1.405         63        640: 100%|██████████| 45/45 [00:16<00:00,  2.66it/s]
                 Class     Images  Instances      Box(P          R      mAP50  mAP50-95): 100%|██████████| 2/2 [00:01<00:00,  1.19it/s]
```

```
                   all         60        201       0.61      0.617      0.585      0.307

```

```


```

```

      Epoch    GPU_mem   box_loss   cls_loss   dfl_loss  Instances       Size

```

```
      13/50      2.43G       1.39      1.307      1.397         77        640: 100%|██████████| 45/45 [00:17<00:00,  2.52it/s]
                 Class     Images  Instances      Box(P          R      mAP50  mAP50-95): 100%|██████████| 2/2 [00:00<00:00,  3.10it/s]
```

```
                   all         60        201      0.669      0.582      0.617      0.322

```

```


```

```

      Epoch    GPU_mem   box_loss   cls_loss   dfl_loss  Instances       Size

```

```
      14/50       2.4G       1.35      1.273      1.391         65        640: 100%|██████████| 45/45 [00:18<00:00,  2.42it/s]
                 Class     Images  Instances      Box(P          R      mAP50  mAP50-95): 100%|██████████| 2/2 [00:00<00:00,  2.67it/s]
```

```
                   all         60        201      0.644      0.558      0.602      0.341

```

```


```

```

      Epoch    GPU_mem   box_loss   cls_loss   dfl_loss  Instances       Size

```

```
      15/50      2.42G      1.334      1.234      1.377         74        640: 100%|██████████| 45/45 [00:18<00:00,  2.40it/s]
                 Class     Images  Instances      Box(P          R      mAP50  mAP50-95): 100%|██████████| 2/2 [00:00<00:00,  2.04it/s]
```

```
                   all         60        201      0.577      0.618      0.621      0.353

```

```


```

```

      Epoch    GPU_mem   box_loss   cls_loss   dfl_loss  Instances       Size

```

```
      16/50       2.4G      1.313      1.192      1.351         70        640: 100%|██████████| 45/45 [00:19<00:00,  2.35it/s]
                 Class     Images  Instances      Box(P          R      mAP50  mAP50-95): 100%|██████████| 2/2 [00:00<00:00,  2.70it/s]
```

```
                   all         60        201      0.695      0.562      0.642      0.349

```

```


```

```

      Epoch    GPU_mem   box_loss   cls_loss   dfl_loss  Instances       Size

```

```
      17/50       2.4G      1.313      1.207      1.369         61        640: 100%|██████████| 45/45 [00:17<00:00,  2.51it/s]
                 Class     Images  Instances      Box(P          R      mAP50  mAP50-95): 100%|██████████| 2/2 [00:00<00:00,  2.72it/s]
```

```
                   all         60        201      0.704      0.617      0.689      0.377

```

```


```

```

      Epoch    GPU_mem   box_loss   cls_loss   dfl_loss  Instances       Size

```

```
      18/50       2.4G      1.299       1.19      1.361         60        640: 100%|██████████| 45/45 [00:18<00:00,  2.39it/s]
                 Class     Images  Instances      Box(P          R      mAP50  mAP50-95): 100%|██████████| 2/2 [00:00<00:00,  3.06it/s]
```

```
                   all         60        201      0.636      0.647      0.627      0.357

```

```


```

```

      Epoch    GPU_mem   box_loss   cls_loss   dfl_loss  Instances       Size

```

```
      19/50       2.4G      1.266      1.123      1.342         57        640: 100%|██████████| 45/45 [00:17<00:00,  2.53it/s]
                 Class     Images  Instances      Box(P          R      mAP50  mAP50-95): 100%|██████████| 2/2 [00:01<00:00,  1.96it/s]
```

```
                   all         60        201      0.649      0.607      0.631      0.351

```

```


```

```

      Epoch    GPU_mem   box_loss   cls_loss   dfl_loss  Instances       Size

```

```
      20/50      2.43G      1.256      1.104      1.335         62        640: 100%|██████████| 45/45 [00:18<00:00,  2.47it/s]
                 Class     Images  Instances      Box(P          R      mAP50  mAP50-95): 100%|██████████| 2/2 [00:00<00:00,  2.13it/s]
```

```
                   all         60        201      0.638      0.641      0.658      0.371

```

```


```

```

      Epoch    GPU_mem   box_loss   cls_loss   dfl_loss  Instances       Size

```

```
      21/50      2.46G      1.252      1.125      1.324         62        640: 100%|██████████| 45/45 [00:18<00:00,  2.47it/s]
                 Class     Images  Instances      Box(P          R      mAP50  mAP50-95): 100%|██████████| 2/2 [00:01<00:00,  1.80it/s]
```

```
                   all         60        201      0.681      0.607      0.647      0.371

```

```


```

```

      Epoch    GPU_mem   box_loss   cls_loss   dfl_loss  Instances       Size

```

```
      22/50      2.42G      1.213      1.059      1.287         67        640: 100%|██████████| 45/45 [00:17<00:00,  2.53it/s]
                 Class     Images  Instances      Box(P          R      mAP50  mAP50-95): 100%|██████████| 2/2 [00:01<00:00,  1.75it/s]
```

```
                   all         60        201      0.674      0.637      0.658      0.384

```

```


```

```

      Epoch    GPU_mem   box_loss   cls_loss   dfl_loss  Instances       Size

```

```
      23/50       2.4G      1.229      1.056      1.283         81        640: 100%|██████████| 45/45 [00:18<00:00,  2.45it/s]
                 Class     Images  Instances      Box(P          R      mAP50  mAP50-95): 100%|██████████| 2/2 [00:01<00:00,  1.14it/s]
```

```
                   all         60        201      0.606      0.711      0.665      0.363

```

```


```

```

      Epoch    GPU_mem   box_loss   cls_loss   dfl_loss  Instances       Size

```

```
      24/50      2.42G      1.208      1.009      1.286         61        640: 100%|██████████| 45/45 [00:17<00:00,  2.60it/s]
                 Class     Images  Instances      Box(P          R      mAP50  mAP50-95): 100%|██████████| 2/2 [00:01<00:00,  1.30it/s]
```

```
                   all         60        201      0.692      0.592      0.648      0.378

```

```


```

```

      Epoch    GPU_mem   box_loss   cls_loss   dfl_loss  Instances       Size

```

```
      25/50       2.4G      1.177      1.014      1.289         62        640: 100%|██████████| 45/45 [00:18<00:00,  2.48it/s]
                 Class     Images  Instances      Box(P          R      mAP50  mAP50-95): 100%|██████████| 2/2 [00:01<00:00,  1.07it/s]
```

```
                   all         60        201       0.61      0.662      0.666      0.378

```

```


```

```

      Epoch    GPU_mem   box_loss   cls_loss   dfl_loss  Instances       Size

```

```
      26/50       2.4G      1.171     0.9726      1.277         31        640: 100%|██████████| 45/45 [00:18<00:00,  2.42it/s]
                 Class     Images  Instances      Box(P          R      mAP50  mAP50-95): 100%|██████████| 2/2 [00:02<00:00,  1.06s/it]
```

```
                   all         60        201      0.627      0.702      0.707      0.397

```

```


```

```

      Epoch    GPU_mem   box_loss   cls_loss   dfl_loss  Instances       Size

```

```
      27/50       2.4G      1.186     0.9838      1.276         58        640: 100%|██████████| 45/45 [00:18<00:00,  2.48it/s]
                 Class     Images  Instances      Box(P          R      mAP50  mAP50-95): 100%|██████████| 2/2 [00:00<00:00,  2.32it/s]
```

```
                   all         60        201      0.645      0.642       0.63       0.35

```

```


```

```

      Epoch    GPU_mem   box_loss   cls_loss   dfl_loss  Instances       Size

```

```
      28/50       2.4G      1.149     0.9449      1.264         75        640: 100%|██████████| 45/45 [00:18<00:00,  2.41it/s]
                 Class     Images  Instances      Box(P          R      mAP50  mAP50-95): 100%|██████████| 2/2 [00:00<00:00,  2.14it/s]
```

```
                   all         60        201      0.705       0.69      0.706      0.393

```

```


```

```

      Epoch    GPU_mem   box_loss   cls_loss   dfl_loss  Instances       Size

```

```
      29/50      2.42G       1.16     0.9383      1.251         63        640: 100%|██████████| 45/45 [00:17<00:00,  2.56it/s]
                 Class     Images  Instances      Box(P          R      mAP50  mAP50-95): 100%|██████████| 2/2 [00:01<00:00,  1.99it/s]
```

```
                   all         60        201      0.764      0.572      0.665      0.393

```

```


```

```

      Epoch    GPU_mem   box_loss   cls_loss   dfl_loss  Instances       Size

```

```
      30/50      2.45G      1.105     0.9163       1.22         62        640: 100%|██████████| 45/45 [00:18<00:00,  2.43it/s]
                 Class     Images  Instances      Box(P          R      mAP50  mAP50-95): 100%|██████████| 2/2 [00:00<00:00,  2.79it/s]
```

```
                   all         60        201      0.712      0.627      0.684      0.412

```

```


```

```

      Epoch    GPU_mem   box_loss   cls_loss   dfl_loss  Instances       Size

```

```
      31/50      2.42G      1.119     0.9104      1.222         94        640: 100%|██████████| 45/45 [00:18<00:00,  2.48it/s]
                 Class     Images  Instances      Box(P          R      mAP50  mAP50-95): 100%|██████████| 2/2 [00:02<00:00,  1.02s/it]
```

```
                   all         60        201      0.656      0.722      0.689       0.39

```

```


```

```

      Epoch    GPU_mem   box_loss   cls_loss   dfl_loss  Instances       Size

```

```
      32/50      2.42G      1.122     0.8891      1.235         51        640: 100%|██████████| 45/45 [00:17<00:00,  2.54it/s]
                 Class     Images  Instances      Box(P          R      mAP50  mAP50-95): 100%|██████████| 2/2 [00:00<00:00,  2.53it/s]
```

```
                   all         60        201      0.727      0.637      0.695      0.393

```

```


```

```

      Epoch    GPU_mem   box_loss   cls_loss   dfl_loss  Instances       Size

```

```
      33/50      2.42G      1.103     0.8865      1.215         78        640: 100%|██████████| 45/45 [00:18<00:00,  2.45it/s]
                 Class     Images  Instances      Box(P          R      mAP50  mAP50-95): 100%|██████████| 2/2 [00:00<00:00,  2.11it/s]
```

```
                   all         60        201      0.708      0.687       0.71      0.419

```

```


```

```

      Epoch    GPU_mem   box_loss   cls_loss   dfl_loss  Instances       Size

```

```
      34/50      2.42G      1.076     0.8429      1.206         63        640: 100%|██████████| 45/45 [00:18<00:00,  2.50it/s]
                 Class     Images  Instances      Box(P          R      mAP50  mAP50-95): 100%|██████████| 2/2 [00:00<00:00,  2.46it/s]
```

```
                   all         60        201       0.75      0.662      0.713      0.413

```

```


```

```

      Epoch    GPU_mem   box_loss   cls_loss   dfl_loss  Instances       Size

```

```
      35/50       2.4G      1.074     0.8391      1.205         81        640: 100%|██████████| 45/45 [00:18<00:00,  2.48it/s]
                 Class     Images  Instances      Box(P          R      mAP50  mAP50-95): 100%|██████████| 2/2 [00:01<00:00,  1.89it/s]
```

```
                   all         60        201       0.76      0.632      0.709      0.417

```

```


```

```

      Epoch    GPU_mem   box_loss   cls_loss   dfl_loss  Instances       Size

```

```
      36/50      2.42G      1.084     0.8326      1.203         90        640: 100%|██████████| 45/45 [00:17<00:00,  2.56it/s]
                 Class     Images  Instances      Box(P          R      mAP50  mAP50-95): 100%|██████████| 2/2 [00:00<00:00,  2.67it/s]
```

```
                   all         60        201      0.714      0.672      0.702      0.419

```

```


```

```

      Epoch    GPU_mem   box_loss   cls_loss   dfl_loss  Instances       Size

```

```
      37/50       2.4G      1.081     0.8295      1.197         55        640: 100%|██████████| 45/45 [00:17<00:00,  2.52it/s]
                 Class     Images  Instances      Box(P          R      mAP50  mAP50-95): 100%|██████████| 2/2 [00:00<00:00,  3.04it/s]
```

```
                   all         60        201      0.713      0.666      0.672      0.397

```

```


```

```

      Epoch    GPU_mem   box_loss   cls_loss   dfl_loss  Instances       Size

```

```
      38/50      2.42G      1.011     0.7808      1.166         75        640: 100%|██████████| 45/45 [00:17<00:00,  2.50it/s]
                 Class     Images  Instances      Box(P          R      mAP50  mAP50-95): 100%|██████████| 2/2 [00:01<00:00,  1.71it/s]
```

```
                   all         60        201      0.733      0.613      0.703      0.417

```

```


```

```

      Epoch    GPU_mem   box_loss   cls_loss   dfl_loss  Instances       Size

```

```
      39/50       2.4G      1.025      0.779      1.176         68        640: 100%|██████████| 45/45 [00:17<00:00,  2.61it/s]
                 Class     Images  Instances      Box(P          R      mAP50  mAP50-95): 100%|██████████| 2/2 [00:01<00:00,  1.42it/s]
```

```
                   all         60        201      0.694      0.672      0.688      0.408

```

```


```

```

      Epoch    GPU_mem   box_loss   cls_loss   dfl_loss  Instances       Size

```

```
      40/50      2.42G     0.9952     0.7621      1.162         80        640: 100%|██████████| 45/45 [00:19<00:00,  2.36it/s]
                 Class     Images  Instances      Box(P          R      mAP50  mAP50-95): 100%|██████████| 2/2 [00:01<00:00,  1.54it/s]
```

```
                   all         60        201      0.731      0.701      0.726      0.426

```

```


```

```
Closing dataloader mosaic
[34m[1malbumentations: [0mBlur(p=0.01, blur_limit=(3, 7)), MedianBlur(p=0.01, blur_limit=(3, 7)), ToGray(p=0.01, num_output_channels=3, method='weighted_average'), CLAHE(p=0.01, clip_limit=(1.0, 4.0), tile_grid_size=(8, 8))

      Epoch    GPU_mem   box_loss   cls_loss   dfl_loss  Instances       Size

```

```
      41/50       2.4G     0.9482     0.6759      1.121         47        640: 100%|██████████| 45/45 [00:19<00:00,  2.36it/s]
                 Class     Images  Instances      Box(P          R      mAP50  mAP50-95): 100%|██████████| 2/2 [00:00<00:00,  2.82it/s]
```

```
                   all         60        201      0.762      0.692      0.724      0.425

```

```


```

```

      Epoch    GPU_mem   box_loss   cls_loss   dfl_loss  Instances       Size

```

```
      42/50      2.38G     0.9451     0.6355      1.111         62        640: 100%|██████████| 45/45 [00:17<00:00,  2.61it/s]
                 Class     Images  Instances      Box(P          R      mAP50  mAP50-95): 100%|██████████| 2/2 [00:00<00:00,  2.49it/s]
```

```
                   all         60        201      0.716      0.687       0.71      0.419

```

```


```

```

      Epoch    GPU_mem   box_loss   cls_loss   dfl_loss  Instances       Size

```

```
      43/50      2.42G     0.9185     0.6423      1.097         35        640: 100%|██████████| 45/45 [00:17<00:00,  2.59it/s]
                 Class     Images  Instances      Box(P          R      mAP50  mAP50-95): 100%|██████████| 2/2 [00:00<00:00,  2.94it/s]
```

```
                   all         60        201      0.752      0.678      0.722      0.432

```

```


```

```

      Epoch    GPU_mem   box_loss   cls_loss   dfl_loss  Instances       Size

```

```
      44/50      2.38G     0.8902     0.6011       1.09         31        640: 100%|██████████| 45/45 [00:17<00:00,  2.59it/s]
                 Class     Images  Instances      Box(P          R      mAP50  mAP50-95): 100%|██████████| 2/2 [00:00<00:00,  2.52it/s]
```

```
                   all         60        201      0.733      0.711      0.732      0.444

```

```


```

```

      Epoch    GPU_mem   box_loss   cls_loss   dfl_loss  Instances       Size

```

```
      45/50      2.38G     0.8867     0.5949      1.088         42        640: 100%|██████████| 45/45 [00:16<00:00,  2.69it/s]
                 Class     Images  Instances      Box(P          R      mAP50  mAP50-95): 100%|██████████| 2/2 [00:00<00:00,  2.74it/s]
```

```
                   all         60        201      0.749      0.654      0.703      0.424

```

```


```

```

      Epoch    GPU_mem   box_loss   cls_loss   dfl_loss  Instances       Size

```

```
      46/50      2.44G     0.8628      0.564       1.07         32        640: 100%|██████████| 45/45 [00:17<00:00,  2.63it/s]
                 Class     Images  Instances      Box(P          R      mAP50  mAP50-95): 100%|██████████| 2/2 [00:00<00:00,  2.63it/s]
```

```
                   all         60        201      0.674      0.692      0.694      0.416

```

```


```

```

      Epoch    GPU_mem   box_loss   cls_loss   dfl_loss  Instances       Size

```

```
      47/50       2.4G     0.8489     0.5606      1.048         58        640: 100%|██████████| 45/45 [00:17<00:00,  2.57it/s]
                 Class     Images  Instances      Box(P          R      mAP50  mAP50-95): 100%|██████████| 2/2 [00:00<00:00,  2.67it/s]
```

```
                   all         60        201      0.659      0.721      0.704      0.424

```

```


```

```

      Epoch    GPU_mem   box_loss   cls_loss   dfl_loss  Instances       Size

```

```
      48/50      2.42G     0.8494      0.549      1.053         52        640: 100%|██████████| 45/45 [00:17<00:00,  2.62it/s]
                 Class     Images  Instances      Box(P          R      mAP50  mAP50-95): 100%|██████████| 2/2 [00:00<00:00,  3.03it/s]
```

```
                   all         60        201      0.684      0.721      0.711      0.432

```

```


```

```

      Epoch    GPU_mem   box_loss   cls_loss   dfl_loss  Instances       Size

```

```
      49/50      2.42G     0.8382     0.5449      1.046         54        640: 100%|██████████| 45/45 [00:17<00:00,  2.61it/s]
                 Class     Images  Instances      Box(P          R      mAP50  mAP50-95): 100%|██████████| 2/2 [00:00<00:00,  2.93it/s]
```

```
                   all         60        201      0.672      0.706      0.705       0.43

```

```


```

```

      Epoch    GPU_mem   box_loss   cls_loss   dfl_loss  Instances       Size

```

```
      50/50      2.42G     0.8402     0.5417      1.055         32        640: 100%|██████████| 45/45 [00:16<00:00,  2.68it/s]
                 Class     Images  Instances      Box(P          R      mAP50  mAP50-95): 100%|██████████| 2/2 [00:00<00:00,  2.63it/s]
```

```
                   all         60        201      0.691      0.697      0.713      0.438

```

```


```

```

50 epochs completed in 0.285 hours.
Optimizer stripped from runs/detect/train2/weights/last.pt, 6.2MB
Optimizer stripped from runs/detect/train2/weights/best.pt, 6.2MB

Validating runs/detect/train2/weights/best.pt...
Ultralytics 8.3.28 🚀 Python-3.10.12 torch-2.5.0+cu121 CUDA:0 (Tesla T4, 15102MiB)
Model summary (fused): 168 layers, 3,005,843 parameters, 0 gradients, 8.1 GFLOPs

```

```
                 Class     Images  Instances      Box(P          R      mAP50  mAP50-95): 100%|██████████| 2/2 [00:01<00:00,  1.84it/s]

```

```
                   all         60        201      0.734      0.715      0.731      0.443
Speed: 0.6ms preprocess, 2.8ms inference, 0.0ms loss, 3.1ms postprocess per image
Results saved to [1mruns/detect/train2[0m

```

```python
# Reconfigure locale encoding to UTF-8
import locale
locale.getpreferredencoding = lambda: 'UTF-8'

# Define the path to the directory
post_training_files_path = '/content/drive/MyDrive/pothole_detection_dataset/MyDrive/runs/detect/train2'

# List the files in the directory
!ls {post_training_files_path}
```

```
args.yaml					   PR_curve.png		train_batch1.jpg
confusion_matrix_normalized.png			   R_curve.png		train_batch2.jpg
confusion_matrix.png				   results.csv		val_batch0_labels.jpg
events.out.tfevents.1731238815.c5e05294ecc9.229.2  results.png		val_batch0_pred.jpg
F1_curve.png					   train_batch0.jpg	val_batch1_labels.jpg
labels_correlogram.jpg				   train_batch1800.jpg	val_batch1_pred.jpg
labels.jpg					   train_batch1801.jpg	weights
P_curve.png					   train_batch1802.jpg

```

```python
#Confusion matrix is the chart that shows how our model handles different classes
#68% of the time the model detected correctly that there is a pothole, while 32% of the time, when the pothole is there but the model is not
#able to detect it
%cd {HOME}
from IPython.display import display, Image # Import the 'display' and 'Image' from IPython.display
display(Image(filename=f'/content/drive/MyDrive/pothole_detection_dataset/MyDrive/runs/detect/train2/confusion_matrix.png', width=900)) # Use 'display' function to display the image
```

```
[Errno 2] No such file or directory: '{HOME}'
/content

```

```
<IPython.core.display.Image object>
```

```python
# Here is the graph of the training and validation loss
#box loss and class loss is important
# The behavior of the model is convincing the model is coverging, Training more will give better results
Image(filename=f'/content/drive/MyDrive/pothole_detection_dataset/MyDrive/runs/detect/train2/results.png', width=600)
```

```
<IPython.core.display.Image object>
```

```python
import os
import matplotlib.pyplot as plt
from ultralytics import YOLO
import cv2

# Define paths
valid_images_path = '/content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images'
output_path = '/content/drive/MyDrive/pothole_detection_dataset/MyDrive/runs/detect/train2/val_batch0_pred.jpg'

# Load model
model = YOLO('/content/drive/MyDrive/pothole_detection_dataset/MyDrive/runs/detect/train2/weights/best.pt')

# Get a list of validation images
image_files = [f for f in os.listdir(valid_images_path) if f.endswith('.jpg')]
num_images = min(9, len(image_files))  # Select up to 9 images

# Prepare a figure for a 3x3 grid
fig, axes = plt.subplots(3, 3, figsize=(20, 20))

for i, ax in enumerate(axes.flatten()):
    if i >= num_images:
        break
    # Load and predict on each image
    image_path = os.path.join(valid_images_path, image_files[i])
    results = model.predict(source=image_path, imgsz=640)

    # Retrieve annotated image
    annotated_image = results[0].plot()  # Plot predictions on image
    annotated_image_rgb = cv2.cvtColor(annotated_image, cv2.COLOR_BGR2RGB)  # Convert for matplotlib display

    # Display image in grid
    ax.imshow(annotated_image_rgb)
    ax.axis('off')
    ax.set_title(f"Prediction on {image_files[i]}")

plt.tight_layout()
plt.savefig(output_path)  # Save as a file for future reference
plt.show()

```

```

image 1/1 /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-42-_jpg.rf.28b626ac5e887c92feeed1a3c5e85b64.jpg: 640x640 3 Potholes, 12.8ms
Speed: 7.9ms preprocess, 12.8ms inference, 2.4ms postprocess per image at shape (1, 3, 640, 640)

image 1/1 /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-33-_jpg.rf.143c56d136e3245555b26b4d5108a4e1.jpg: 640x640 5 Potholes, 12.7ms
Speed: 2.0ms preprocess, 12.7ms inference, 1.8ms postprocess per image at shape (1, 3, 640, 640)

image 1/1 /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-273-_jpg.rf.36d10c68fb23799bd0a58e48e0b995ce.jpg: 640x640 4 Potholes, 11.0ms
Speed: 2.0ms preprocess, 11.0ms inference, 2.1ms postprocess per image at shape (1, 3, 640, 640)

image 1/1 /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-114-_jpg.rf.a0f30e06b3b96d7879d5f55a7012433c.jpg: 640x640 1 Pothole, 9.5ms
Speed: 2.7ms preprocess, 9.5ms inference, 1.8ms postprocess per image at shape (1, 3, 640, 640)

image 1/1 /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-290-_jpg.rf.bcf58ab867c40a607759aec5666fece4.jpg: 640x640 14 Potholes, 10.1ms
Speed: 2.8ms preprocess, 10.1ms inference, 1.7ms postprocess per image at shape (1, 3, 640, 640)

image 1/1 /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-183-_jpg.rf.277cfed19f046acc63dc9640b239f1df.jpg: 640x640 1 Pothole, 16.1ms
Speed: 2.7ms preprocess, 16.1ms inference, 1.9ms postprocess per image at shape (1, 3, 640, 640)

image 1/1 /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-151-_jpg.rf.45a82558c583efe9dda4ea02e294595a.jpg: 640x640 2 Potholes, 20.7ms
Speed: 4.4ms preprocess, 20.7ms inference, 2.3ms postprocess per image at shape (1, 3, 640, 640)

image 1/1 /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-228-_jpg.rf.4dcc6aa7dfc0c9a59a7f033e2ed12413.jpg: 640x640 1 Pothole, 18.4ms
Speed: 3.3ms preprocess, 18.4ms inference, 2.3ms postprocess per image at shape (1, 3, 640, 640)

image 1/1 /content/drive/MyDrive/pothole_detection_dataset/MyDrive/Pothole_Segmentation_YOLOv8-1/valid/images/pic-178-_jpg.rf.2e27d006aec1544f1eec88d9170fd6ce.jpg: 640x640 1 Pothole, 11.0ms
Speed: 3.3ms preprocess, 11.0ms inference, 1.7ms postprocess per image at shape (1, 3, 640, 640)

```

```
<Figure size 2000x2000 with 9 Axes>
```

```python
import cv2
import numpy as np
from collections import deque
from ultralytics import YOLO  # Ensure YOLOv8 is installed
from IPython.display import Video

# Define paths for input and output videos
video_path = '/content/drive/MyDrive/Pothole_Segmentation_YOLOv8-1/sample_video.mp4'
output_video_path = '/content/drive/MyDrive/road_damage_assessment.mp4'

# Load the trained model
best_model = YOLO('/content/drive/MyDrive/runs/detect/train2/weights/best.pt')

# Define font and colors for annotation
font = cv2.FONT_HERSHEY_SIMPLEX
font_scale = 1
text_position = (40, 80)
font_color = (255, 255, 255)    # White text
background_color = (255, 0, 0)  # Red background for text

# Initialize a deque for averaging percentage damage across frames
damage_deque = deque(maxlen=10)

# Open the video
cap = cv2.VideoCapture(video_path)
width, height = int(cap.get(3)), int(cap.get(4))

# Define the codec and VideoWriter object for .mp4 output
fourcc = cv2.VideoWriter_fourcc(*'mp4v')
out = cv2.VideoWriter(output_video_path, fourcc, 20.0, (width, height))

# Process video frames
while cap.isOpened():
    ret, frame = cap.read()
    if not ret:
        break

    # Perform detection on the frame
    results = best_model.predict(source=frame, imgsz=640, conf=0.25)

    # Print results to check if predictions are being made
    print(f"Detections: {results[0].boxes}")

    # Process and annotate the frame with bounding boxes
    processed_frame = results[0].plot()

    # Initialize percentage damage
    percentage_damage = 0

    # If masks are available, calculate damage area as a percentage of the frame
    if results[0].masks is not None:
        total_area = 0
        masks = results[0].masks.data.cpu().numpy()
        image_area = frame.shape[0] * frame.shape[1]  # total number of pixels in the image
        for mask in masks:
            binary_mask = (mask > 0).astype(np.uint8) * 255
            contours, _ = cv2.findContours(binary_mask, cv2.RETR_TREE, cv2.CHAIN_APPROX_SIMPLE)
            for contour in contours:
                total_area += cv2.contourArea(contour)

        percentage_damage = (total_area / image_area) * 100

    # Update deque and calculate smoothed damage percentage
    damage_deque.append(percentage_damage)
    smoothed_percentage_damage = sum(damage_deque) / len(damage_deque)

    # Draw a line background and add damage annotation text
    cv2.line(processed_frame, (text_position[0], text_position[1] - 10),
             (text_position[0] + 350, text_position[1] - 10), background_color, 40)
    cv2.putText(processed_frame, f'Road Damage: {smoothed_percentage_damage:.2f}%',
                text_position, font, font_scale, font_color, 2, cv2.LINE_AA)

    # Write the processed frame to the output video
    out.write(processed_frame)

cap.release()
out.release()

# Verify if the file was created and has content
import os
print(f"Output video exists: {os.path.exists(output_video_path)}")
print(f"Output video size: {os.path.getsize(output_video_path)} bytes")

# Display the processed video within the notebook
Video(output_video_path, embed=True, width=960)


# import cv2
# import numpy as np
# from collections import deque
# from ultralytics import YOLO  # Make sure to install YOLOv8
# from IPython.display import Video

# # Define paths for input and output videos
# video_path = '/content/drive/MyDrive/Pothole_Segmentation_YOLOv8-1/sample_video.mp4'
# output_video_path = '/content/drive/MyDrive/road_damage_assessment.mp4'

# # Load the trained model
# best_model = YOLO('/content/drive/MyDrive/runs/detect/train2/weights/best.pt')

# # Define font and colors for annotation
# font = cv2.FONT_HERSHEY_SIMPLEX
# font_scale = 1
# text_position = (40, 80)
# font_color = (255, 255, 255)    # White text
# background_color = (255, 0, 0)  # Red background for text

# # Initialize a deque for averaging percentage damage across frames
# damage_deque = deque(maxlen=10)

# # Open the video
# cap = cv2.VideoCapture(video_path)
# width, height = int(cap.get(3)), int(cap.get(4))

# # Define the codec and VideoWriter object for .mp4 output
# fourcc = cv2.VideoWriter_fourcc(*'mp4v')
# out = cv2.VideoWriter(output_video_path, fourcc, 20.0, (width, height))

# # Process video frames
# while cap.isOpened():
#     ret, frame = cap.read()
#     if not ret:
#         break

#     # Perform detection on the frame
#     results = best_model.predict(source=frame, imgsz=640, conf=0.25)
#     processed_frame = results[0].plot()

#     # Initialize percentage damage
#     percentage_damage = 0

#     # If masks are available, calculate damage area as a percentage of the frame
#     if results[0].masks is not None:
#         total_area = 0
#         masks = results[0].masks.data.cpu().numpy()
#         image_area = frame.shape[0] * frame.shape[1]  # total number of pixels in the image
#         for mask in masks:
#             binary_mask = (mask > 0).astype(np.uint8) * 255
#             contours, _ = cv2.findContours(binary_mask, cv2.RETR_TREE, cv2.CHAIN_APPROX_SIMPLE)
#             for contour in contours:
#                 total_area += cv2.contourArea(contour)

#         percentage_damage = (total_area / image_area) * 100

#     # Update deque and calculate smoothed damage percentage
#     damage_deque.append(percentage_damage)
#     smoothed_percentage_damage = sum(damage_deque) / len(damage_deque)

#     # Draw a line background and add damage annotation text
#     cv2.line(processed_frame, (text_position[0], text_position[1] - 10),
#              (text_position[0] + 350, text_position[1] - 10), background_color, 40)
#     cv2.putText(processed_frame, f'Road Damage: {smoothed_percentage_damage:.2f}%',
#                 text_position, font, font_scale, font_color, 2, cv2.LINE_AA)

#     # Write the processed frame to the output video
#     out.write(processed_frame)

# cap.release()
# out.release()

# # Display the processed video within the notebook
# Video(output_video_path, embed=True, width=960)

```

```
[1;30;43mStreaming output truncated to the last 5000 lines.[0m
0: 384x640 3 Potholes, 17.5ms
Speed: 2.0ms preprocess, 17.5ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0.], device='cuda:0')
conf: tensor([0.6392, 0.6147, 0.5506], device='cuda:0')
data: tensor([[3.3099e+02, 2.3085e+02, 4.3323e+02, 2.5443e+02, 6.3922e-01, 0.0000e+00],
        [4.3321e+02, 3.2016e+02, 6.3630e+02, 3.7039e+02, 6.1467e-01, 0.0000e+00],
        [4.3968e+01, 4.7296e+02, 6.6719e+02, 6.6314e+02, 5.5063e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([3, 6])
xywh: tensor([[382.1117, 242.6402, 102.2442,  23.5713],
        [534.7581, 345.2773, 203.0894,  50.2334],
        [355.5811, 568.0532, 623.2271, 190.1831]], device='cuda:0')
xywhn: tensor([[0.2985, 0.3370, 0.0799, 0.0327],
        [0.4178, 0.4796, 0.1587, 0.0698],
        [0.2778, 0.7890, 0.4869, 0.2641]], device='cuda:0')
xyxy: tensor([[330.9896, 230.8546, 433.2338, 254.4259],
        [433.2134, 320.1606, 636.3028, 370.3940],
        [ 43.9676, 472.9617, 667.1946, 663.1448]], device='cuda:0')
xyxyn: tensor([[0.2586, 0.3206, 0.3385, 0.3534],
        [0.3384, 0.4447, 0.4971, 0.5144],
        [0.0343, 0.6569, 0.5212, 0.9210]], device='cuda:0')

0: 384x640 4 Potholes, 17.6ms
Speed: 2.2ms preprocess, 17.6ms inference, 1.9ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.7809, 0.6161, 0.6100, 0.2560], device='cuda:0')
data: tensor([[4.1218e+00, 4.9764e+02, 5.4276e+02, 7.0770e+02, 7.8087e-01, 0.0000e+00],
        [3.2843e+02, 2.3476e+02, 4.3314e+02, 2.6072e+02, 6.1608e-01, 0.0000e+00],
        [4.3085e+02, 3.2686e+02, 6.5583e+02, 3.8015e+02, 6.0999e-01, 0.0000e+00],
        [1.8985e+01, 4.9785e+02, 7.8164e+02, 6.9030e+02, 2.5601e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([4, 6])
xywh: tensor([[273.4394, 602.6688, 538.6353, 210.0654],
        [380.7830, 247.7409, 104.7111,  25.9674],
        [543.3414, 353.5040, 224.9741,  53.2880],
        [400.3121, 594.0714, 762.6547, 192.4519]], device='cuda:0')
xywhn: tensor([[0.2136, 0.8370, 0.4208, 0.2918],
        [0.2975, 0.3441, 0.0818, 0.0361],
        [0.4245, 0.4910, 0.1758, 0.0740],
        [0.3127, 0.8251, 0.5958, 0.2673]], device='cuda:0')
xyxy: tensor([[  4.1218, 497.6361, 542.7571, 707.7015],
        [328.4275, 234.7572, 433.1385, 260.7246],
        [430.8544, 326.8600, 655.8285, 380.1480],
        [ 18.9847, 497.8455, 781.6394, 690.2974]], device='cuda:0')
xyxyn: tensor([[0.0032, 0.6912, 0.4240, 0.9829],
        [0.2566, 0.3261, 0.3384, 0.3621],
        [0.3366, 0.4540, 0.5124, 0.5280],
        [0.0148, 0.6915, 0.6107, 0.9587]], device='cuda:0')

0: 384x640 4 Potholes, 13.7ms
Speed: 2.1ms preprocess, 13.7ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.7422, 0.7217, 0.6721, 0.2705], device='cuda:0')
data: tensor([[3.4055e+00, 5.0798e+02, 6.1311e+02, 7.1375e+02, 7.4224e-01, 0.0000e+00],
        [3.2284e+02, 2.3446e+02, 4.3029e+02, 2.6396e+02, 7.2167e-01, 0.0000e+00],
        [4.3026e+02, 3.2734e+02, 6.5479e+02, 3.8566e+02, 6.7212e-01, 0.0000e+00],
        [1.5715e+02, 4.1995e+02, 2.5907e+02, 4.6269e+02, 2.7051e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([4, 6])
xywh: tensor([[308.2574, 610.8666, 609.7039, 205.7678],
        [376.5664, 249.2136, 107.4454,  29.5024],
        [542.5216, 356.4978, 224.5332,  58.3199],
        [208.1145, 441.3194, 101.9200,  42.7441]], device='cuda:0')
xywhn: tensor([[0.2408, 0.8484, 0.4763, 0.2858],
        [0.2942, 0.3461, 0.0839, 0.0410],
        [0.4238, 0.4951, 0.1754, 0.0810],
        [0.1626, 0.6129, 0.0796, 0.0594]], device='cuda:0')
xyxy: tensor([[  3.4055, 507.9827, 613.1094, 713.7505],
        [322.8437, 234.4623, 430.2891, 263.9648],
        [430.2550, 327.3378, 654.7882, 385.6577],
        [157.1544, 419.9474, 259.0745, 462.6915]], device='cuda:0')
xyxyn: tensor([[0.0027, 0.7055, 0.4790, 0.9913],
        [0.2522, 0.3256, 0.3362, 0.3666],
        [0.3361, 0.4546, 0.5116, 0.5356],
        [0.1228, 0.5833, 0.2024, 0.6426]], device='cuda:0')

0: 384x640 5 Potholes, 15.1ms
Speed: 2.3ms preprocess, 15.1ms inference, 2.0ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.6711, 0.6535, 0.5935, 0.5727, 0.4470], device='cuda:0')
data: tensor([[3.2274e+02, 2.3610e+02, 4.3020e+02, 2.6435e+02, 6.7112e-01, 0.0000e+00],
        [4.2947e+02, 3.3221e+02, 6.4147e+02, 3.9180e+02, 6.5346e-01, 0.0000e+00],
        [1.0365e+01, 5.1655e+02, 9.2049e+02, 7.2000e+02, 5.9349e-01, 0.0000e+00],
        [1.4934e+02, 4.2555e+02, 2.5728e+02, 4.6989e+02, 5.7268e-01, 0.0000e+00],
        [1.7330e+00, 5.1936e+02, 5.5345e+02, 7.2000e+02, 4.4702e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([5, 6])
xywh: tensor([[376.4661, 250.2249, 107.4594,  28.2449],
        [535.4713, 362.0019, 212.0024,  59.5910],
        [465.4263, 618.2726, 910.1237, 203.4547],
        [203.3092, 447.7216, 107.9460,  44.3435],
        [277.5911, 619.6818, 551.7162, 200.6364]], device='cuda:0')
xywhn: tensor([[0.2941, 0.3475, 0.0840, 0.0392],
        [0.4183, 0.5028, 0.1656, 0.0828],
        [0.3636, 0.8587, 0.7110, 0.2826],
        [0.1588, 0.6218, 0.0843, 0.0616],
        [0.2169, 0.8607, 0.4310, 0.2787]], device='cuda:0')
xyxy: tensor([[322.7365, 236.1024, 430.1958, 264.3474],
        [429.4701, 332.2064, 641.4725, 391.7974],
        [ 10.3645, 516.5453, 920.4882, 720.0000],
        [149.3363, 425.5499, 257.2822, 469.8934],
        [  1.7330, 519.3636, 553.4492, 720.0000]], device='cuda:0')
xyxyn: tensor([[0.2521, 0.3279, 0.3361, 0.3671],
        [0.3355, 0.4614, 0.5012, 0.5442],
        [0.0081, 0.7174, 0.7191, 1.0000],
        [0.1167, 0.5910, 0.2010, 0.6526],
        [0.0014, 0.7213, 0.4324, 1.0000]], device='cuda:0')

0: 384x640 5 Potholes, 19.7ms
Speed: 2.0ms preprocess, 19.7ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.6870, 0.6810, 0.6618, 0.5084, 0.2869], device='cuda:0')
data: tensor([[4.3360e+02, 3.3736e+02, 6.5306e+02, 3.9459e+02, 6.8696e-01, 0.0000e+00],
        [1.6375e+01, 5.2169e+02, 9.3167e+02, 7.2000e+02, 6.8101e-01, 0.0000e+00],
        [3.1925e+02, 2.3865e+02, 4.2903e+02, 2.6528e+02, 6.6184e-01, 0.0000e+00],
        [1.4255e+02, 4.3262e+02, 2.5273e+02, 4.8103e+02, 5.0844e-01, 0.0000e+00],
        [1.0364e+03, 2.9053e+02, 1.1429e+03, 3.1825e+02, 2.8695e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([5, 6])
xywh: tensor([[ 543.3313,  365.9766,  219.4598,   57.2358],
        [ 474.0218,  620.8427,  915.2936,  198.3147],
        [ 374.1432,  251.9645,  109.7793,   26.6211],
        [ 197.6412,  456.8237,  110.1793,   48.4028],
        [1089.6594,  304.3896,  106.5657,   27.7166]], device='cuda:0')
xywhn: tensor([[0.4245, 0.5083, 0.1715, 0.0795],
        [0.3703, 0.8623, 0.7151, 0.2754],
        [0.2923, 0.3500, 0.0858, 0.0370],
        [0.1544, 0.6345, 0.0861, 0.0672],
        [0.8513, 0.4228, 0.0833, 0.0385]], device='cuda:0')
xyxy: tensor([[ 433.6014,  337.3587,  653.0612,  394.5945],
        [  16.3750,  521.6853,  931.6686,  720.0000],
        [ 319.2535,  238.6539,  429.0328,  265.2750],
        [ 142.5515,  432.6223,  252.7308,  481.0251],
        [1036.3766,  290.5313, 1142.9423,  318.2478]], device='cuda:0')
xyxyn: tensor([[0.3388, 0.4686, 0.5102, 0.5480],
        [0.0128, 0.7246, 0.7279, 1.0000],
        [0.2494, 0.3315, 0.3352, 0.3684],
        [0.1114, 0.6009, 0.1974, 0.6681],
        [0.8097, 0.4035, 0.8929, 0.4420]], device='cuda:0')

0: 384x640 6 Potholes, 13.2ms
Speed: 2.6ms preprocess, 13.2ms inference, 3.5ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.6391, 0.6275, 0.5587, 0.5034, 0.4836, 0.2503], device='cuda:0')
data: tensor([[8.3793e+00, 5.4282e+02, 8.3017e+02, 7.2000e+02, 6.3909e-01, 0.0000e+00],
        [3.1576e+02, 2.4472e+02, 4.2862e+02, 2.6884e+02, 6.2754e-01, 0.0000e+00],
        [4.2657e+02, 3.4385e+02, 6.4786e+02, 4.0233e+02, 5.5872e-01, 0.0000e+00],
        [4.0576e+02, 2.8276e+02, 5.5130e+02, 3.1307e+02, 5.0344e-01, 0.0000e+00],
        [2.2546e+00, 5.4835e+02, 5.6291e+02, 7.2000e+02, 4.8363e-01, 0.0000e+00],
        [1.0412e+03, 2.9380e+02, 1.1614e+03, 3.2383e+02, 2.5027e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([6, 6])
xywh: tensor([[ 419.2729,  631.4092,  821.7872,  177.1816],
        [ 372.1884,  256.7778,  112.8638,   24.1144],
        [ 537.2180,  373.0863,  221.2898,   58.4804],
        [ 478.5289,  297.9124,  145.5469,   30.3086],
        [ 282.5833,  634.1755,  560.6575,  171.6489],
        [1101.3391,  308.8136,  120.1943,   30.0267]], device='cuda:0')
xywhn: tensor([[0.3276, 0.8770, 0.6420, 0.2461],
        [0.2908, 0.3566, 0.0882, 0.0335],
        [0.4197, 0.5182, 0.1729, 0.0812],
        [0.3739, 0.4138, 0.1137, 0.0421],
        [0.2208, 0.8808, 0.4380, 0.2384],
        [0.8604, 0.4289, 0.0939, 0.0417]], device='cuda:0')
xyxy: tensor([[   8.3793,  542.8184,  830.1665,  720.0000],
        [ 315.7565,  244.7206,  428.6202,  268.8350],
        [ 426.5731,  343.8461,  647.8629,  402.3265],
        [ 405.7554,  282.7581,  551.3023,  313.0667],
        [   2.2546,  548.3511,  562.9120,  720.0000],
        [1041.2419,  293.8002, 1161.4363,  323.8270]], device='cuda:0')
xyxyn: tensor([[0.0065, 0.7539, 0.6486, 1.0000],
        [0.2467, 0.3399, 0.3349, 0.3734],
        [0.3333, 0.4776, 0.5061, 0.5588],
        [0.3170, 0.3927, 0.4307, 0.4348],
        [0.0018, 0.7616, 0.4398, 1.0000],
        [0.8135, 0.4081, 0.9074, 0.4498]], device='cuda:0')

0: 384x640 6 Potholes, 10.7ms
Speed: 2.0ms preprocess, 10.7ms inference, 1.9ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.7093, 0.6916, 0.6878, 0.6385, 0.4615, 0.2818], device='cuda:0')
data: tensor([[1.6051e+00, 5.5306e+02, 6.5081e+02, 7.2000e+02, 7.0935e-01, 0.0000e+00],
        [3.1347e+02, 2.4568e+02, 4.2692e+02, 2.7011e+02, 6.9156e-01, 0.0000e+00],
        [4.3596e+02, 3.4949e+02, 6.5442e+02, 4.1301e+02, 6.8779e-01, 0.0000e+00],
        [1.1433e+02, 4.5533e+02, 2.3472e+02, 5.0608e+02, 6.3848e-01, 0.0000e+00],
        [3.9648e+02, 2.8454e+02, 5.5360e+02, 3.1522e+02, 4.6150e-01, 0.0000e+00],
        [2.1817e+00, 5.4669e+02, 8.9790e+02, 7.2000e+02, 2.8178e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([6, 6])
xywh: tensor([[326.2058, 636.5303, 649.2014, 166.9395],
        [370.1961, 257.8941, 113.4498,  24.4319],
        [545.1858, 381.2474, 218.4590,  63.5182],
        [174.5246, 480.7043, 120.3873,  50.7511],
        [475.0360, 299.8778, 157.1205,  30.6786],
        [450.0403, 633.3459, 895.7172, 173.3082]], device='cuda:0')
xywhn: tensor([[0.2548, 0.8841, 0.5072, 0.2319],
        [0.2892, 0.3582, 0.0886, 0.0339],
        [0.4259, 0.5295, 0.1707, 0.0882],
        [0.1363, 0.6676, 0.0941, 0.0705],
        [0.3711, 0.4165, 0.1228, 0.0426],
        [0.3516, 0.8796, 0.6998, 0.2407]], device='cuda:0')
xyxy: tensor([[  1.6051, 553.0605, 650.8065, 720.0000],
        [313.4712, 245.6782, 426.9210, 270.1100],
        [435.9563, 349.4883, 654.4153, 413.0065],
        [114.3309, 455.3287, 234.7183, 506.0798],
        [396.4758, 284.5385, 553.5963, 315.2171],
        [  2.1817, 546.6918, 897.8989, 720.0000]], device='cuda:0')
xyxyn: tensor([[0.0013, 0.7681, 0.5084, 1.0000],
        [0.2449, 0.3412, 0.3335, 0.3752],
        [0.3406, 0.4854, 0.5113, 0.5736],
        [0.0893, 0.6324, 0.1834, 0.7029],
        [0.3097, 0.3952, 0.4325, 0.4378],
        [0.0017, 0.7593, 0.7015, 1.0000]], device='cuda:0')

0: 384x640 5 Potholes, 14.6ms
Speed: 2.0ms preprocess, 14.6ms inference, 2.0ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.7584, 0.6259, 0.5564, 0.5155, 0.5141], device='cuda:0')
data: tensor([[3.1176e+02, 2.4602e+02, 4.2513e+02, 2.7035e+02, 7.5839e-01, 0.0000e+00],
        [4.2613e+02, 3.5152e+02, 6.6230e+02, 4.1860e+02, 6.2595e-01, 0.0000e+00],
        [1.0825e+02, 4.6070e+02, 2.2878e+02, 5.1546e+02, 5.5638e-01, 0.0000e+00],
        [3.9587e+02, 2.8674e+02, 5.5144e+02, 3.1685e+02, 5.1553e-01, 0.0000e+00],
        [1.0128e+00, 5.7369e+02, 5.9419e+02, 7.2000e+02, 5.1413e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([5, 6])
xywh: tensor([[368.4464, 258.1851, 113.3698,  24.3208],
        [544.2168, 385.0622, 236.1665,  67.0799],
        [168.5164, 488.0795, 120.5331,  54.7610],
        [473.6571, 301.7954, 155.5675,  30.1172],
        [297.6011, 646.8451, 593.1765, 146.3098]], device='cuda:0')
xywhn: tensor([[0.2878, 0.3586, 0.0886, 0.0338],
        [0.4252, 0.5348, 0.1845, 0.0932],
        [0.1317, 0.6779, 0.0942, 0.0761],
        [0.3700, 0.4192, 0.1215, 0.0418],
        [0.2325, 0.8984, 0.4634, 0.2032]], device='cuda:0')
xyxy: tensor([[311.7615, 246.0247, 425.1313, 270.3455],
        [426.1335, 351.5223, 662.3000, 418.6022],
        [108.2498, 460.6989, 228.7829, 515.4600],
        [395.8734, 286.7368, 551.4409, 316.8540],
        [  1.0128, 573.6902, 594.1893, 720.0000]], device='cuda:0')
xyxyn: tensor([[2.4356e-01, 3.4170e-01, 3.3213e-01, 3.7548e-01],
        [3.3292e-01, 4.8823e-01, 5.1742e-01, 5.8139e-01],
        [8.4570e-02, 6.3986e-01, 1.7874e-01, 7.1592e-01],
        [3.0928e-01, 3.9825e-01, 4.3081e-01, 4.4007e-01],
        [7.9126e-04, 7.9679e-01, 4.6421e-01, 1.0000e+00]], device='cuda:0')

0: 384x640 3 Potholes, 11.4ms
Speed: 1.9ms preprocess, 11.4ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0.], device='cuda:0')
conf: tensor([0.7595, 0.6424, 0.4810], device='cuda:0')
data: tensor([[3.1185e+02, 2.4755e+02, 4.2449e+02, 2.7590e+02, 7.5950e-01, 0.0000e+00],
        [4.3031e+02, 3.6053e+02, 6.4934e+02, 4.2821e+02, 6.4237e-01, 0.0000e+00],
        [6.1859e+00, 5.9957e+02, 6.7614e+02, 7.2000e+02, 4.8104e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([3, 6])
xywh: tensor([[368.1673, 261.7249, 112.6404,  28.3420],
        [539.8264, 394.3664, 219.0331,  67.6793],
        [341.1646, 659.7850, 669.9575, 120.4300]], device='cuda:0')
xywhn: tensor([[0.2876, 0.3635, 0.0880, 0.0394],
        [0.4217, 0.5477, 0.1711, 0.0940],
        [0.2665, 0.9164, 0.5234, 0.1673]], device='cuda:0')
xyxy: tensor([[311.8471, 247.5539, 424.4875, 275.8959],
        [430.3099, 360.5267, 649.3430, 428.2061],
        [  6.1859, 599.5700, 676.1433, 720.0000]], device='cuda:0')
xyxyn: tensor([[0.2436, 0.3438, 0.3316, 0.3832],
        [0.3362, 0.5007, 0.5073, 0.5947],
        [0.0048, 0.8327, 0.5282, 1.0000]], device='cuda:0')

0: 384x640 3 Potholes, 9.7ms
Speed: 2.4ms preprocess, 9.7ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0.], device='cuda:0')
conf: tensor([0.7513, 0.5169, 0.3090], device='cuda:0')
data: tensor([[3.0967e+02, 2.4962e+02, 4.2470e+02, 2.7748e+02, 7.5132e-01, 0.0000e+00],
        [4.2575e+02, 3.6352e+02, 6.4696e+02, 4.3428e+02, 5.1691e-01, 0.0000e+00],
        [6.2351e+00, 6.0485e+02, 7.0017e+02, 7.2000e+02, 3.0903e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([3, 6])
xywh: tensor([[367.1834, 263.5497, 115.0340,  27.8529],
        [536.3525, 398.9003, 221.2081,  70.7546],
        [353.2034, 662.4264, 693.9366, 115.1472]], device='cuda:0')
xywhn: tensor([[0.2869, 0.3660, 0.0899, 0.0387],
        [0.4190, 0.5540, 0.1728, 0.0983],
        [0.2759, 0.9200, 0.5421, 0.1599]], device='cuda:0')
xyxy: tensor([[309.6664, 249.6233, 424.7004, 277.4762],
        [425.7485, 363.5230, 646.9566, 434.2776],
        [  6.2351, 604.8528, 700.1718, 720.0000]], device='cuda:0')
xyxyn: tensor([[0.2419, 0.3467, 0.3318, 0.3854],
        [0.3326, 0.5049, 0.5054, 0.6032],
        [0.0049, 0.8401, 0.5470, 1.0000]], device='cuda:0')

0: 384x640 2 Potholes, 12.1ms
Speed: 2.0ms preprocess, 12.1ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0.], device='cuda:0')
conf: tensor([0.7315, 0.5102], device='cuda:0')
data: tensor([[3.0970e+02, 2.5150e+02, 4.2276e+02, 2.7930e+02, 7.3149e-01, 0.0000e+00],
        [4.2496e+02, 3.5853e+02, 6.9711e+02, 4.3960e+02, 5.1022e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([2, 6])
xywh: tensor([[366.2269, 265.3992, 113.0584,  27.8042],
        [561.0323, 399.0673, 272.1494,  81.0688]], device='cuda:0')
xywhn: tensor([[0.2861, 0.3686, 0.0883, 0.0386],
        [0.4383, 0.5543, 0.2126, 0.1126]], device='cuda:0')
xyxy: tensor([[309.6977, 251.4971, 422.7561, 279.3013],
        [424.9576, 358.5329, 697.1071, 439.6017]], device='cuda:0')
xyxyn: tensor([[0.2420, 0.3493, 0.3303, 0.3879],
        [0.3320, 0.4980, 0.5446, 0.6106]], device='cuda:0')

0: 384x640 3 Potholes, 10.3ms
Speed: 1.9ms preprocess, 10.3ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0.], device='cuda:0')
conf: tensor([0.7205, 0.5540, 0.5232], device='cuda:0')
data: tensor([[3.0453e+02, 2.5408e+02, 4.2211e+02, 2.8370e+02, 7.2052e-01, 0.0000e+00],
        [3.7969e+02, 2.9797e+02, 5.5609e+02, 3.3474e+02, 5.5398e-01, 0.0000e+00],
        [4.1467e+02, 3.6787e+02, 6.8964e+02, 4.5244e+02, 5.2321e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([3, 6])
xywh: tensor([[363.3170, 268.8887, 117.5833,  29.6174],
        [467.8890, 316.3540, 176.3922,  36.7703],
        [552.1565, 410.1526, 274.9702,  84.5668]], device='cuda:0')
xywhn: tensor([[0.2838, 0.3735, 0.0919, 0.0411],
        [0.3655, 0.4394, 0.1378, 0.0511],
        [0.4314, 0.5697, 0.2148, 0.1175]], device='cuda:0')
xyxy: tensor([[304.5253, 254.0800, 422.1086, 283.6974],
        [379.6929, 297.9688, 556.0851, 334.7391],
        [414.6714, 367.8692, 689.6416, 452.4360]], device='cuda:0')
xyxyn: tensor([[0.2379, 0.3529, 0.3298, 0.3940],
        [0.2966, 0.4138, 0.4344, 0.4649],
        [0.3240, 0.5109, 0.5388, 0.6284]], device='cuda:0')

0: 384x640 5 Potholes, 9.8ms
Speed: 1.9ms preprocess, 9.8ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.7680, 0.6308, 0.5178, 0.3280, 0.2805], device='cuda:0')
data: tensor([[3.0465e+02, 2.5533e+02, 4.2136e+02, 2.8403e+02, 7.6804e-01, 0.0000e+00],
        [4.1803e+02, 3.7268e+02, 6.9829e+02, 4.6042e+02, 6.3082e-01, 0.0000e+00],
        [3.9237e+02, 3.0085e+02, 5.5152e+02, 3.3808e+02, 5.1776e-01, 0.0000e+00],
        [1.1032e+03, 3.2066e+02, 1.2208e+03, 3.5348e+02, 3.2799e-01, 0.0000e+00],
        [3.5007e+01, 5.2020e+02, 1.7822e+02, 5.8700e+02, 2.8046e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([5, 6])
xywh: tensor([[ 363.0084,  269.6812,  116.7113,   28.7021],
        [ 558.1580,  416.5490,  280.2543,   87.7397],
        [ 471.9457,  319.4628,  159.1553,   37.2350],
        [1162.0085,  337.0710,  117.5986,   32.8253],
        [ 106.6129,  553.6003,  143.2117,   66.7977]], device='cuda:0')
xywhn: tensor([[0.2836, 0.3746, 0.0912, 0.0399],
        [0.4361, 0.5785, 0.2189, 0.1219],
        [0.3687, 0.4437, 0.1243, 0.0517],
        [0.9078, 0.4682, 0.0919, 0.0456],
        [0.0833, 0.7689, 0.1119, 0.0928]], device='cuda:0')
xyxy: tensor([[ 304.6528,  255.3301,  421.3641,  284.0322],
        [ 418.0308,  372.6791,  698.2851,  460.4188],
        [ 392.3681,  300.8453,  551.5234,  338.0803],
        [1103.2092,  320.6584, 1220.8079,  353.4837],
        [  35.0070,  520.2014,  178.2187,  586.9991]], device='cuda:0')
xyxyn: tensor([[0.2380, 0.3546, 0.3292, 0.3945],
        [0.3266, 0.5176, 0.5455, 0.6395],
        [0.3065, 0.4178, 0.4309, 0.4696],
        [0.8619, 0.4454, 0.9538, 0.4909],
        [0.0273, 0.7225, 0.1392, 0.8153]], device='cuda:0')

0: 384x640 5 Potholes, 18.7ms
Speed: 2.0ms preprocess, 18.7ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.7823, 0.6804, 0.4428, 0.3698, 0.3298], device='cuda:0')
data: tensor([[3.0068e+02, 2.5815e+02, 4.1793e+02, 2.8468e+02, 7.8231e-01, 0.0000e+00],
        [4.0992e+02, 3.7559e+02, 7.1026e+02, 4.6667e+02, 6.8037e-01, 0.0000e+00],
        [3.9103e+02, 3.0513e+02, 5.5493e+02, 3.4093e+02, 4.4278e-01, 0.0000e+00],
        [1.1055e+03, 3.1727e+02, 1.2314e+03, 3.5186e+02, 3.6981e-01, 0.0000e+00],
        [2.2790e+01, 5.3188e+02, 1.7354e+02, 5.9802e+02, 3.2977e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([5, 6])
xywh: tensor([[ 359.3038,  271.4180,  117.2559,   26.5336],
        [ 560.0900,  421.1290,  300.3439,   91.0823],
        [ 472.9814,  323.0277,  163.9044,   35.8025],
        [1168.4607,  334.5647,  125.8704,   34.5981],
        [  98.1664,  564.9483,  150.7526,   66.1411]], device='cuda:0')
xywhn: tensor([[0.2807, 0.3770, 0.0916, 0.0369],
        [0.4376, 0.5849, 0.2346, 0.1265],
        [0.3695, 0.4486, 0.1281, 0.0497],
        [0.9129, 0.4647, 0.0983, 0.0481],
        [0.0767, 0.7847, 0.1178, 0.0919]], device='cuda:0')
xyxy: tensor([[ 300.6759,  258.1512,  417.9318,  284.6848],
        [ 409.9181,  375.5879,  710.2620,  466.6702],
        [ 391.0292,  305.1264,  554.9336,  340.9289],
        [1105.5255,  317.2656, 1231.3959,  351.8638],
        [  22.7901,  531.8777,  173.5427,  598.0189]], device='cuda:0')
xyxyn: tensor([[0.2349, 0.3585, 0.3265, 0.3954],
        [0.3202, 0.5216, 0.5549, 0.6482],
        [0.3055, 0.4238, 0.4335, 0.4735],
        [0.8637, 0.4406, 0.9620, 0.4887],
        [0.0178, 0.7387, 0.1356, 0.8306]], device='cuda:0')

0: 384x640 4 Potholes, 10.2ms
Speed: 2.2ms preprocess, 10.2ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.7745, 0.7134, 0.5931, 0.2897], device='cuda:0')
data: tensor([[2.9846e+02, 2.6070e+02, 4.1656e+02, 2.8752e+02, 7.7454e-01, 0.0000e+00],
        [4.0169e+02, 3.8394e+02, 7.3765e+02, 4.7702e+02, 7.1336e-01, 0.0000e+00],
        [3.8452e+02, 3.0491e+02, 5.5311e+02, 3.4671e+02, 5.9309e-01, 0.0000e+00],
        [1.1138e+03, 3.2135e+02, 1.2380e+03, 3.5186e+02, 2.8967e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([4, 6])
xywh: tensor([[ 357.5127,  274.1127,  118.0993,   26.8234],
        [ 569.6692,  430.4796,  335.9633,   93.0770],
        [ 468.8172,  325.8116,  168.5886,   41.8060],
        [1175.9104,  336.6054,  124.2285,   30.5068]], device='cuda:0')
xywhn: tensor([[0.2793, 0.3807, 0.0923, 0.0373],
        [0.4451, 0.5979, 0.2625, 0.1293],
        [0.3663, 0.4525, 0.1317, 0.0581],
        [0.9187, 0.4675, 0.0971, 0.0424]], device='cuda:0')
xyxy: tensor([[ 298.4630,  260.7010,  416.5623,  287.5244],
        [ 401.6876,  383.9410,  737.6508,  477.0181],
        [ 384.5229,  304.9086,  553.1115,  346.7146],
        [1113.7961,  321.3520, 1238.0247,  351.8588]], device='cuda:0')
xyxyn: tensor([[0.2332, 0.3621, 0.3254, 0.3993],
        [0.3138, 0.5333, 0.5763, 0.6625],
        [0.3004, 0.4235, 0.4321, 0.4815],
        [0.8702, 0.4463, 0.9672, 0.4887]], device='cuda:0')

0: 384x640 4 Potholes, 12.4ms
Speed: 2.2ms preprocess, 12.4ms inference, 1.9ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.7920, 0.7865, 0.6979, 0.2625], device='cuda:0')
data: tensor([[3.8392e+02, 3.0661e+02, 5.5306e+02, 3.5234e+02, 7.9201e-01, 0.0000e+00],
        [2.9223e+02, 2.6195e+02, 4.1453e+02, 2.9276e+02, 7.8648e-01, 0.0000e+00],
        [4.1228e+02, 3.9292e+02, 7.1956e+02, 4.8985e+02, 6.9787e-01, 0.0000e+00],
        [2.4141e-01, 5.6210e+02, 1.4047e+02, 6.7121e+02, 2.6245e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([4, 6])
xywh: tensor([[468.4887, 329.4797, 169.1335,  45.7303],
        [353.3783, 277.3545, 122.2947,  30.8101],
        [565.9227, 441.3844, 307.2791,  96.9272],
        [ 70.3562, 616.6523, 140.2296, 109.1141]], device='cuda:0')
xywhn: tensor([[0.3660, 0.4576, 0.1321, 0.0635],
        [0.2761, 0.3852, 0.0955, 0.0428],
        [0.4421, 0.6130, 0.2401, 0.1346],
        [0.0550, 0.8565, 0.1096, 0.1515]], device='cuda:0')
xyxy: tensor([[3.8392e+02, 3.0661e+02, 5.5306e+02, 3.5234e+02],
        [2.9223e+02, 2.6195e+02, 4.1453e+02, 2.9276e+02],
        [4.1228e+02, 3.9292e+02, 7.1956e+02, 4.8985e+02],
        [2.4141e-01, 5.6210e+02, 1.4047e+02, 6.7121e+02]], device='cuda:0')
xyxyn: tensor([[2.9994e-01, 4.2585e-01, 4.3207e-01, 4.8937e-01],
        [2.2831e-01, 3.6382e-01, 3.2385e-01, 4.0661e-01],
        [3.2210e-01, 5.4572e-01, 5.6216e-01, 6.8034e-01],
        [1.8860e-04, 7.8069e-01, 1.0974e-01, 9.3224e-01]], device='cuda:0')

0: 384x640 4 Potholes, 11.8ms
Speed: 3.0ms preprocess, 11.8ms inference, 1.8ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.7713, 0.7253, 0.6940, 0.3151], device='cuda:0')
data: tensor([[2.8981e+02, 2.6318e+02, 4.1342e+02, 2.9774e+02, 7.7126e-01, 0.0000e+00],
        [3.7948e+02, 3.0800e+02, 5.5477e+02, 3.5472e+02, 7.2531e-01, 0.0000e+00],
        [4.2002e+02, 4.0445e+02, 6.9636e+02, 4.9655e+02, 6.9400e-01, 0.0000e+00],
        [8.7438e+02, 3.2939e+02, 1.0000e+03, 3.5799e+02, 3.1514e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([4, 6])
xywh: tensor([[351.6118, 280.4623, 123.6110,  34.5583],
        [467.1243, 331.3594, 175.2831,  46.7286],
        [558.1893, 450.4975, 276.3474,  92.1026],
        [937.2051, 343.6895, 125.6455,  28.5978]], device='cuda:0')
xywhn: tensor([[0.2747, 0.3895, 0.0966, 0.0480],
        [0.3649, 0.4602, 0.1369, 0.0649],
        [0.4361, 0.6257, 0.2159, 0.1279],
        [0.7322, 0.4773, 0.0982, 0.0397]], device='cuda:0')
xyxy: tensor([[ 289.8063,  263.1831,  413.4173,  297.7415],
        [ 379.4828,  307.9951,  554.7659,  354.7237],
        [ 420.0156,  404.4462,  696.3630,  496.5488],
        [ 874.3823,  329.3906, 1000.0278,  357.9883]], device='cuda:0')
xyxyn: tensor([[0.2264, 0.3655, 0.3230, 0.4135],
        [0.2965, 0.4278, 0.4334, 0.4927],
        [0.3281, 0.5617, 0.5440, 0.6897],
        [0.6831, 0.4575, 0.7813, 0.4972]], device='cuda:0')

0: 384x640 5 Potholes, 12.3ms
Speed: 2.3ms preprocess, 12.3ms inference, 3.2ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.7824, 0.7766, 0.6507, 0.4852, 0.2767], device='cuda:0')
data: tensor([[2.8749e+02, 2.6454e+02, 4.1233e+02, 3.0076e+02, 7.8240e-01, 0.0000e+00],
        [4.1046e+02, 3.9991e+02, 7.3044e+02, 5.0846e+02, 7.7660e-01, 0.0000e+00],
        [3.7642e+02, 3.1558e+02, 5.5522e+02, 3.5661e+02, 6.5068e-01, 0.0000e+00],
        [1.1410e+03, 3.2688e+02, 1.2752e+03, 3.6830e+02, 4.8523e-01, 0.0000e+00],
        [8.8192e+02, 3.3429e+02, 1.0051e+03, 3.6088e+02, 2.7669e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([5, 6])
xywh: tensor([[ 349.9124,  282.6500,  124.8452,   36.2159],
        [ 570.4512,  454.1839,  319.9736,  108.5433],
        [ 465.8236,  336.0964,  178.7979,   41.0295],
        [1208.1035,  347.5903,  134.2056,   41.4263],
        [ 943.5286,  347.5829,  123.2103,   26.5907]], device='cuda:0')
xywhn: tensor([[0.2734, 0.3926, 0.0975, 0.0503],
        [0.4457, 0.6308, 0.2500, 0.1508],
        [0.3639, 0.4668, 0.1397, 0.0570],
        [0.9438, 0.4828, 0.1048, 0.0575],
        [0.7371, 0.4828, 0.0963, 0.0369]], device='cuda:0')
xyxy: tensor([[ 287.4898,  264.5421,  412.3350,  300.7580],
        [ 410.4644,  399.9123,  730.4380,  508.4556],
        [ 376.4247,  315.5816,  555.2225,  356.6111],
        [1141.0007,  326.8772, 1275.2063,  368.3035],
        [ 881.9235,  334.2875, 1005.1338,  360.8782]], device='cuda:0')
xyxyn: tensor([[0.2246, 0.3674, 0.3221, 0.4177],
        [0.3207, 0.5554, 0.5707, 0.7062],
        [0.2941, 0.4383, 0.4338, 0.4953],
        [0.8914, 0.4540, 0.9963, 0.5115],
        [0.6890, 0.4643, 0.7853, 0.5012]], device='cuda:0')

0: 384x640 4 Potholes, 17.1ms
Speed: 2.2ms preprocess, 17.1ms inference, 2.0ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.7893, 0.7591, 0.6726, 0.2888], device='cuda:0')
data: tensor([[4.1667e+02, 4.0466e+02, 7.5858e+02, 5.2608e+02, 7.8934e-01, 0.0000e+00],
        [2.7949e+02, 2.6854e+02, 4.1102e+02, 3.0168e+02, 7.5915e-01, 0.0000e+00],
        [3.7667e+02, 3.2437e+02, 5.5713e+02, 3.6561e+02, 6.7258e-01, 0.0000e+00],
        [8.8990e+02, 3.3862e+02, 1.0219e+03, 3.6702e+02, 2.8880e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([4, 6])
xywh: tensor([[587.6258, 465.3685, 341.9030, 121.4158],
        [345.2547, 285.1101, 131.5326,  33.1311],
        [466.9026, 344.9896, 180.4593,  41.2443],
        [955.8794, 352.8192, 131.9492,  28.3977]], device='cuda:0')
xywhn: tensor([[0.4591, 0.6463, 0.2671, 0.1686],
        [0.2697, 0.3960, 0.1028, 0.0460],
        [0.3648, 0.4792, 0.1410, 0.0573],
        [0.7468, 0.4900, 0.1031, 0.0394]], device='cuda:0')
xyxy: tensor([[ 416.6743,  404.6606,  758.5773,  526.0764],
        [ 279.4884,  268.5445,  411.0210,  301.6756],
        [ 376.6729,  324.3674,  557.1322,  365.6117],
        [ 889.9048,  338.6203, 1021.8540,  367.0180]], device='cuda:0')
xyxyn: tensor([[0.3255, 0.5620, 0.5926, 0.7307],
        [0.2184, 0.3730, 0.3211, 0.4190],
        [0.2943, 0.4505, 0.4353, 0.5078],
        [0.6952, 0.4703, 0.7983, 0.5097]], device='cuda:0')

0: 384x640 5 Potholes, 9.5ms
Speed: 2.1ms preprocess, 9.5ms inference, 2.5ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.8358, 0.8065, 0.7579, 0.4504, 0.3174], device='cuda:0')
data: tensor([[3.9922e+02, 4.1383e+02, 7.6467e+02, 5.3894e+02, 8.3584e-01, 0.0000e+00],
        [2.7810e+02, 2.7054e+02, 4.0743e+02, 3.0211e+02, 8.0646e-01, 0.0000e+00],
        [3.7500e+02, 3.2636e+02, 5.5735e+02, 3.7195e+02, 7.5787e-01, 0.0000e+00],
        [8.9572e+02, 3.4068e+02, 1.0243e+03, 3.7108e+02, 4.5040e-01, 0.0000e+00],
        [9.4423e-01, 6.2572e+02, 8.9680e+01, 7.1442e+02, 3.1735e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([5, 6])
xywh: tensor([[581.9410, 476.3812, 365.4495, 125.1106],
        [342.7661, 286.3238, 129.3250,  31.5706],
        [466.1743, 349.1557, 182.3568,  45.5875],
        [960.0198, 355.8762, 128.6001,  30.3996],
        [ 45.3123, 670.0732,  88.7361,  88.7034]], device='cuda:0')
xywhn: tensor([[0.4546, 0.6616, 0.2855, 0.1738],
        [0.2678, 0.3977, 0.1010, 0.0438],
        [0.3642, 0.4849, 0.1425, 0.0633],
        [0.7500, 0.4943, 0.1005, 0.0422],
        [0.0354, 0.9307, 0.0693, 0.1232]], device='cuda:0')
xyxy: tensor([[3.9922e+02, 4.1383e+02, 7.6467e+02, 5.3894e+02],
        [2.7810e+02, 2.7054e+02, 4.0743e+02, 3.0211e+02],
        [3.7500e+02, 3.2636e+02, 5.5735e+02, 3.7195e+02],
        [8.9572e+02, 3.4068e+02, 1.0243e+03, 3.7108e+02],
        [9.4423e-01, 6.2572e+02, 8.9680e+01, 7.1442e+02]], device='cuda:0')
xyxyn: tensor([[3.1189e-01, 5.7476e-01, 5.9740e-01, 7.4852e-01],
        [2.1727e-01, 3.7575e-01, 3.1830e-01, 4.1960e-01],
        [2.9297e-01, 4.5328e-01, 4.3543e-01, 5.1660e-01],
        [6.9978e-01, 4.7316e-01, 8.0025e-01, 5.1538e-01],
        [7.3768e-04, 8.6906e-01, 7.0063e-02, 9.9226e-01]], device='cuda:0')

0: 384x640 7 Potholes, 9.6ms
Speed: 2.5ms preprocess, 9.6ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.8247, 0.7358, 0.7129, 0.5225, 0.3988, 0.3759, 0.3401], device='cuda:0')
data: tensor([[3.9312e+02, 4.2151e+02, 7.6982e+02, 5.4808e+02, 8.2467e-01, 0.0000e+00],
        [2.7346e+02, 2.7211e+02, 4.0723e+02, 3.0423e+02, 7.3576e-01, 0.0000e+00],
        [3.7673e+02, 3.2653e+02, 5.5499e+02, 3.7309e+02, 7.1286e-01, 0.0000e+00],
        [9.0245e+02, 3.4303e+02, 1.0311e+03, 3.7397e+02, 5.2252e-01, 0.0000e+00],
        [8.9563e+02, 2.9512e+02, 1.0223e+03, 3.2376e+02, 3.9876e-01, 0.0000e+00],
        [1.1740e+03, 3.4371e+02, 1.2789e+03, 3.9495e+02, 3.7585e-01, 0.0000e+00],
        [9.0002e+02, 2.4964e+02, 1.0495e+03, 2.8247e+02, 3.4008e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([7, 6])
xywh: tensor([[ 581.4717,  484.7930,  376.7053,  126.5748],
        [ 340.3464,  288.1733,  133.7677,   32.1216],
        [ 465.8615,  349.8089,  178.2561,   46.5591],
        [ 966.7930,  358.5002,  128.6826,   30.9333],
        [ 958.9443,  309.4398,  126.6353,   28.6353],
        [1226.4508,  369.3296,  104.9148,   51.2354],
        [ 974.7624,  266.0538,  149.4806,   32.8325]], device='cuda:0')
xywhn: tensor([[0.4543, 0.6733, 0.2943, 0.1758],
        [0.2659, 0.4002, 0.1045, 0.0446],
        [0.3640, 0.4858, 0.1393, 0.0647],
        [0.7553, 0.4979, 0.1005, 0.0430],
        [0.7492, 0.4298, 0.0989, 0.0398],
        [0.9582, 0.5130, 0.0820, 0.0712],
        [0.7615, 0.3695, 0.1168, 0.0456]], device='cuda:0')
xyxy: tensor([[ 393.1190,  421.5056,  769.8243,  548.0804],
        [ 273.4625,  272.1125,  407.2302,  304.2341],
        [ 376.7334,  326.5293,  554.9895,  373.0884],
        [ 902.4517,  343.0336, 1031.1343,  373.9669],
        [ 895.6266,  295.1222, 1022.2619,  323.7574],
        [1173.9934,  343.7119, 1278.9082,  394.9473],
        [ 900.0221,  249.6376, 1049.5027,  282.4701]], device='cuda:0')
xyxyn: tensor([[0.3071, 0.5854, 0.6014, 0.7612],
        [0.2136, 0.3779, 0.3181, 0.4225],
        [0.2943, 0.4535, 0.4336, 0.5182],
        [0.7050, 0.4764, 0.8056, 0.5194],
        [0.6997, 0.4099, 0.7986, 0.4497],
        [0.9172, 0.4774, 0.9991, 0.5485],
        [0.7031, 0.3467, 0.8199, 0.3923]], device='cuda:0')

0: 384x640 6 Potholes, 9.3ms
Speed: 2.0ms preprocess, 9.3ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.8346, 0.8305, 0.7569, 0.6589, 0.4769, 0.2507], device='cuda:0')
data: tensor([[3.7162e+02, 4.2914e+02, 7.7642e+02, 5.7678e+02, 8.3459e-01, 0.0000e+00],
        [2.6539e+02, 2.7551e+02, 4.0174e+02, 3.0882e+02, 8.3048e-01, 0.0000e+00],
        [3.6330e+02, 3.3304e+02, 5.5383e+02, 3.8574e+02, 7.5688e-01, 0.0000e+00],
        [9.1134e+02, 3.5153e+02, 1.0457e+03, 3.8109e+02, 6.5891e-01, 0.0000e+00],
        [9.1259e+02, 2.5233e+02, 1.0630e+03, 2.8397e+02, 4.7695e-01, 0.0000e+00],
        [1.1926e+03, 3.5293e+02, 1.2790e+03, 3.8614e+02, 2.5070e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([6, 6])
xywh: tensor([[ 574.0205,  502.9598,  404.7981,  147.6306],
        [ 333.5618,  292.1645,  136.3478,   33.3015],
        [ 458.5641,  359.3906,  190.5289,   52.6941],
        [ 978.4931,  366.3086,  134.3138,   29.5641],
        [ 987.7752,  268.1529,  150.3788,   31.6359],
        [1235.7732,  369.5360,   86.3994,   33.2068]], device='cuda:0')
xywhn: tensor([[0.4485, 0.6986, 0.3162, 0.2050],
        [0.2606, 0.4058, 0.1065, 0.0463],
        [0.3583, 0.4992, 0.1489, 0.0732],
        [0.7644, 0.5088, 0.1049, 0.0411],
        [0.7717, 0.3724, 0.1175, 0.0439],
        [0.9654, 0.5132, 0.0675, 0.0461]], device='cuda:0')
xyxy: tensor([[ 371.6215,  429.1445,  776.4196,  576.7751],
        [ 265.3879,  275.5137,  401.7357,  308.8152],
        [ 363.2996,  333.0436,  553.8286,  385.7377],
        [ 911.3362,  351.5266, 1045.6500,  381.0907],
        [ 912.5858,  252.3350, 1062.9646,  283.9708],
        [1192.5735,  352.9326, 1278.9729,  386.1395]], device='cuda:0')
xyxyn: tensor([[0.2903, 0.5960, 0.6066, 0.8011],
        [0.2073, 0.3827, 0.3139, 0.4289],
        [0.2838, 0.4626, 0.4327, 0.5357],
        [0.7120, 0.4882, 0.8169, 0.5293],
        [0.7130, 0.3505, 0.8304, 0.3944],
        [0.9317, 0.4902, 0.9992, 0.5363]], device='cuda:0')

0: 384x640 6 Potholes, 11.2ms
Speed: 2.1ms preprocess, 11.2ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.8714, 0.8153, 0.8037, 0.6448, 0.6059, 0.3561], device='cuda:0')
data: tensor([[3.7484e+02, 4.3299e+02, 7.9001e+02, 5.8925e+02, 8.7136e-01, 0.0000e+00],
        [3.6338e+02, 3.3445e+02, 5.5567e+02, 3.8927e+02, 8.1532e-01, 0.0000e+00],
        [2.6303e+02, 2.7651e+02, 4.0183e+02, 3.1471e+02, 8.0367e-01, 0.0000e+00],
        [9.1370e+02, 3.5274e+02, 1.0520e+03, 3.8591e+02, 6.4477e-01, 0.0000e+00],
        [9.1475e+02, 2.5405e+02, 1.0658e+03, 2.8449e+02, 6.0589e-01, 0.0000e+00],
        [9.0985e+02, 3.0203e+02, 1.0365e+03, 3.3429e+02, 3.5609e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([6, 6])
xywh: tensor([[582.4211, 511.1229, 415.1709, 156.2637],
        [459.5247, 361.8622, 192.2979,  54.8158],
        [332.4322, 295.6125, 138.8010,  38.2022],
        [982.8369, 369.3278, 138.2656,  33.1691],
        [990.3021, 269.2682, 151.0945,  30.4425],
        [973.1818, 318.1613, 126.6580,  32.2672]], device='cuda:0')
xywhn: tensor([[0.4550, 0.7099, 0.3244, 0.2170],
        [0.3590, 0.5026, 0.1502, 0.0761],
        [0.2597, 0.4106, 0.1084, 0.0531],
        [0.7678, 0.5130, 0.1080, 0.0461],
        [0.7737, 0.3740, 0.1180, 0.0423],
        [0.7603, 0.4419, 0.0990, 0.0448]], device='cuda:0')
xyxy: tensor([[ 374.8356,  432.9911,  790.0065,  589.2548],
        [ 363.3758,  334.4543,  555.6736,  389.2701],
        [ 263.0317,  276.5114,  401.8327,  314.7136],
        [ 913.7041,  352.7433, 1051.9697,  385.9124],
        [ 914.7549,  254.0470, 1065.8494,  284.4895],
        [ 909.8528,  302.0277, 1036.5107,  334.2949]], device='cuda:0')
xyxyn: tensor([[0.2928, 0.6014, 0.6172, 0.8184],
        [0.2839, 0.4645, 0.4341, 0.5407],
        [0.2055, 0.3840, 0.3139, 0.4371],
        [0.7138, 0.4899, 0.8219, 0.5360],
        [0.7147, 0.3528, 0.8327, 0.3951],
        [0.7108, 0.4195, 0.8098, 0.4643]], device='cuda:0')

0: 384x640 8 Potholes, 12.3ms
Speed: 2.0ms preprocess, 12.3ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0., 0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.8692, 0.7913, 0.7790, 0.7104, 0.5865, 0.3298, 0.3121, 0.3091], device='cuda:0')
data: tensor([[3.6354e+02, 4.4126e+02, 7.8898e+02, 5.9256e+02, 8.6920e-01, 0.0000e+00],
        [2.6232e+02, 2.7846e+02, 4.0133e+02, 3.1776e+02, 7.9133e-01, 0.0000e+00],
        [3.5532e+02, 3.3938e+02, 5.5848e+02, 3.9345e+02, 7.7897e-01, 0.0000e+00],
        [9.2076e+02, 3.5757e+02, 1.0620e+03, 3.8950e+02, 7.1041e-01, 0.0000e+00],
        [9.1647e+02, 2.5613e+02, 1.0709e+03, 2.8574e+02, 5.8652e-01, 0.0000e+00],
        [1.2104e+03, 3.6157e+02, 1.2797e+03, 3.9277e+02, 3.2978e-01, 0.0000e+00],
        [9.0735e+02, 3.0341e+02, 1.0393e+03, 3.3452e+02, 3.1212e-01, 0.0000e+00],
        [1.2085e+03, 3.6171e+02, 1.2798e+03, 4.0522e+02, 3.0908e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([8, 6])
xywh: tensor([[ 576.2570,  516.9132,  425.4376,  151.3005],
        [ 331.8220,  298.1137,  139.0098,   39.3005],
        [ 456.9037,  366.4145,  203.1587,   54.0739],
        [ 991.3742,  373.5342,  141.2340,   31.9290],
        [ 993.6659,  270.9329,  154.3955,   29.6075],
        [1245.0657,  377.1725,   69.3081,   31.1982],
        [ 973.3495,  318.9664,  131.9993,   31.1141],
        [1244.1556,  383.4605,   71.2434,   43.5094]], device='cuda:0')
xywhn: tensor([[0.4502, 0.7179, 0.3324, 0.2101],
        [0.2592, 0.4140, 0.1086, 0.0546],
        [0.3570, 0.5089, 0.1587, 0.0751],
        [0.7745, 0.5188, 0.1103, 0.0443],
        [0.7763, 0.3763, 0.1206, 0.0411],
        [0.9727, 0.5239, 0.0541, 0.0433],
        [0.7604, 0.4430, 0.1031, 0.0432],
        [0.9720, 0.5326, 0.0557, 0.0604]], device='cuda:0')
xyxy: tensor([[ 363.5382,  441.2630,  788.9758,  592.5635],
        [ 262.3171,  278.4634,  401.3269,  317.7640],
        [ 355.3243,  339.3776,  558.4830,  393.4515],
        [ 920.7572,  357.5697, 1061.9912,  389.4987],
        [ 916.4681,  256.1292, 1070.8636,  285.7366],
        [1210.4116,  361.5734, 1279.7197,  392.7717],
        [ 907.3499,  303.4093, 1039.3491,  334.5235],
        [1208.5339,  361.7058, 1279.7773,  405.2152]], device='cuda:0')
xyxyn: tensor([[0.2840, 0.6129, 0.6164, 0.8230],
        [0.2049, 0.3868, 0.3135, 0.4413],
        [0.2776, 0.4714, 0.4363, 0.5465],
        [0.7193, 0.4966, 0.8297, 0.5410],
        [0.7160, 0.3557, 0.8366, 0.3969],
        [0.9456, 0.5022, 0.9998, 0.5455],
        [0.7089, 0.4214, 0.8120, 0.4646],
        [0.9442, 0.5024, 0.9998, 0.5628]], device='cuda:0')

0: 384x640 7 Potholes, 10.0ms
Speed: 2.6ms preprocess, 10.0ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.8436, 0.8433, 0.7661, 0.6649, 0.5089, 0.3645, 0.3125], device='cuda:0')
data: tensor([[3.5830e+02, 4.5456e+02, 7.9370e+02, 6.0338e+02, 8.4363e-01, 0.0000e+00],
        [2.6040e+02, 2.8106e+02, 4.0101e+02, 3.1768e+02, 8.4332e-01, 0.0000e+00],
        [3.5149e+02, 3.4695e+02, 5.5835e+02, 3.9808e+02, 7.6605e-01, 0.0000e+00],
        [9.2096e+02, 3.5705e+02, 1.0687e+03, 3.9414e+02, 6.6493e-01, 0.0000e+00],
        [9.1667e+02, 3.0437e+02, 1.0460e+03, 3.3685e+02, 5.0892e-01, 0.0000e+00],
        [9.2121e+02, 2.5918e+02, 1.0769e+03, 2.8904e+02, 3.6449e-01, 0.0000e+00],
        [1.2195e+03, 3.6305e+02, 1.2793e+03, 3.9196e+02, 3.1246e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([7, 6])
xywh: tensor([[ 575.9991,  528.9685,  435.4071,  148.8160],
        [ 330.7009,  299.3682,  140.6113,   36.6177],
        [ 454.9235,  372.5154,  206.8619,   51.1219],
        [ 994.8066,  375.5961,  147.6882,   37.0948],
        [ 981.3546,  320.6092,  129.3767,   32.4792],
        [ 999.0502,  274.1104,  155.6765,   29.8679],
        [1249.3906,  377.5081,   59.8169,   28.9082]], device='cuda:0')
xywhn: tensor([[0.4500, 0.7347, 0.3402, 0.2067],
        [0.2584, 0.4158, 0.1099, 0.0509],
        [0.3554, 0.5174, 0.1616, 0.0710],
        [0.7772, 0.5217, 0.1154, 0.0515],
        [0.7667, 0.4453, 0.1011, 0.0451],
        [0.7805, 0.3807, 0.1216, 0.0415],
        [0.9761, 0.5243, 0.0467, 0.0402]], device='cuda:0')
xyxy: tensor([[ 358.2955,  454.5605,  793.7026,  603.3765],
        [ 260.3952,  281.0594,  401.0065,  317.6770],
        [ 351.4925,  346.9545,  558.3544,  398.0764],
        [ 920.9625,  357.0486, 1068.6508,  394.1435],
        [ 916.6663,  304.3696, 1046.0430,  336.8488],
        [ 921.2119,  259.1765, 1076.8884,  289.0444],
        [1219.4822,  363.0540, 1279.2991,  391.9622]], device='cuda:0')
xyxyn: tensor([[0.2799, 0.6313, 0.6201, 0.8380],
        [0.2034, 0.3904, 0.3133, 0.4412],
        [0.2746, 0.4819, 0.4362, 0.5529],
        [0.7195, 0.4959, 0.8349, 0.5474],
        [0.7161, 0.4227, 0.8172, 0.4678],
        [0.7197, 0.3600, 0.8413, 0.4015],
        [0.9527, 0.5042, 0.9995, 0.5444]], device='cuda:0')

0: 384x640 6 Potholes, 10.6ms
Speed: 2.0ms preprocess, 10.6ms inference, 4.7ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.8514, 0.7672, 0.7380, 0.6713, 0.5721, 0.4997], device='cuda:0')
data: tensor([[3.4270e+02, 4.6477e+02, 8.0774e+02, 6.4688e+02, 8.5136e-01, 0.0000e+00],
        [3.5123e+02, 3.5497e+02, 5.5866e+02, 4.1075e+02, 7.6723e-01, 0.0000e+00],
        [2.5676e+02, 2.8666e+02, 3.9662e+02, 3.2310e+02, 7.3800e-01, 0.0000e+00],
        [9.3693e+02, 3.6769e+02, 1.0876e+03, 4.0385e+02, 6.7133e-01, 0.0000e+00],
        [9.2558e+02, 3.1067e+02, 1.0626e+03, 3.4648e+02, 5.7210e-01, 0.0000e+00],
        [9.2485e+02, 2.6391e+02, 1.0851e+03, 2.9577e+02, 4.9974e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([6, 6])
xywh: tensor([[ 575.2217,  555.8265,  465.0346,  182.1158],
        [ 454.9413,  382.8633,  207.4296,   55.7823],
        [ 326.6878,  304.8839,  139.8651,   36.4412],
        [1012.2756,  385.7672,  150.6978,   36.1588],
        [ 994.0837,  328.5707,  137.0073,   35.8110],
        [1004.9623,  279.8410,  160.2273,   31.8584]], device='cuda:0')
xywhn: tensor([[0.4494, 0.7720, 0.3633, 0.2529],
        [0.3554, 0.5318, 0.1621, 0.0775],
        [0.2552, 0.4234, 0.1093, 0.0506],
        [0.7908, 0.5358, 0.1177, 0.0502],
        [0.7766, 0.4563, 0.1070, 0.0497],
        [0.7851, 0.3887, 0.1252, 0.0442]], device='cuda:0')
xyxy: tensor([[ 342.7044,  464.7686,  807.7390,  646.8844],
        [ 351.2266,  354.9722,  558.6561,  410.7545],
        [ 256.7552,  286.6633,  396.6203,  323.1045],
        [ 936.9268,  367.6878, 1087.6245,  403.8466],
        [ 925.5801,  310.6652, 1062.5874,  346.4763],
        [ 924.8486,  263.9118, 1085.0759,  295.7702]], device='cuda:0')
xyxyn: tensor([[0.2677, 0.6455, 0.6310, 0.8985],
        [0.2744, 0.4930, 0.4365, 0.5705],
        [0.2006, 0.3981, 0.3099, 0.4488],
        [0.7320, 0.5107, 0.8497, 0.5609],
        [0.7231, 0.4315, 0.8301, 0.4812],
        [0.7225, 0.3665, 0.8477, 0.4108]], device='cuda:0')

0: 384x640 6 Potholes, 10.2ms
Speed: 2.0ms preprocess, 10.2ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.8622, 0.7956, 0.7862, 0.6967, 0.6812, 0.6322], device='cuda:0')
data: tensor([[3.4115e+02, 4.6920e+02, 8.1918e+02, 6.5675e+02, 8.6222e-01, 0.0000e+00],
        [3.4474e+02, 3.5820e+02, 5.5798e+02, 4.1381e+02, 7.9564e-01, 0.0000e+00],
        [2.4805e+02, 2.8956e+02, 3.9239e+02, 3.2602e+02, 7.8618e-01, 0.0000e+00],
        [9.3262e+02, 3.1175e+02, 1.0687e+03, 3.5093e+02, 6.9670e-01, 0.0000e+00],
        [9.4504e+02, 3.7214e+02, 1.0940e+03, 4.0921e+02, 6.8124e-01, 0.0000e+00],
        [9.2901e+02, 2.6101e+02, 1.0934e+03, 2.9809e+02, 6.3215e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([6, 6])
xywh: tensor([[ 580.1660,  562.9765,  478.0313,  187.5449],
        [ 451.3615,  386.0065,  213.2368,   55.6168],
        [ 320.2207,  307.7877,  144.3486,   36.4585],
        [1000.6451,  331.3399,  136.0521,   39.1876],
        [1019.5378,  390.6733,  148.9889,   37.0706],
        [1011.1986,  279.5538,  164.3804,   37.0814]], device='cuda:0')
xywhn: tensor([[0.4533, 0.7819, 0.3735, 0.2605],
        [0.3526, 0.5361, 0.1666, 0.0772],
        [0.2502, 0.4275, 0.1128, 0.0506],
        [0.7818, 0.4602, 0.1063, 0.0544],
        [0.7965, 0.5426, 0.1164, 0.0515],
        [0.7900, 0.3883, 0.1284, 0.0515]], device='cuda:0')
xyxy: tensor([[ 341.1504,  469.2040,  819.1816,  656.7490],
        [ 344.7430,  358.1981,  557.9799,  413.8149],
        [ 248.0464,  289.5585,  392.3950,  326.0170],
        [ 932.6190,  311.7461, 1068.6711,  350.9337],
        [ 945.0433,  372.1381, 1094.0322,  409.2086],
        [ 929.0084,  261.0131, 1093.3888,  298.0945]], device='cuda:0')
xyxyn: tensor([[0.2665, 0.6517, 0.6400, 0.9122],
        [0.2693, 0.4975, 0.4359, 0.5747],
        [0.1938, 0.4022, 0.3066, 0.4528],
        [0.7286, 0.4330, 0.8349, 0.4874],
        [0.7383, 0.5169, 0.8547, 0.5683],
        [0.7258, 0.3625, 0.8542, 0.4140]], device='cuda:0')

0: 384x640 6 Potholes, 9.6ms
Speed: 2.0ms preprocess, 9.6ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.8994, 0.8013, 0.7678, 0.7392, 0.7247, 0.5893], device='cuda:0')
data: tensor([[3.3483e+02, 4.8093e+02, 8.3233e+02, 6.6301e+02, 8.9942e-01, 0.0000e+00],
        [2.4277e+02, 2.9166e+02, 3.8994e+02, 3.3146e+02, 8.0133e-01, 0.0000e+00],
        [3.4341e+02, 3.6394e+02, 5.5794e+02, 4.1644e+02, 7.6781e-01, 0.0000e+00],
        [9.5116e+02, 3.7977e+02, 1.0982e+03, 4.1318e+02, 7.3921e-01, 0.0000e+00],
        [9.3387e+02, 2.6232e+02, 1.0993e+03, 2.9937e+02, 7.2472e-01, 0.0000e+00],
        [9.2986e+02, 3.1510e+02, 1.0712e+03, 3.5064e+02, 5.8931e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([6, 6])
xywh: tensor([[ 583.5820,  571.9694,  497.5037,  182.0798],
        [ 316.3541,  311.5607,  147.1756,   39.8070],
        [ 450.6744,  390.1913,  214.5286,   52.4999],
        [1024.6760,  396.4742,  147.0294,   33.4050],
        [1016.5874,  280.8422,  165.4360,   37.0491],
        [1000.5268,  332.8687,  141.3282,   35.5372]], device='cuda:0')
xywhn: tensor([[0.4559, 0.7944, 0.3887, 0.2529],
        [0.2472, 0.4327, 0.1150, 0.0553],
        [0.3521, 0.5419, 0.1676, 0.0729],
        [0.8005, 0.5507, 0.1149, 0.0464],
        [0.7942, 0.3901, 0.1292, 0.0515],
        [0.7817, 0.4623, 0.1104, 0.0494]], device='cuda:0')
xyxy: tensor([[ 334.8302,  480.9295,  832.3339,  663.0093],
        [ 242.7663,  291.6572,  389.9419,  331.4642],
        [ 343.4101,  363.9413,  557.9387,  416.4413],
        [ 951.1613,  379.7717, 1098.1907,  413.1768],
        [ 933.8694,  262.3176, 1099.3054,  299.3667],
        [ 929.8627,  315.1001, 1071.1909,  350.6373]], device='cuda:0')
xyxyn: tensor([[0.2616, 0.6680, 0.6503, 0.9208],
        [0.1897, 0.4051, 0.3046, 0.4604],
        [0.2683, 0.5055, 0.4359, 0.5784],
        [0.7431, 0.5275, 0.8580, 0.5739],
        [0.7296, 0.3643, 0.8588, 0.4158],
        [0.7265, 0.4376, 0.8369, 0.4870]], device='cuda:0')

0: 384x640 7 Potholes, 11.2ms
Speed: 4.0ms preprocess, 11.2ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.8185, 0.8147, 0.7966, 0.7205, 0.6932, 0.5374, 0.3037], device='cuda:0')
data: tensor([[3.4056e+02, 3.6967e+02, 5.5767e+02, 4.3263e+02, 8.1846e-01, 0.0000e+00],
        [2.3089e+02, 2.9492e+02, 3.8873e+02, 3.3711e+02, 8.1474e-01, 0.0000e+00],
        [3.1970e+02, 4.9595e+02, 8.5253e+02, 7.1874e+02, 7.9663e-01, 0.0000e+00],
        [9.4103e+02, 2.6379e+02, 1.1100e+03, 3.0178e+02, 7.2046e-01, 0.0000e+00],
        [9.6421e+02, 3.8744e+02, 1.1250e+03, 4.2459e+02, 6.9318e-01, 0.0000e+00],
        [9.3585e+02, 3.1906e+02, 1.0902e+03, 3.5634e+02, 5.3743e-01, 0.0000e+00],
        [3.3708e+02, 5.0277e+02, 1.1861e+03, 7.2000e+02, 3.0374e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([7, 6])
xywh: tensor([[ 449.1119,  401.1472,  217.1121,   62.9639],
        [ 309.8104,  316.0138,  157.8491,   42.1829],
        [ 586.1156,  607.3447,  532.8325,  222.7883],
        [1025.5377,  282.7842,  169.0085,   37.9891],
        [1044.5887,  406.0182,  160.7478,   37.1485],
        [1013.0172,  337.7005,  154.3325,   37.2803],
        [ 761.5710,  611.3832,  848.9788,  217.2336]], device='cuda:0')
xywhn: tensor([[0.3509, 0.5571, 0.1696, 0.0874],
        [0.2420, 0.4389, 0.1233, 0.0586],
        [0.4579, 0.8435, 0.4163, 0.3094],
        [0.8012, 0.3928, 0.1320, 0.0528],
        [0.8161, 0.5639, 0.1256, 0.0516],
        [0.7914, 0.4690, 0.1206, 0.0518],
        [0.5950, 0.8491, 0.6633, 0.3017]], device='cuda:0')
xyxy: tensor([[ 340.5559,  369.6653,  557.6680,  432.6291],
        [ 230.8859,  294.9224,  388.7350,  337.1052],
        [ 319.6993,  495.9506,  852.5319,  718.7389],
        [ 941.0334,  263.7896, 1110.0420,  301.7787],
        [ 964.2148,  387.4440, 1124.9626,  424.5925],
        [ 935.8510,  319.0603, 1090.1835,  356.3406],
        [ 337.0817,  502.7664, 1186.0604,  720.0000]], device='cuda:0')
xyxyn: tensor([[0.2661, 0.5134, 0.4357, 0.6009],
        [0.1804, 0.4096, 0.3037, 0.4682],
        [0.2498, 0.6888, 0.6660, 0.9982],
        [0.7352, 0.3664, 0.8672, 0.4191],
        [0.7533, 0.5381, 0.8789, 0.5897],
        [0.7311, 0.4431, 0.8517, 0.4949],
        [0.2633, 0.6983, 0.9266, 1.0000]], device='cuda:0')

0: 384x640 6 Potholes, 8.4ms
Speed: 3.2ms preprocess, 8.4ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.8794, 0.8608, 0.7954, 0.7510, 0.7488, 0.6824], device='cuda:0')
data: tensor([[3.1806e+02, 5.0315e+02, 8.5078e+02, 7.1967e+02, 8.7942e-01, 0.0000e+00],
        [2.3086e+02, 2.9925e+02, 3.8658e+02, 3.3938e+02, 8.6076e-01, 0.0000e+00],
        [3.3814e+02, 3.7506e+02, 5.5991e+02, 4.3764e+02, 7.9539e-01, 0.0000e+00],
        [9.6688e+02, 3.8816e+02, 1.1306e+03, 4.3071e+02, 7.5096e-01, 0.0000e+00],
        [9.4230e+02, 2.6508e+02, 1.1149e+03, 3.0481e+02, 7.4876e-01, 0.0000e+00],
        [9.5101e+02, 3.2226e+02, 1.0959e+03, 3.6307e+02, 6.8238e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([6, 6])
xywh: tensor([[ 584.4216,  611.4077,  532.7227,  216.5200],
        [ 308.7178,  319.3185,  155.7231,   40.1289],
        [ 449.0213,  406.3481,  221.7682,   62.5815],
        [1048.7290,  409.4367,  163.6885,   42.5461],
        [1028.5784,  284.9438,  172.5497,   39.7324],
        [1023.4622,  342.6668,  144.9043,   40.8107]], device='cuda:0')
xywhn: tensor([[0.4566, 0.8492, 0.4162, 0.3007],
        [0.2412, 0.4435, 0.1217, 0.0557],
        [0.3508, 0.5644, 0.1733, 0.0869],
        [0.8193, 0.5687, 0.1279, 0.0591],
        [0.8036, 0.3958, 0.1348, 0.0552],
        [0.7996, 0.4759, 0.1132, 0.0567]], device='cuda:0')
xyxy: tensor([[ 318.0603,  503.1477,  850.7830,  719.6677],
        [ 230.8562,  299.2540,  386.5793,  339.3829],
        [ 338.1372,  375.0573,  559.9055,  437.6389],
        [ 966.8848,  388.1636, 1130.5732,  430.7098],
        [ 942.3035,  265.0776, 1114.8533,  304.8100],
        [ 951.0100,  322.2615, 1095.9143,  363.0722]], device='cuda:0')
xyxyn: tensor([[0.2485, 0.6988, 0.6647, 0.9995],
        [0.1804, 0.4156, 0.3020, 0.4714],
        [0.2642, 0.5209, 0.4374, 0.6078],
        [0.7554, 0.5391, 0.8833, 0.5982],
        [0.7362, 0.3682, 0.8710, 0.4233],
        [0.7430, 0.4476, 0.8562, 0.5043]], device='cuda:0')

0: 384x640 7 Potholes, 11.2ms
Speed: 1.9ms preprocess, 11.2ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.8526, 0.8271, 0.8216, 0.7690, 0.7468, 0.7258, 0.3222], device='cuda:0')
data: tensor([[3.1360e+02, 5.1375e+02, 8.8146e+02, 7.1997e+02, 8.5261e-01, 0.0000e+00],
        [2.3020e+02, 3.0115e+02, 3.8527e+02, 3.4001e+02, 8.2708e-01, 0.0000e+00],
        [3.3218e+02, 3.8169e+02, 5.6026e+02, 4.4627e+02, 8.2156e-01, 0.0000e+00],
        [9.4811e+02, 3.2430e+02, 1.1034e+03, 3.6600e+02, 7.6901e-01, 0.0000e+00],
        [9.7280e+02, 3.9255e+02, 1.1434e+03, 4.3580e+02, 7.4675e-01, 0.0000e+00],
        [9.4223e+02, 2.6799e+02, 1.1187e+03, 3.0787e+02, 7.2583e-01, 0.0000e+00],
        [3.3296e+02, 5.1417e+02, 1.1833e+03, 7.2000e+02, 3.2218e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([7, 6])
xywh: tensor([[ 597.5296,  616.8618,  567.8542,  206.2213],
        [ 307.7349,  320.5797,  155.0715,   38.8579],
        [ 446.2240,  413.9817,  228.0818,   64.5758],
        [1025.7395,  345.1497,  155.2527,   41.7034],
        [1058.0879,  414.1738,  170.5664,   43.2539],
        [1030.4724,  287.9323,  176.4931,   39.8853],
        [ 758.1474,  617.0833,  850.3776,  205.8336]], device='cuda:0')
xywhn: tensor([[0.4668, 0.8568, 0.4436, 0.2864],
        [0.2404, 0.4452, 0.1211, 0.0540],
        [0.3486, 0.5750, 0.1782, 0.0897],
        [0.8014, 0.4794, 0.1213, 0.0579],
        [0.8266, 0.5752, 0.1333, 0.0601],
        [0.8051, 0.3999, 0.1379, 0.0554],
        [0.5923, 0.8571, 0.6644, 0.2859]], device='cuda:0')
xyxy: tensor([[ 313.6025,  513.7511,  881.4567,  719.9724],
        [ 230.1991,  301.1507,  385.2707,  340.0086],
        [ 332.1831,  381.6938,  560.2649,  446.2696],
        [ 948.1132,  324.2980, 1103.3658,  366.0014],
        [ 972.8047,  392.5469, 1143.3711,  435.8008],
        [ 942.2259,  267.9896, 1118.7190,  307.8749],
        [ 332.9586,  514.1664, 1183.3362,  720.0000]], device='cuda:0')
xyxyn: tensor([[0.2450, 0.7135, 0.6886, 1.0000],
        [0.1798, 0.4183, 0.3010, 0.4722],
        [0.2595, 0.5301, 0.4377, 0.6198],
        [0.7407, 0.4504, 0.8620, 0.5083],
        [0.7600, 0.5452, 0.8933, 0.6053],
        [0.7361, 0.3722, 0.8740, 0.4276],
        [0.2601, 0.7141, 0.9245, 1.0000]], device='cuda:0')

0: 384x640 7 Potholes, 11.9ms
Speed: 1.9ms preprocess, 11.9ms inference, 2.8ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.8372, 0.8242, 0.7674, 0.7467, 0.6882, 0.6701, 0.5514], device='cuda:0')
data: tensor([[3.2113e+02, 3.8877e+02, 5.6056e+02, 4.5740e+02, 8.3724e-01, 0.0000e+00],
        [3.0303e+02, 5.3353e+02, 9.0382e+02, 7.2000e+02, 8.2415e-01, 0.0000e+00],
        [2.2058e+02, 3.0622e+02, 3.8066e+02, 3.4903e+02, 7.6743e-01, 0.0000e+00],
        [9.5072e+02, 2.7207e+02, 1.1363e+03, 3.1420e+02, 7.4673e-01, 0.0000e+00],
        [9.7846e+02, 4.0547e+02, 1.1616e+03, 4.4870e+02, 6.8816e-01, 0.0000e+00],
        [3.2366e+02, 5.3133e+02, 1.2149e+03, 7.2000e+02, 6.7008e-01, 0.0000e+00],
        [9.6696e+02, 3.2745e+02, 1.1187e+03, 3.6993e+02, 5.5142e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([7, 6])
xywh: tensor([[ 440.8430,  423.0814,  239.4339,   68.6290],
        [ 603.4243,  626.7666,  600.7904,  186.4668],
        [ 300.6167,  327.6223,  160.0775,   42.8115],
        [1043.5092,  293.1332,  185.5859,   42.1308],
        [1070.0396,  427.0823,  183.1548,   43.2319],
        [ 769.2715,  625.6628,  891.2290,  188.6744],
        [1042.8223,  348.6914,  151.7148,   42.4778]], device='cuda:0')
xywhn: tensor([[0.3444, 0.5876, 0.1871, 0.0953],
        [0.4714, 0.8705, 0.4694, 0.2590],
        [0.2349, 0.4550, 0.1251, 0.0595],
        [0.8152, 0.4071, 0.1450, 0.0585],
        [0.8360, 0.5932, 0.1431, 0.0600],
        [0.6010, 0.8690, 0.6963, 0.2620],
        [0.8147, 0.4843, 0.1185, 0.0590]], device='cuda:0')
xyxy: tensor([[ 321.1260,  388.7668,  560.5599,  457.3959],
        [ 303.0291,  533.5332,  903.8195,  720.0000],
        [ 220.5780,  306.2166,  380.6555,  349.0281],
        [ 950.7162,  272.0678, 1136.3021,  314.1986],
        [ 978.4621,  405.4664, 1161.6169,  448.6982],
        [ 323.6570,  531.3256, 1214.8860,  720.0000],
        [ 966.9648,  327.4525, 1118.6797,  369.9303]], device='cuda:0')
xyxyn: tensor([[0.2509, 0.5400, 0.4379, 0.6353],
        [0.2367, 0.7410, 0.7061, 1.0000],
        [0.1723, 0.4253, 0.2974, 0.4848],
        [0.7427, 0.3779, 0.8877, 0.4364],
        [0.7644, 0.5631, 0.9075, 0.6232],
        [0.2529, 0.7380, 0.9491, 1.0000],
        [0.7554, 0.4548, 0.8740, 0.5138]], device='cuda:0')

0: 384x640 7 Potholes, 13.2ms
Speed: 3.2ms preprocess, 13.2ms inference, 1.8ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.8483, 0.8243, 0.7774, 0.7519, 0.7509, 0.7269, 0.5026], device='cuda:0')
data: tensor([[3.1667e+02, 3.9588e+02, 5.6206e+02, 4.6712e+02, 8.4829e-01, 0.0000e+00],
        [2.1444e+02, 3.0726e+02, 3.7904e+02, 3.5521e+02, 8.2429e-01, 0.0000e+00],
        [9.9279e+02, 4.1795e+02, 1.1783e+03, 4.6022e+02, 7.7740e-01, 0.0000e+00],
        [9.5601e+02, 2.7652e+02, 1.1381e+03, 3.1671e+02, 7.5191e-01, 0.0000e+00],
        [2.6796e+02, 5.4472e+02, 9.1931e+02, 7.2000e+02, 7.5090e-01, 0.0000e+00],
        [9.7341e+02, 3.3230e+02, 1.1290e+03, 3.7568e+02, 7.2695e-01, 0.0000e+00],
        [2.8636e+02, 5.3998e+02, 1.1635e+03, 7.2000e+02, 5.0265e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([7, 6])
xywh: tensor([[ 439.3665,  431.4979,  245.3946,   71.2406],
        [ 296.7396,  331.2356,  164.6090,   47.9417],
        [1085.5505,  439.0837,  185.5137,   42.2735],
        [1047.0710,  296.6131,  182.1226,   40.1847],
        [ 593.6376,  632.3602,  651.3501,  175.2795],
        [1051.2211,  353.9907,  155.6130,   43.3824],
        [ 724.9117,  629.9897,  877.1072,  180.0205]], device='cuda:0')
xywhn: tensor([[0.3433, 0.5993, 0.1917, 0.0989],
        [0.2318, 0.4600, 0.1286, 0.0666],
        [0.8481, 0.6098, 0.1449, 0.0587],
        [0.8180, 0.4120, 0.1423, 0.0558],
        [0.4638, 0.8783, 0.5089, 0.2434],
        [0.8213, 0.4917, 0.1216, 0.0603],
        [0.5663, 0.8750, 0.6852, 0.2500]], device='cuda:0')
xyxy: tensor([[ 316.6693,  395.8776,  562.0638,  467.1182],
        [ 214.4351,  307.2648,  379.0441,  355.2064],
        [ 992.7936,  417.9470, 1178.3074,  460.2205],
        [ 956.0097,  276.5208, 1138.1323,  316.7054],
        [ 267.9625,  544.7205,  919.3126,  720.0000],
        [ 973.4146,  332.2994, 1129.0276,  375.6819],
        [ 286.3581,  539.9795, 1163.4653,  720.0000]], device='cuda:0')
xyxyn: tensor([[0.2474, 0.5498, 0.4391, 0.6488],
        [0.1675, 0.4268, 0.2961, 0.4933],
        [0.7756, 0.5805, 0.9206, 0.6392],
        [0.7469, 0.3841, 0.8892, 0.4399],
        [0.2093, 0.7566, 0.7182, 1.0000],
        [0.7605, 0.4615, 0.8821, 0.5218],
        [0.2237, 0.7500, 0.9090, 1.0000]], device='cuda:0')

0: 384x640 6 Potholes, 11.1ms
Speed: 1.9ms preprocess, 11.1ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.8673, 0.8317, 0.8277, 0.7823, 0.6972, 0.6955], device='cuda:0')
data: tensor([[3.1675e+02, 4.0030e+02, 5.6132e+02, 4.7559e+02, 8.6733e-01, 0.0000e+00],
        [2.1480e+02, 3.1006e+02, 3.7760e+02, 3.5790e+02, 8.3165e-01, 0.0000e+00],
        [1.0050e+03, 4.2188e+02, 1.1878e+03, 4.6464e+02, 8.2770e-01, 0.0000e+00],
        [9.6506e+02, 2.7703e+02, 1.1445e+03, 3.1925e+02, 7.8230e-01, 0.0000e+00],
        [2.7540e+02, 5.5114e+02, 9.0918e+02, 7.2000e+02, 6.9721e-01, 0.0000e+00],
        [9.7689e+02, 3.3992e+02, 1.1351e+03, 3.8258e+02, 6.9552e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([6, 6])
xywh: tensor([[ 439.0359,  437.9448,  244.5742,   75.2947],
        [ 296.2033,  333.9792,  162.7990,   47.8441],
        [1096.3982,  443.2594,  182.7195,   42.7653],
        [1054.7734,  298.1420,  179.4282,   42.2156],
        [ 592.2911,  635.5692,  633.7744,  168.8616],
        [1056.0132,  361.2537,  158.2456,   42.6616]], device='cuda:0')
xywhn: tensor([[0.3430, 0.6083, 0.1911, 0.1046],
        [0.2314, 0.4639, 0.1272, 0.0665],
        [0.8566, 0.6156, 0.1427, 0.0594],
        [0.8240, 0.4141, 0.1402, 0.0586],
        [0.4627, 0.8827, 0.4951, 0.2345],
        [0.8250, 0.5017, 0.1236, 0.0593]], device='cuda:0')
xyxy: tensor([[ 316.7488,  400.2974,  561.3230,  475.5921],
        [ 214.8038,  310.0571,  377.6028,  357.9012],
        [1005.0385,  421.8768, 1187.7579,  464.6420],
        [ 965.0594,  277.0342, 1144.4875,  319.2498],
        [ 275.4039,  551.1384,  909.1783,  720.0000],
        [ 976.8904,  339.9229, 1135.1360,  382.5845]], device='cuda:0')
xyxyn: tensor([[0.2475, 0.5560, 0.4385, 0.6605],
        [0.1678, 0.4306, 0.2950, 0.4971],
        [0.7852, 0.5859, 0.9279, 0.6453],
        [0.7540, 0.3848, 0.8941, 0.4434],
        [0.2152, 0.7655, 0.7103, 1.0000],
        [0.7632, 0.4721, 0.8868, 0.5314]], device='cuda:0')

0: 384x640 6 Potholes, 13.1ms
Speed: 2.5ms preprocess, 13.1ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.9024, 0.8705, 0.8077, 0.7813, 0.7712, 0.6883], device='cuda:0')
data: tensor([[3.1147e+02, 4.0429e+02, 5.6698e+02, 4.8181e+02, 9.0236e-01, 0.0000e+00],
        [2.0980e+02, 3.1637e+02, 3.7658e+02, 3.6121e+02, 8.7047e-01, 0.0000e+00],
        [9.6530e+02, 2.7825e+02, 1.1482e+03, 3.2187e+02, 8.0774e-01, 0.0000e+00],
        [9.8114e+02, 3.4106e+02, 1.1430e+03, 3.8570e+02, 7.8134e-01, 0.0000e+00],
        [1.0155e+03, 4.2714e+02, 1.1987e+03, 4.7071e+02, 7.7125e-01, 0.0000e+00],
        [2.6398e+02, 5.6612e+02, 9.1166e+02, 7.2000e+02, 6.8834e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([6, 6])
xywh: tensor([[ 439.2270,  443.0515,  255.5120,   77.5262],
        [ 293.1868,  338.7898,  166.7796,   44.8479],
        [1056.7279,  300.0569,  182.8562,   43.6184],
        [1062.0525,  363.3793,  161.8271,   44.6437],
        [1107.0984,  448.9267,  183.1586,   43.5646],
        [ 587.8176,  643.0597,  647.6819,  153.8806]], device='cuda:0')
xywhn: tensor([[0.3431, 0.6153, 0.1996, 0.1077],
        [0.2291, 0.4705, 0.1303, 0.0623],
        [0.8256, 0.4167, 0.1429, 0.0606],
        [0.8297, 0.5047, 0.1264, 0.0620],
        [0.8649, 0.6235, 0.1431, 0.0605],
        [0.4592, 0.8931, 0.5060, 0.2137]], device='cuda:0')
xyxy: tensor([[ 311.4710,  404.2883,  566.9830,  481.8146],
        [ 209.7970,  316.3659,  376.5765,  361.2138],
        [ 965.2998,  278.2477, 1148.1560,  321.8661],
        [ 981.1390,  341.0574, 1142.9661,  385.7011],
        [1015.5191,  427.1444, 1198.6777,  470.7090],
        [ 263.9767,  566.1194,  911.6586,  720.0000]], device='cuda:0')
xyxyn: tensor([[0.2433, 0.5615, 0.4430, 0.6692],
        [0.1639, 0.4394, 0.2942, 0.5017],
        [0.7541, 0.3865, 0.8970, 0.4470],
        [0.7665, 0.4737, 0.8929, 0.5357],
        [0.7934, 0.5933, 0.9365, 0.6538],
        [0.2062, 0.7863, 0.7122, 1.0000]], device='cuda:0')

0: 384x640 6 Potholes, 12.3ms
Speed: 2.3ms preprocess, 12.3ms inference, 2.8ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.9053, 0.8792, 0.7865, 0.7859, 0.7631, 0.6609], device='cuda:0')
data: tensor([[1.9523e+02, 3.2147e+02, 3.7225e+02, 3.7119e+02, 9.0527e-01, 0.0000e+00],
        [3.0110e+02, 4.1711e+02, 5.6921e+02, 5.0174e+02, 8.7918e-01, 0.0000e+00],
        [9.9001e+02, 3.4369e+02, 1.1652e+03, 3.9542e+02, 7.8653e-01, 0.0000e+00],
        [1.0213e+03, 4.3751e+02, 1.2265e+03, 4.8590e+02, 7.8590e-01, 0.0000e+00],
        [9.6843e+02, 2.8518e+02, 1.1716e+03, 3.2811e+02, 7.6308e-01, 0.0000e+00],
        [3.1942e+02, 5.9143e+02, 9.0902e+02, 7.2000e+02, 6.6091e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([6, 6])
xywh: tensor([[ 283.7395,  346.3286,  177.0176,   49.7240],
        [ 435.1547,  459.4283,  268.1083,   84.6328],
        [1077.6021,  369.5529,  175.1885,   51.7247],
        [1123.8879,  461.7020,  205.1663,   48.3935],
        [1070.0366,  306.6444,  203.2200,   42.9232],
        [ 614.2200,  655.7163,  589.6000,  128.5674]], device='cuda:0')
xywhn: tensor([[0.2217, 0.4810, 0.1383, 0.0691],
        [0.3400, 0.6381, 0.2095, 0.1175],
        [0.8419, 0.5133, 0.1369, 0.0718],
        [0.8780, 0.6413, 0.1603, 0.0672],
        [0.8360, 0.4259, 0.1588, 0.0596],
        [0.4799, 0.9107, 0.4606, 0.1786]], device='cuda:0')
xyxy: tensor([[ 195.2307,  321.4666,  372.2483,  371.1906],
        [ 301.1005,  417.1119,  569.2088,  501.7448],
        [ 990.0078,  343.6906, 1165.1963,  395.4153],
        [1021.3048,  437.5053, 1226.4711,  485.8988],
        [ 968.4266,  285.1828, 1171.6466,  328.1060],
        [ 319.4200,  591.4326,  909.0200,  720.0000]], device='cuda:0')
xyxyn: tensor([[0.1525, 0.4465, 0.2908, 0.5155],
        [0.2352, 0.5793, 0.4447, 0.6969],
        [0.7734, 0.4773, 0.9103, 0.5492],
        [0.7979, 0.6076, 0.9582, 0.6749],
        [0.7566, 0.3961, 0.9153, 0.4557],
        [0.2495, 0.8214, 0.7102, 1.0000]], device='cuda:0')

0: 384x640 6 Potholes, 14.6ms
Speed: 1.9ms preprocess, 14.6ms inference, 3.3ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.8811, 0.8649, 0.8373, 0.8217, 0.7885, 0.6301], device='cuda:0')
data: tensor([[2.9676e+02, 4.2627e+02, 5.6873e+02, 5.1119e+02, 8.8115e-01, 0.0000e+00],
        [1.9445e+02, 3.2237e+02, 3.6905e+02, 3.7368e+02, 8.6492e-01, 0.0000e+00],
        [1.0245e+03, 4.4663e+02, 1.2423e+03, 4.9684e+02, 8.3733e-01, 0.0000e+00],
        [9.7585e+02, 2.8683e+02, 1.1809e+03, 3.3018e+02, 8.2165e-01, 0.0000e+00],
        [9.9180e+02, 3.4954e+02, 1.1726e+03, 3.9868e+02, 7.8846e-01, 0.0000e+00],
        [3.2755e+02, 6.0709e+02, 9.0611e+02, 7.2000e+02, 6.3011e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([6, 6])
xywh: tensor([[ 432.7453,  468.7283,  271.9683,   84.9226],
        [ 281.7494,  348.0245,  174.5941,   51.3069],
        [1133.4009,  471.7394,  217.7051,   50.2101],
        [1078.3777,  308.5012,  205.0564,   43.3510],
        [1082.2107,  374.1095,  180.8130,   49.1425],
        [ 616.8329,  663.5444,  578.5630,  112.9111]], device='cuda:0')
xywhn: tensor([[0.3381, 0.6510, 0.2125, 0.1179],
        [0.2201, 0.4834, 0.1364, 0.0713],
        [0.8855, 0.6552, 0.1701, 0.0697],
        [0.8425, 0.4285, 0.1602, 0.0602],
        [0.8455, 0.5196, 0.1413, 0.0683],
        [0.4819, 0.9216, 0.4520, 0.1568]], device='cuda:0')
xyxy: tensor([[ 296.7612,  426.2670,  568.7295,  511.1896],
        [ 194.4523,  322.3711,  369.0464,  373.6780],
        [1024.5483,  446.6343, 1242.2534,  496.8444],
        [ 975.8495,  286.8257, 1180.9059,  330.1767],
        [ 991.8042,  349.5383, 1172.6172,  398.6807],
        [ 327.5514,  607.0889,  906.1144,  720.0000]], device='cuda:0')
xyxyn: tensor([[0.2318, 0.5920, 0.4443, 0.7100],
        [0.1519, 0.4477, 0.2883, 0.5190],
        [0.8004, 0.6203, 0.9705, 0.6901],
        [0.7624, 0.3984, 0.9226, 0.4586],
        [0.7748, 0.4855, 0.9161, 0.5537],
        [0.2559, 0.8432, 0.7079, 1.0000]], device='cuda:0')

0: 384x640 6 Potholes, 10.3ms
Speed: 2.0ms preprocess, 10.3ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.9236, 0.8909, 0.8130, 0.7944, 0.7884, 0.3638], device='cuda:0')
data: tensor([[2.9584e+02, 4.3150e+02, 5.7424e+02, 5.1951e+02, 9.2360e-01, 0.0000e+00],
        [1.8884e+02, 3.2666e+02, 3.6968e+02, 3.7743e+02, 8.9091e-01, 0.0000e+00],
        [9.8467e+02, 2.9106e+02, 1.1837e+03, 3.3436e+02, 8.1302e-01, 0.0000e+00],
        [1.0433e+03, 4.5607e+02, 1.2532e+03, 5.0229e+02, 7.9442e-01, 0.0000e+00],
        [9.9840e+02, 3.5469e+02, 1.1804e+03, 4.0428e+02, 7.8844e-01, 0.0000e+00],
        [3.3991e+02, 6.2051e+02, 9.1083e+02, 7.2000e+02, 3.6382e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([6, 6])
xywh: tensor([[ 435.0388,  475.5060,  278.3939,   88.0045],
        [ 279.2630,  352.0474,  180.8406,   50.7699],
        [1084.1940,  312.7064,  199.0542,   43.3018],
        [1148.2377,  479.1797,  209.9722,   46.2292],
        [1089.3850,  379.4849,  181.9786,   49.5983],
        [ 625.3668,  670.2565,  570.9219,   99.4871]], device='cuda:0')
xywhn: tensor([[0.3399, 0.6604, 0.2175, 0.1222],
        [0.2182, 0.4890, 0.1413, 0.0705],
        [0.8470, 0.4343, 0.1555, 0.0601],
        [0.8971, 0.6655, 0.1640, 0.0642],
        [0.8511, 0.5271, 0.1422, 0.0689],
        [0.4886, 0.9309, 0.4460, 0.1382]], device='cuda:0')
xyxy: tensor([[ 295.8419,  431.5038,  574.2358,  519.5083],
        [ 188.8427,  326.6624,  369.6833,  377.4323],
        [ 984.6669,  291.0555, 1183.7211,  334.3573],
        [1043.2516,  456.0651, 1253.2238,  502.2943],
        [ 998.3957,  354.6858, 1180.3743,  404.2841],
        [ 339.9059,  620.5129,  910.8278,  720.0000]], device='cuda:0')
xyxyn: tensor([[0.2311, 0.5993, 0.4486, 0.7215],
        [0.1475, 0.4537, 0.2888, 0.5242],
        [0.7693, 0.4042, 0.9248, 0.4644],
        [0.8150, 0.6334, 0.9791, 0.6976],
        [0.7800, 0.4926, 0.9222, 0.5615],
        [0.2656, 0.8618, 0.7116, 1.0000]], device='cuda:0')

0: 384x640 6 Potholes, 13.3ms
Speed: 1.9ms preprocess, 13.3ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.9149, 0.9073, 0.8335, 0.7607, 0.7033, 0.3059], device='cuda:0')
data: tensor([[1.7591e+02, 3.3527e+02, 3.6500e+02, 3.8971e+02, 9.1492e-01, 0.0000e+00],
        [2.7149e+02, 4.4510e+02, 5.7926e+02, 5.4258e+02, 9.0727e-01, 0.0000e+00],
        [9.9505e+02, 2.9136e+02, 1.1985e+03, 3.4301e+02, 8.3348e-01, 0.0000e+00],
        [1.0414e+03, 4.6217e+02, 1.2790e+03, 5.2568e+02, 7.6065e-01, 0.0000e+00],
        [1.0244e+03, 3.5665e+02, 1.2057e+03, 4.1592e+02, 7.0330e-01, 0.0000e+00],
        [4.0155e+02, 6.4689e+02, 9.1138e+02, 7.2000e+02, 3.0591e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([6, 6])
xywh: tensor([[ 270.4534,  362.4935,  189.0963,   54.4372],
        [ 425.3749,  493.8417,  307.7740,   97.4749],
        [1096.7712,  317.1842,  203.4458,   51.6539],
        [1160.2012,  493.9282,  237.5415,   63.5122],
        [1115.0376,  386.2870,  181.3638,   59.2758],
        [ 656.4634,  683.4456,  509.8330,   73.1089]], device='cuda:0')
xywhn: tensor([[0.2113, 0.5035, 0.1477, 0.0756],
        [0.3323, 0.6859, 0.2404, 0.1354],
        [0.8569, 0.4405, 0.1589, 0.0717],
        [0.9064, 0.6860, 0.1856, 0.0882],
        [0.8711, 0.5365, 0.1417, 0.0823],
        [0.5129, 0.9492, 0.3983, 0.1015]], device='cuda:0')
xyxy: tensor([[ 175.9052,  335.2749,  365.0015,  389.7121],
        [ 271.4879,  445.1042,  579.2620,  542.5791],
        [ 995.0483,  291.3572, 1198.4941,  343.0112],
        [1041.4304,  462.1721, 1278.9719,  525.6843],
        [1024.3557,  356.6491, 1205.7195,  415.9249],
        [ 401.5469,  646.8911,  911.3799,  720.0000]], device='cuda:0')
xyxyn: tensor([[0.1374, 0.4657, 0.2852, 0.5413],
        [0.2121, 0.6182, 0.4525, 0.7536],
        [0.7774, 0.4047, 0.9363, 0.4764],
        [0.8136, 0.6419, 0.9992, 0.7301],
        [0.8003, 0.4953, 0.9420, 0.5777],
        [0.3137, 0.8985, 0.7120, 1.0000]], device='cuda:0')

0: 384x640 5 Potholes, 14.3ms
Speed: 2.5ms preprocess, 14.3ms inference, 1.8ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.9153, 0.8854, 0.8055, 0.7157, 0.5620], device='cuda:0')
data: tensor([[2.7330e+02, 4.5149e+02, 5.8530e+02, 5.5451e+02, 9.1525e-01, 0.0000e+00],
        [1.7395e+02, 3.3702e+02, 3.5362e+02, 3.9468e+02, 8.8539e-01, 0.0000e+00],
        [1.0001e+03, 2.9693e+02, 1.2102e+03, 3.4519e+02, 8.0555e-01, 0.0000e+00],
        [1.0271e+03, 3.6542e+02, 1.2195e+03, 4.2123e+02, 7.1569e-01, 0.0000e+00],
        [1.0524e+03, 4.7813e+02, 1.2799e+03, 5.3328e+02, 5.6200e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([5, 6])
xywh: tensor([[ 429.2978,  503.0001,  312.0005,  103.0166],
        [ 263.7823,  365.8487,  179.6695,   57.6550],
        [1105.1366,  321.0610,  210.0957,   48.2522],
        [1123.3071,  393.3216,  192.3308,   55.8120],
        [1166.1511,  505.7039,  227.5471,   55.1516]], device='cuda:0')
xywhn: tensor([[0.3354, 0.6986, 0.2438, 0.1431],
        [0.2061, 0.5081, 0.1404, 0.0801],
        [0.8634, 0.4459, 0.1641, 0.0670],
        [0.8776, 0.5463, 0.1503, 0.0775],
        [0.9111, 0.7024, 0.1778, 0.0766]], device='cuda:0')
xyxy: tensor([[ 273.2975,  451.4918,  585.2980,  554.5084],
        [ 173.9475,  337.0212,  353.6171,  394.6762],
        [1000.0887,  296.9349, 1210.1844,  345.1871],
        [1027.1417,  365.4156, 1219.4725,  421.2276],
        [1052.3776,  478.1280, 1279.9247,  533.2797]], device='cuda:0')
xyxyn: tensor([[0.2135, 0.6271, 0.4573, 0.7702],
        [0.1359, 0.4681, 0.2763, 0.5482],
        [0.7813, 0.4124, 0.9455, 0.4794],
        [0.8025, 0.5075, 0.9527, 0.5850],
        [0.8222, 0.6641, 0.9999, 0.7407]], device='cuda:0')

0: 384x640 5 Potholes, 14.5ms
Speed: 2.0ms preprocess, 14.5ms inference, 1.8ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.9059, 0.8888, 0.8153, 0.7490, 0.6555], device='cuda:0')
data: tensor([[2.6982e+02, 4.6266e+02, 5.8183e+02, 5.6702e+02, 9.0594e-01, 0.0000e+00],
        [1.6610e+02, 3.4220e+02, 3.5493e+02, 4.0014e+02, 8.8882e-01, 0.0000e+00],
        [1.0030e+03, 2.9719e+02, 1.2162e+03, 3.4747e+02, 8.1533e-01, 0.0000e+00],
        [1.0393e+03, 3.7085e+02, 1.2272e+03, 4.3267e+02, 7.4903e-01, 0.0000e+00],
        [1.1111e+03, 4.8781e+02, 1.2800e+03, 5.4297e+02, 6.5548e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([5, 6])
xywh: tensor([[ 425.8244,  514.8431,  312.0143,  104.3581],
        [ 260.5147,  371.1722,  188.8331,   57.9355],
        [1109.6147,  322.3306,  213.1321,   50.2713],
        [1133.2372,  401.7621,  187.9272,   61.8208],
        [1195.5591,  515.3937,  168.8818,   55.1588]], device='cuda:0')
xywhn: tensor([[0.3327, 0.7151, 0.2438, 0.1449],
        [0.2035, 0.5155, 0.1475, 0.0805],
        [0.8669, 0.4477, 0.1665, 0.0698],
        [0.8853, 0.5580, 0.1468, 0.0859],
        [0.9340, 0.7158, 0.1319, 0.0766]], device='cuda:0')
xyxy: tensor([[ 269.8173,  462.6641,  581.8315,  567.0222],
        [ 166.0982,  342.2045,  354.9313,  400.1400],
        [1003.0487,  297.1950, 1216.1808,  347.4663],
        [1039.2736,  370.8517, 1227.2008,  432.6725],
        [1111.1182,  487.8143, 1280.0000,  542.9731]], device='cuda:0')
xyxyn: tensor([[0.2108, 0.6426, 0.4546, 0.7875],
        [0.1298, 0.4753, 0.2773, 0.5558],
        [0.7836, 0.4128, 0.9501, 0.4826],
        [0.8119, 0.5151, 0.9588, 0.6009],
        [0.8681, 0.6775, 1.0000, 0.7541]], device='cuda:0')

0: 384x640 5 Potholes, 11.7ms
Speed: 1.9ms preprocess, 11.7ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.9025, 0.8954, 0.8197, 0.7528, 0.2861], device='cuda:0')
data: tensor([[2.5732e+02, 4.7995e+02, 5.8741e+02, 5.9360e+02, 9.0247e-01, 0.0000e+00],
        [1.5166e+02, 3.5067e+02, 3.5115e+02, 4.0980e+02, 8.9536e-01, 0.0000e+00],
        [1.0062e+03, 3.0224e+02, 1.2325e+03, 3.5691e+02, 8.1974e-01, 0.0000e+00],
        [1.0453e+03, 3.7973e+02, 1.2491e+03, 4.3762e+02, 7.5277e-01, 0.0000e+00],
        [1.1271e+03, 5.0752e+02, 1.2800e+03, 5.6890e+02, 2.8612e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([5, 6])
xywh: tensor([[ 422.3660,  536.7726,  330.0975,  113.6520],
        [ 251.4062,  380.2368,  199.4849,   59.1238],
        [1119.3514,  329.5754,  226.2122,   54.6777],
        [1147.2255,  408.6749,  203.7793,   57.8822],
        [1203.5468,  538.2077,  152.9065,   61.3837]], device='cuda:0')
xywhn: tensor([[0.3300, 0.7455, 0.2579, 0.1578],
        [0.1964, 0.5281, 0.1558, 0.0821],
        [0.8745, 0.4577, 0.1767, 0.0759],
        [0.8963, 0.5676, 0.1592, 0.0804],
        [0.9403, 0.7475, 0.1195, 0.0853]], device='cuda:0')
xyxy: tensor([[ 257.3173,  479.9467,  587.4148,  593.5986],
        [ 151.6638,  350.6749,  351.1487,  409.7987],
        [1006.2454,  302.2365, 1232.4575,  356.9142],
        [1045.3358,  379.7338, 1249.1151,  437.6160],
        [1127.0935,  507.5159, 1280.0000,  568.8995]], device='cuda:0')
xyxyn: tensor([[0.2010, 0.6666, 0.4589, 0.8244],
        [0.1185, 0.4870, 0.2743, 0.5692],
        [0.7861, 0.4198, 0.9629, 0.4957],
        [0.8167, 0.5274, 0.9759, 0.6078],
        [0.8805, 0.7049, 1.0000, 0.7901]], device='cuda:0')

0: 384x640 4 Potholes, 12.6ms
Speed: 2.0ms preprocess, 12.6ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.8974, 0.8605, 0.8183, 0.8080], device='cuda:0')
data: tensor([[2.4921e+02, 4.8463e+02, 5.9256e+02, 6.0671e+02, 8.9743e-01, 0.0000e+00],
        [1.4045e+02, 3.5460e+02, 3.5257e+02, 4.1685e+02, 8.6050e-01, 0.0000e+00],
        [1.0184e+03, 3.0376e+02, 1.2344e+03, 3.5977e+02, 8.1832e-01, 0.0000e+00],
        [1.0709e+03, 3.8459e+02, 1.2663e+03, 4.4465e+02, 8.0803e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([4, 6])
xywh: tensor([[ 420.8865,  545.6709,  343.3433,  122.0726],
        [ 246.5131,  385.7249,  212.1180,   62.2484],
        [1126.3813,  331.7638,  215.9980,   56.0093],
        [1168.6047,  414.6180,  195.3584,   60.0616]], device='cuda:0')
xywhn: tensor([[0.3288, 0.7579, 0.2682, 0.1695],
        [0.1926, 0.5357, 0.1657, 0.0865],
        [0.8800, 0.4608, 0.1687, 0.0778],
        [0.9130, 0.5759, 0.1526, 0.0834]], device='cuda:0')
xyxy: tensor([[ 249.2149,  484.6346,  592.5582,  606.7072],
        [ 140.4541,  354.6006,  352.5721,  416.8491],
        [1018.3824,  303.7592, 1234.3804,  359.7684],
        [1070.9255,  384.5872, 1266.2839,  444.6488]], device='cuda:0')
xyxyn: tensor([[0.1947, 0.6731, 0.4629, 0.8426],
        [0.1097, 0.4925, 0.2754, 0.5790],
        [0.7956, 0.4219, 0.9644, 0.4997],
        [0.8367, 0.5341, 0.9893, 0.6176]], device='cuda:0')

0: 384x640 5 Potholes, 13.9ms
Speed: 1.9ms preprocess, 13.9ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.9079, 0.9010, 0.8304, 0.7918, 0.2723], device='cuda:0')
data: tensor([[1.4330e+02, 3.6121e+02, 3.4324e+02, 4.2260e+02, 9.0787e-01, 0.0000e+00],
        [2.3248e+02, 4.9477e+02, 5.8585e+02, 6.2343e+02, 9.0095e-01, 0.0000e+00],
        [1.0304e+03, 3.0709e+02, 1.2552e+03, 3.6509e+02, 8.3040e-01, 0.0000e+00],
        [1.0806e+03, 3.8837e+02, 1.2771e+03, 4.5192e+02, 7.9181e-01, 0.0000e+00],
        [1.2520e+02, 4.9257e+02, 2.1433e+02, 5.3143e+02, 2.7227e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([5, 6])
xywh: tensor([[ 243.2693,  391.9066,  199.9359,   61.3869],
        [ 409.1644,  559.1000,  353.3755,  128.6606],
        [1142.8096,  336.0881,  224.8369,   58.0056],
        [1178.8707,  420.1444,  196.4905,   63.5583],
        [ 169.7680,  511.9968,   89.1328,   38.8623]], device='cuda:0')
xywhn: tensor([[0.1901, 0.5443, 0.1562, 0.0853],
        [0.3197, 0.7765, 0.2761, 0.1787],
        [0.8928, 0.4668, 0.1757, 0.0806],
        [0.9210, 0.5835, 0.1535, 0.0883],
        [0.1326, 0.7111, 0.0696, 0.0540]], device='cuda:0')
xyxy: tensor([[ 143.3014,  361.2132,  343.2372,  422.6001],
        [ 232.4767,  494.7697,  585.8522,  623.4303],
        [1030.3911,  307.0853, 1255.2280,  365.0909],
        [1080.6255,  388.3652, 1277.1160,  451.9236],
        [ 125.2016,  492.5657,  214.3344,  531.4280]], device='cuda:0')
xyxyn: tensor([[0.1120, 0.5017, 0.2682, 0.5869],
        [0.1816, 0.6872, 0.4577, 0.8659],
        [0.8050, 0.4265, 0.9806, 0.5071],
        [0.8442, 0.5394, 0.9977, 0.6277],
        [0.0978, 0.6841, 0.1674, 0.7381]], device='cuda:0')

0: 384x640 5 Potholes, 17.3ms
Speed: 1.9ms preprocess, 17.3ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.9057, 0.8453, 0.8298, 0.6058, 0.5021], device='cuda:0')
data: tensor([[2.2882e+02, 4.9991e+02, 5.9132e+02, 6.3426e+02, 9.0574e-01, 0.0000e+00],
        [1.3525e+02, 3.6565e+02, 3.4174e+02, 4.2999e+02, 8.4531e-01, 0.0000e+00],
        [1.0377e+03, 3.0777e+02, 1.2648e+03, 3.6682e+02, 8.2984e-01, 0.0000e+00],
        [1.0678e+03, 3.9290e+02, 1.2800e+03, 4.6328e+02, 6.0578e-01, 0.0000e+00],
        [1.1834e+03, 5.3705e+02, 1.2799e+03, 6.0032e+02, 5.0211e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([5, 6])
xywh: tensor([[ 410.0727,  567.0833,  362.5038,  134.3499],
        [ 238.4975,  397.8190,  206.4908,   64.3374],
        [1151.2478,  337.2955,  227.0828,   59.0563],
        [1173.9202,  428.0930,  212.1597,   70.3806],
        [1231.6453,  568.6847,   96.4536,   63.2690]], device='cuda:0')
xywhn: tensor([[0.3204, 0.7876, 0.2832, 0.1866],
        [0.1863, 0.5525, 0.1613, 0.0894],
        [0.8994, 0.4685, 0.1774, 0.0820],
        [0.9171, 0.5946, 0.1657, 0.0978],
        [0.9622, 0.7898, 0.0754, 0.0879]], device='cuda:0')
xyxy: tensor([[ 228.8207,  499.9083,  591.3246,  634.2582],
        [ 135.2522,  365.6503,  341.7429,  429.9877],
        [1037.7064,  307.7674, 1264.7892,  366.8237],
        [1067.8403,  392.9027, 1280.0000,  463.2833],
        [1183.4185,  537.0502, 1279.8721,  600.3192]], device='cuda:0')
xyxyn: tensor([[0.1788, 0.6943, 0.4620, 0.8809],
        [0.1057, 0.5078, 0.2670, 0.5972],
        [0.8107, 0.4275, 0.9881, 0.5095],
        [0.8343, 0.5457, 1.0000, 0.6434],
        [0.9245, 0.7459, 0.9999, 0.8338]], device='cuda:0')

0: 384x640 5 Potholes, 17.5ms
Speed: 2.1ms preprocess, 17.5ms inference, 1.8ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.8788, 0.8531, 0.8292, 0.3146, 0.2553], device='cuda:0')
data: tensor([[1.1961e+02, 3.6981e+02, 3.3789e+02, 4.3859e+02, 8.7882e-01, 0.0000e+00],
        [2.0283e+02, 5.2182e+02, 5.9101e+02, 6.6472e+02, 8.5315e-01, 0.0000e+00],
        [1.0495e+03, 3.1271e+02, 1.2767e+03, 3.7489e+02, 8.2917e-01, 0.0000e+00],
        [1.1080e+03, 4.0086e+02, 1.2800e+03, 4.7217e+02, 3.1459e-01, 0.0000e+00],
        [9.5193e+01, 5.1840e+02, 1.9603e+02, 5.6633e+02, 2.5532e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([5, 6])
xywh: tensor([[ 228.7503,  404.1996,  218.2861,   68.7839],
        [ 396.9185,  593.2703,  388.1750,  142.9020],
        [1163.0870,  343.7972,  227.2034,   62.1830],
        [1193.9951,  436.5161,  172.0098,   71.3063],
        [ 145.6093,  542.3640,  100.8331,   47.9274]], device='cuda:0')
xywhn: tensor([[0.1787, 0.5614, 0.1705, 0.0955],
        [0.3101, 0.8240, 0.3033, 0.1985],
        [0.9087, 0.4775, 0.1775, 0.0864],
        [0.9328, 0.6063, 0.1344, 0.0990],
        [0.1138, 0.7533, 0.0788, 0.0666]], device='cuda:0')
xyxy: tensor([[ 119.6072,  369.8077,  337.8934,  438.5916],
        [ 202.8309,  521.8193,  591.0060,  664.7213],
        [1049.4854,  312.7057, 1276.6887,  374.8887],
        [1107.9902,  400.8629, 1280.0000,  472.1693],
        [  95.1928,  518.4003,  196.0258,  566.3277]], device='cuda:0')
xyxyn: tensor([[0.0934, 0.5136, 0.2640, 0.6092],
        [0.1585, 0.7247, 0.4617, 0.9232],
        [0.8199, 0.4343, 0.9974, 0.5207],
        [0.8656, 0.5568, 1.0000, 0.6558],
        [0.0744, 0.7200, 0.1531, 0.7866]], device='cuda:0')

0: 384x640 6 Potholes, 14.2ms
Speed: 2.0ms preprocess, 14.2ms inference, 2.6ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.9099, 0.9064, 0.8511, 0.6001, 0.3420, 0.3022], device='cuda:0')
data: tensor([[1.1519e+02, 3.7793e+02, 3.3685e+02, 4.4500e+02, 9.0994e-01, 0.0000e+00],
        [1.9223e+02, 5.3116e+02, 5.8904e+02, 6.9539e+02, 9.0637e-01, 0.0000e+00],
        [1.0525e+03, 3.1637e+02, 1.2800e+03, 3.7954e+02, 8.5114e-01, 0.0000e+00],
        [1.1196e+03, 4.0589e+02, 1.2800e+03, 4.7405e+02, 6.0014e-01, 0.0000e+00],
        [1.0840e+03, 3.9415e+02, 1.2800e+03, 4.7395e+02, 3.4195e-01, 0.0000e+00],
        [1.2314e+03, 5.6814e+02, 1.2797e+03, 6.3418e+02, 3.0222e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([6, 6])
xywh: tensor([[ 226.0211,  411.4642,  221.6622,   67.0629],
        [ 390.6338,  613.2737,  396.8086,  164.2275],
        [1166.2257,  347.9525,  227.5486,   63.1741],
        [1199.8197,  439.9735,  160.3606,   68.1617],
        [1182.0210,  434.0507,  195.9580,   79.7986],
        [1255.5304,  601.1609,   48.3230,   66.0430]], device='cuda:0')
xywhn: tensor([[0.1766, 0.5715, 0.1732, 0.0931],
        [0.3052, 0.8518, 0.3100, 0.2281],
        [0.9111, 0.4833, 0.1778, 0.0877],
        [0.9374, 0.6111, 0.1253, 0.0947],
        [0.9235, 0.6028, 0.1531, 0.1108],
        [0.9809, 0.8349, 0.0378, 0.0917]], device='cuda:0')
xyxy: tensor([[ 115.1899,  377.9328,  336.8522,  444.9957],
        [ 192.2295,  531.1599,  589.0381,  695.3875],
        [1052.4514,  316.3655, 1280.0000,  379.5396],
        [1119.6394,  405.8926, 1280.0000,  474.0544],
        [1084.0420,  394.1514, 1280.0000,  473.9500],
        [1231.3689,  568.1394, 1279.6919,  634.1824]], device='cuda:0')
xyxyn: tensor([[0.0900, 0.5249, 0.2632, 0.6180],
        [0.1502, 0.7377, 0.4602, 0.9658],
        [0.8222, 0.4394, 1.0000, 0.5271],
        [0.8747, 0.5637, 1.0000, 0.6584],
        [0.8469, 0.5474, 1.0000, 0.6583],
        [0.9620, 0.7891, 0.9998, 0.8808]], device='cuda:0')

0: 384x640 3 Potholes, 15.2ms
Speed: 2.0ms preprocess, 15.2ms inference, 2.7ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0.], device='cuda:0')
conf: tensor([0.9030, 0.8905, 0.8391], device='cuda:0')
data: tensor([[1.0296e+02, 3.8198e+02, 3.3437e+02, 4.4890e+02, 9.0305e-01, 0.0000e+00],
        [1.8171e+02, 5.4272e+02, 6.0029e+02, 7.1012e+02, 8.9053e-01, 0.0000e+00],
        [1.0659e+03, 3.1845e+02, 1.2800e+03, 3.8085e+02, 8.3908e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([3, 6])
xywh: tensor([[ 218.6676,  415.4417,  231.4082,   66.9141],
        [ 390.9991,  626.4197,  418.5845,  167.4061],
        [1172.9434,  349.6505,  214.1133,   62.4034]], device='cuda:0')
xywhn: tensor([[0.1708, 0.5770, 0.1808, 0.0929],
        [0.3055, 0.8700, 0.3270, 0.2325],
        [0.9164, 0.4856, 0.1673, 0.0867]], device='cuda:0')
xyxy: tensor([[ 102.9636,  381.9846,  334.3717,  448.8987],
        [ 181.7068,  542.7166,  600.2914,  710.1227],
        [1065.8867,  318.4488, 1280.0000,  380.8522]], device='cuda:0')
xyxyn: tensor([[0.0804, 0.5305, 0.2612, 0.6235],
        [0.1420, 0.7538, 0.4690, 0.9863],
        [0.8327, 0.4423, 1.0000, 0.5290]], device='cuda:0')

0: 384x640 4 Potholes, 13.8ms
Speed: 2.1ms preprocess, 13.8ms inference, 1.8ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.8935, 0.8838, 0.8157, 0.3240], device='cuda:0')
data: tensor([[8.6686e+01, 3.9123e+02, 3.2903e+02, 4.6778e+02, 8.9348e-01, 0.0000e+00],
        [1.6381e+02, 5.6256e+02, 6.0901e+02, 7.2000e+02, 8.8382e-01, 0.0000e+00],
        [1.0788e+03, 3.2327e+02, 1.2800e+03, 3.8771e+02, 8.1572e-01, 0.0000e+00],
        [5.1474e+01, 5.5923e+02, 1.6145e+02, 6.1645e+02, 3.2401e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([4, 6])
xywh: tensor([[ 207.8573,  429.5037,  242.3417,   76.5516],
        [ 386.4109,  641.2808,  445.2032,  157.4385],
        [1179.4086,  355.4894,  201.1829,   64.4414],
        [ 106.4644,  587.8386,  109.9811,   57.2156]], device='cuda:0')
xywhn: tensor([[0.1624, 0.5965, 0.1893, 0.1063],
        [0.3019, 0.8907, 0.3478, 0.2187],
        [0.9214, 0.4937, 0.1572, 0.0895],
        [0.0832, 0.8164, 0.0859, 0.0795]], device='cuda:0')
xyxy: tensor([[  86.6864,  391.2279,  329.0282,  467.7795],
        [ 163.8093,  562.5615,  609.0125,  720.0000],
        [1078.8171,  323.2687, 1280.0000,  387.7101],
        [  51.4738,  559.2308,  161.4549,  616.4464]], device='cuda:0')
xyxyn: tensor([[0.0677, 0.5434, 0.2571, 0.6497],
        [0.1280, 0.7813, 0.4758, 1.0000],
        [0.8428, 0.4490, 1.0000, 0.5385],
        [0.0402, 0.7767, 0.1261, 0.8562]], device='cuda:0')

0: 384x640 3 Potholes, 19.5ms
Speed: 2.4ms preprocess, 19.5ms inference, 2.4ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0.], device='cuda:0')
conf: tensor([0.8968, 0.7858, 0.7842], device='cuda:0')
data: tensor([[8.4943e+01, 3.9391e+02, 3.2378e+02, 4.7444e+02, 8.9682e-01, 0.0000e+00],
        [1.6168e+02, 5.7929e+02, 6.1694e+02, 7.2000e+02, 7.8584e-01, 0.0000e+00],
        [1.0848e+03, 3.2474e+02, 1.2800e+03, 3.9171e+02, 7.8424e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([3, 6])
xywh: tensor([[ 204.3589,  434.1775,  238.8325,   80.5303],
        [ 389.3147,  649.6439,  455.2598,  140.7123],
        [1182.3776,  358.2232,  195.2449,   66.9743]], device='cuda:0')
xywhn: tensor([[0.1597, 0.6030, 0.1866, 0.1118],
        [0.3042, 0.9023, 0.3557, 0.1954],
        [0.9237, 0.4975, 0.1525, 0.0930]], device='cuda:0')
xyxy: tensor([[  84.9427,  393.9123,  323.7752,  474.4426],
        [ 161.6848,  579.2877,  616.9446,  720.0000],
        [1084.7551,  324.7360, 1280.0000,  391.7103]], device='cuda:0')
xyxyn: tensor([[0.0664, 0.5471, 0.2529, 0.6589],
        [0.1263, 0.8046, 0.4820, 1.0000],
        [0.8475, 0.4510, 1.0000, 0.5440]], device='cuda:0')

0: 384x640 3 Potholes, 10.6ms
Speed: 2.1ms preprocess, 10.6ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0.], device='cuda:0')
conf: tensor([0.8943, 0.8041, 0.7713], device='cuda:0')
data: tensor([[6.7548e+01, 3.9914e+02, 3.2108e+02, 4.7943e+02, 8.9430e-01, 0.0000e+00],
        [1.0888e+03, 3.2679e+02, 1.2800e+03, 3.9777e+02, 8.0412e-01, 0.0000e+00],
        [1.6349e+02, 5.9474e+02, 6.1267e+02, 7.2000e+02, 7.7132e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([3, 6])
xywh: tensor([[ 194.3140,  439.2866,  253.5312,   80.2922],
        [1184.4086,  362.2819,  191.1829,   70.9772],
        [ 388.0792,  657.3680,  449.1819,  125.2640]], device='cuda:0')
xywhn: tensor([[0.1518, 0.6101, 0.1981, 0.1115],
        [0.9253, 0.5032, 0.1494, 0.0986],
        [0.3032, 0.9130, 0.3509, 0.1740]], device='cuda:0')
xyxy: tensor([[  67.5483,  399.1405,  321.0796,  479.4326],
        [1088.8171,  326.7933, 1280.0000,  397.7705],
        [ 163.4883,  594.7360,  612.6702,  720.0000]], device='cuda:0')
xyxyn: tensor([[0.0528, 0.5544, 0.2508, 0.6659],
        [0.8506, 0.4539, 1.0000, 0.5525],
        [0.1277, 0.8260, 0.4786, 1.0000]], device='cuda:0')

0: 384x640 3 Potholes, 17.7ms
Speed: 3.2ms preprocess, 17.7ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0.], device='cuda:0')
conf: tensor([0.9016, 0.7722, 0.7511], device='cuda:0')
data: tensor([[4.7786e+01, 4.1101e+02, 3.1304e+02, 5.0156e+02, 9.0164e-01, 0.0000e+00],
        [3.2614e+02, 6.1386e+02, 6.1001e+02, 7.2000e+02, 7.7221e-01, 0.0000e+00],
        [1.1059e+03, 3.3298e+02, 1.2800e+03, 4.0544e+02, 7.5107e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([3, 6])
xywh: tensor([[ 180.4151,  456.2849,  265.2592,   90.5568],
        [ 468.0721,  666.9298,  283.8673,  106.1404],
        [1192.9456,  369.2070,  174.1088,   72.4586]], device='cuda:0')
xywhn: tensor([[0.1409, 0.6337, 0.2072, 0.1258],
        [0.3657, 0.9263, 0.2218, 0.1474],
        [0.9320, 0.5128, 0.1360, 0.1006]], device='cuda:0')
xyxy: tensor([[  47.7855,  411.0065,  313.0447,  501.5633],
        [ 326.1384,  613.8596,  610.0057,  720.0000],
        [1105.8912,  332.9777, 1280.0000,  405.4363]], device='cuda:0')
xyxyn: tensor([[0.0373, 0.5708, 0.2446, 0.6966],
        [0.2548, 0.8526, 0.4766, 1.0000],
        [0.8640, 0.4625, 1.0000, 0.5631]], device='cuda:0')

0: 384x640 3 Potholes, 13.1ms
Speed: 2.0ms preprocess, 13.1ms inference, 2.0ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0.], device='cuda:0')
conf: tensor([0.8943, 0.7044, 0.6895], device='cuda:0')
data: tensor([[3.6990e+01, 4.1959e+02, 3.0722e+02, 5.0934e+02, 8.9427e-01, 0.0000e+00],
        [3.4729e+02, 6.2742e+02, 6.1856e+02, 7.2000e+02, 7.0440e-01, 0.0000e+00],
        [1.1144e+03, 3.3415e+02, 1.2800e+03, 4.0844e+02, 6.8952e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([3, 6])
xywh: tensor([[ 172.1032,  464.4620,  270.2268,   89.7531],
        [ 482.9271,  673.7086,  271.2717,   92.5828],
        [1197.2246,  371.2938,  165.5509,   74.2922]], device='cuda:0')
xywhn: tensor([[0.1345, 0.6451, 0.2111, 0.1247],
        [0.3773, 0.9357, 0.2119, 0.1286],
        [0.9353, 0.5157, 0.1293, 0.1032]], device='cuda:0')
xyxy: tensor([[  36.9898,  419.5855,  307.2166,  509.3386],
        [ 347.2913,  627.4172,  618.5630,  720.0000],
        [1114.4491,  334.1477, 1280.0000,  408.4399]], device='cuda:0')
xyxyn: tensor([[0.0289, 0.5828, 0.2400, 0.7074],
        [0.2713, 0.8714, 0.4833, 1.0000],
        [0.8707, 0.4641, 1.0000, 0.5673]], device='cuda:0')

0: 384x640 3 Potholes, 13.3ms
Speed: 2.0ms preprocess, 13.3ms inference, 5.0ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0.], device='cuda:0')
conf: tensor([0.9338, 0.6757, 0.4526], device='cuda:0')
data: tensor([[3.3771e+01, 4.2353e+02, 3.0266e+02, 5.1761e+02, 9.3375e-01, 0.0000e+00],
        [1.1238e+03, 3.3782e+02, 1.2800e+03, 4.1216e+02, 6.7574e-01, 0.0000e+00],
        [3.8487e+02, 6.3957e+02, 5.9865e+02, 7.2000e+02, 4.5258e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([3, 6])
xywh: tensor([[ 168.2136,  470.5687,  268.8852,   94.0820],
        [1201.8870,  374.9902,  156.2261,   74.3407],
        [ 491.7645,  679.7827,  213.7791,   80.4347]], device='cuda:0')
xywhn: tensor([[0.1314, 0.6536, 0.2101, 0.1307],
        [0.9390, 0.5208, 0.1221, 0.1033],
        [0.3842, 0.9441, 0.1670, 0.1117]], device='cuda:0')
xyxy: tensor([[  33.7710,  423.5276,  302.6562,  517.6097],
        [1123.7739,  337.8199, 1280.0000,  412.1606],
        [ 384.8749,  639.5653,  598.6540,  720.0000]], device='cuda:0')
xyxyn: tensor([[0.0264, 0.5882, 0.2365, 0.7189],
        [0.8779, 0.4692, 1.0000, 0.5724],
        [0.3007, 0.8883, 0.4677, 1.0000]], device='cuda:0')

0: 384x640 3 Potholes, 14.1ms
Speed: 2.1ms preprocess, 14.1ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0.], device='cuda:0')
conf: tensor([0.8859, 0.5276, 0.3963], device='cuda:0')
data: tensor([[1.1920e+01, 4.2902e+02, 3.0064e+02, 5.3004e+02, 8.8595e-01, 0.0000e+00],
        [1.1294e+03, 3.3700e+02, 1.2800e+03, 4.1963e+02, 5.2760e-01, 0.0000e+00],
        [1.1836e+01, 1.7633e+02, 1.2679e+03, 6.7155e+02, 3.9627e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([3, 6])
xywh: tensor([[ 156.2796,  479.5336,  288.7189,  101.0197],
        [1204.7036,  378.3176,  150.5928,   82.6318],
        [ 639.8513,  423.9415, 1256.0309,  495.2174]], device='cuda:0')
xywhn: tensor([[0.1221, 0.6660, 0.2256, 0.1403],
        [0.9412, 0.5254, 0.1177, 0.1148],
        [0.4999, 0.5888, 0.9813, 0.6878]], device='cuda:0')
xyxy: tensor([[  11.9202,  429.0238,  300.6390,  530.0435],
        [1129.4072,  337.0017, 1280.0000,  419.6335],
        [  11.8358,  176.3328, 1267.8667,  671.5502]], device='cuda:0')
xyxyn: tensor([[0.0093, 0.5959, 0.2349, 0.7362],
        [0.8823, 0.4681, 1.0000, 0.5828],
        [0.0092, 0.2449, 0.9905, 0.9327]], device='cuda:0')

0: 384x640 2 Potholes, 11.5ms
Speed: 1.9ms preprocess, 11.5ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0.], device='cuda:0')
conf: tensor([0.9082, 0.3831], device='cuda:0')
data: tensor([[1.1503e+00, 4.4308e+02, 2.9016e+02, 5.5373e+02, 9.0823e-01, 0.0000e+00],
        [2.8474e+00, 1.7859e+02, 1.2729e+03, 7.1733e+02, 3.8313e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([2, 6])
xywh: tensor([[ 145.6537,  498.4039,  289.0067,  110.6514],
        [ 637.8898,  447.9588, 1270.0847,  538.7396]], device='cuda:0')
xywhn: tensor([[0.1138, 0.6922, 0.2258, 0.1537],
        [0.4984, 0.6222, 0.9923, 0.7482]], device='cuda:0')
xyxy: tensor([[1.1503e+00, 4.4308e+02, 2.9016e+02, 5.5373e+02],
        [2.8474e+00, 1.7859e+02, 1.2729e+03, 7.1733e+02]], device='cuda:0')
xyxyn: tensor([[8.9870e-04, 6.1539e-01, 2.2669e-01, 7.6907e-01],
        [2.2245e-03, 2.4804e-01, 9.9448e-01, 9.9629e-01]], device='cuda:0')

0: 384x640 3 Potholes, 10.0ms
Speed: 1.9ms preprocess, 10.0ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0.], device='cuda:0')
conf: tensor([0.9192, 0.2839, 0.2623], device='cuda:0')
data: tensor([[1.3034e+00, 4.5111e+02, 2.8660e+02, 5.6793e+02, 9.1924e-01, 0.0000e+00],
        [8.6151e+01, 1.7516e+02, 1.2685e+03, 6.9650e+02, 2.8391e-01, 0.0000e+00],
        [1.1504e+03, 3.5235e+02, 1.2799e+03, 4.3534e+02, 2.6230e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([3, 6])
xywh: tensor([[ 143.9521,  509.5197,  285.2975,  116.8108],
        [ 677.3242,  435.8303, 1182.3470,  521.3411],
        [1215.1775,  393.8480,  129.4565,   82.9906]], device='cuda:0')
xywhn: tensor([[0.1125, 0.7077, 0.2229, 0.1622],
        [0.5292, 0.6053, 0.9237, 0.7241],
        [0.9494, 0.5470, 0.1011, 0.1153]], device='cuda:0')
xyxy: tensor([[   1.3034,  451.1143,  286.6009,  567.9251],
        [  86.1506,  175.1598, 1268.4977,  696.5009],
        [1150.4492,  352.3527, 1279.9058,  435.3433]], device='cuda:0')
xyxyn: tensor([[0.0010, 0.6265, 0.2239, 0.7888],
        [0.0673, 0.2433, 0.9910, 0.9674],
        [0.8988, 0.4894, 0.9999, 0.6046]], device='cuda:0')

0: 384x640 3 Potholes, 14.5ms
Speed: 1.9ms preprocess, 14.5ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0.], device='cuda:0')
conf: tensor([0.9217, 0.4795, 0.3904], device='cuda:0')
data: tensor([[1.6208e+00, 4.5666e+02, 2.8114e+02, 5.7517e+02, 9.2171e-01, 0.0000e+00],
        [1.1630e+03, 3.5246e+02, 1.2798e+03, 4.2997e+02, 4.7951e-01, 0.0000e+00],
        [2.1562e+02, 1.7751e+02, 1.2751e+03, 6.9927e+02, 3.9037e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([3, 6])
xywh: tensor([[ 141.3798,  515.9163,  279.5181,  118.5162],
        [1221.3790,  391.2127,  116.8530,   77.5070],
        [ 745.3522,  438.3915, 1059.4590,  521.7534]], device='cuda:0')
xywhn: tensor([[0.1105, 0.7166, 0.2184, 0.1646],
        [0.9542, 0.5434, 0.0913, 0.1076],
        [0.5823, 0.6089, 0.8277, 0.7247]], device='cuda:0')
xyxy: tensor([[   1.6208,  456.6581,  281.1389,  575.1744],
        [1162.9525,  352.4592, 1279.8055,  429.9662],
        [ 215.6227,  177.5148, 1275.0817,  699.2682]], device='cuda:0')
xyxyn: tensor([[0.0013, 0.6342, 0.2196, 0.7989],
        [0.9086, 0.4895, 0.9998, 0.5972],
        [0.1685, 0.2465, 0.9962, 0.9712]], device='cuda:0')

0: 384x640 4 Potholes, 11.2ms
Speed: 1.9ms preprocess, 11.2ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.8861, 0.4624, 0.4621, 0.3735], device='cuda:0')
data: tensor([[1.9632e-01, 4.7486e+02, 2.6679e+02, 6.0358e+02, 8.8615e-01, 0.0000e+00],
        [1.1873e+03, 3.6073e+02, 1.2798e+03, 4.3569e+02, 4.6240e-01, 0.0000e+00],
        [2.1953e+02, 1.7637e+02, 1.2770e+03, 7.2000e+02, 4.6214e-01, 0.0000e+00],
        [4.2212e+02, 5.8822e+02, 1.1626e+03, 7.2000e+02, 3.7354e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([4, 6])
xywh: tensor([[ 133.4941,  539.2220,  266.5956,  128.7196],
        [1233.5276,  398.2098,   92.5364,   74.9608],
        [ 748.2644,  448.1840, 1057.4648,  543.6320],
        [ 792.3555,  654.1079,  740.4618,  131.7841]], device='cuda:0')
xywhn: tensor([[0.1043, 0.7489, 0.2083, 0.1788],
        [0.9637, 0.5531, 0.0723, 0.1041],
        [0.5846, 0.6225, 0.8261, 0.7550],
        [0.6190, 0.9085, 0.5785, 0.1830]], device='cuda:0')
xyxy: tensor([[1.9632e-01, 4.7486e+02, 2.6679e+02, 6.0358e+02],
        [1.1873e+03, 3.6073e+02, 1.2798e+03, 4.3569e+02],
        [2.1953e+02, 1.7637e+02, 1.2770e+03, 7.2000e+02],
        [4.2212e+02, 5.8822e+02, 1.1626e+03, 7.2000e+02]], device='cuda:0')
xyxyn: tensor([[1.5337e-04, 6.5953e-01, 2.0843e-01, 8.3831e-01],
        [9.2755e-01, 5.0101e-01, 9.9984e-01, 6.0513e-01],
        [1.7151e-01, 2.4496e-01, 9.9765e-01, 1.0000e+00],
        [3.2978e-01, 8.1697e-01, 9.0827e-01, 1.0000e+00]], device='cuda:0')

0: 384x640 4 Potholes, 15.1ms
Speed: 2.0ms preprocess, 15.1ms inference, 7.4ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.8377, 0.7923, 0.6077, 0.3408], device='cuda:0')
data: tensor([[0.0000e+00, 4.8207e+02, 2.6564e+02, 7.0320e+02, 8.3773e-01, 0.0000e+00],
        [5.2856e-01, 4.8379e+02, 2.7043e+02, 6.2373e+02, 7.9228e-01, 0.0000e+00],
        [1.1964e+03, 3.6043e+02, 1.2798e+03, 4.3521e+02, 6.0774e-01, 0.0000e+00],
        [2.1285e+02, 1.7668e+02, 1.2771e+03, 7.2000e+02, 3.4083e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([4, 6])
xywh: tensor([[ 132.8206,  592.6332,  265.6412,  221.1313],
        [ 135.4799,  553.7633,  269.9026,  139.9409],
        [1238.0952,  397.8211,   83.4287,   74.7744],
        [ 744.9558,  448.3384, 1064.2209,  543.3232]], device='cuda:0')
xywhn: tensor([[0.1038, 0.8231, 0.2075, 0.3071],
        [0.1058, 0.7691, 0.2109, 0.1944],
        [0.9673, 0.5525, 0.0652, 0.1039],
        [0.5820, 0.6227, 0.8314, 0.7546]], device='cuda:0')
xyxy: tensor([[0.0000e+00, 4.8207e+02, 2.6564e+02, 7.0320e+02],
        [5.2856e-01, 4.8379e+02, 2.7043e+02, 6.2373e+02],
        [1.1964e+03, 3.6043e+02, 1.2798e+03, 4.3521e+02],
        [2.1285e+02, 1.7668e+02, 1.2771e+03, 7.2000e+02]], device='cuda:0')
xyxyn: tensor([[0.0000e+00, 6.6954e-01, 2.0753e-01, 9.7667e-01],
        [4.1294e-04, 6.7193e-01, 2.1127e-01, 8.6630e-01],
        [9.3467e-01, 5.0060e-01, 9.9985e-01, 6.0446e-01],
        [1.6629e-01, 2.4538e-01, 9.9771e-01, 1.0000e+00]], device='cuda:0')

0: 384x640 3 Potholes, 12.2ms
Speed: 1.9ms preprocess, 12.2ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0.], device='cuda:0')
conf: tensor([0.8855, 0.4457, 0.3703], device='cuda:0')
data: tensor([[0.0000e+00, 4.9103e+02, 2.5465e+02, 6.4442e+02, 8.8545e-01, 0.0000e+00],
        [1.9469e+02, 1.7771e+02, 1.2784e+03, 7.2000e+02, 4.4568e-01, 0.0000e+00],
        [1.2119e+03, 3.6461e+02, 1.2796e+03, 4.4332e+02, 3.7029e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([3, 6])
xywh: tensor([[ 127.3229,  567.7238,  254.6458,  153.3890],
        [ 736.5232,  448.8549, 1083.6719,  542.2902],
        [1245.7241,  403.9650,   67.6648,   78.7003]], device='cuda:0')
xywhn: tensor([[0.0995, 0.7885, 0.1989, 0.2130],
        [0.5754, 0.6234, 0.8466, 0.7532],
        [0.9732, 0.5611, 0.0529, 0.1093]], device='cuda:0')
xyxy: tensor([[   0.0000,  491.0293,  254.6458,  644.4183],
        [ 194.6873,  177.7098, 1278.3591,  720.0000],
        [1211.8917,  364.6148, 1279.5565,  443.3151]], device='cuda:0')
xyxyn: tensor([[0.0000, 0.6820, 0.1989, 0.8950],
        [0.1521, 0.2468, 0.9987, 1.0000],
        [0.9468, 0.5064, 0.9997, 0.6157]], device='cuda:0')

0: 384x640 3 Potholes, 17.3ms
Speed: 4.9ms preprocess, 17.3ms inference, 7.0ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0.], device='cuda:0')
conf: tensor([0.8695, 0.5282, 0.2799], device='cuda:0')
data: tensor([[4.2805e-01, 5.1168e+02, 2.4123e+02, 6.9530e+02, 8.6951e-01, 0.0000e+00],
        [1.7014e+02, 1.7381e+02, 1.2764e+03, 7.2000e+02, 5.2819e-01, 0.0000e+00],
        [3.7384e+02, 6.0313e+02, 4.8564e+02, 6.7199e+02, 2.7987e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([3, 6])
xywh: tensor([[ 120.8278,  603.4927,  240.7995,  183.6179],
        [ 723.2606,  446.9075, 1106.2361,  546.1851],
        [ 429.7376,  637.5608,  111.8008,   68.8665]], device='cuda:0')
xywhn: tensor([[0.0944, 0.8382, 0.1881, 0.2550],
        [0.5650, 0.6207, 0.8642, 0.7586],
        [0.3357, 0.8855, 0.0873, 0.0956]], device='cuda:0')
xyxy: tensor([[4.2805e-01, 5.1168e+02, 2.4123e+02, 6.9530e+02],
        [1.7014e+02, 1.7381e+02, 1.2764e+03, 7.2000e+02],
        [3.7384e+02, 6.0313e+02, 4.8564e+02, 6.7199e+02]], device='cuda:0')
xyxyn: tensor([[3.3442e-04, 7.1067e-01, 1.8846e-01, 9.6570e-01],
        [1.3292e-01, 2.4141e-01, 9.9717e-01, 1.0000e+00],
        [2.9206e-01, 8.3768e-01, 3.7940e-01, 9.3333e-01]], device='cuda:0')

0: 384x640 3 Potholes, 22.9ms
Speed: 2.0ms preprocess, 22.9ms inference, 2.8ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0.], device='cuda:0')
conf: tensor([0.8670, 0.7051, 0.2832], device='cuda:0')
data: tensor([[2.9007e-01, 5.1984e+02, 2.3407e+02, 7.0637e+02, 8.6700e-01, 0.0000e+00],
        [1.5619e+02, 1.7956e+02, 1.2777e+03, 7.2000e+02, 7.0511e-01, 0.0000e+00],
        [3.6908e+02, 6.1942e+02, 4.8463e+02, 7.1220e+02, 2.8316e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([3, 6])
xywh: tensor([[ 117.1781,  613.1063,  233.7761,  186.5369],
        [ 716.9666,  449.7787, 1121.5443,  540.4426],
        [ 426.8524,  665.8096,  115.5463,   92.7761]], device='cuda:0')
xywhn: tensor([[0.0915, 0.8515, 0.1826, 0.2591],
        [0.5601, 0.6247, 0.8762, 0.7506],
        [0.3335, 0.9247, 0.0903, 0.1289]], device='cuda:0')
xyxy: tensor([[2.9007e-01, 5.1984e+02, 2.3407e+02, 7.0637e+02],
        [1.5619e+02, 1.7956e+02, 1.2777e+03, 7.2000e+02],
        [3.6908e+02, 6.1942e+02, 4.8463e+02, 7.1220e+02]], device='cuda:0')
xyxyn: tensor([[2.2662e-04, 7.2200e-01, 1.8286e-01, 9.8108e-01],
        [1.2203e-01, 2.4939e-01, 9.9823e-01, 1.0000e+00],
        [2.8834e-01, 8.6031e-01, 3.7861e-01, 9.8916e-01]], device='cuda:0')

0: 384x640 3 Potholes, 20.4ms
Speed: 2.0ms preprocess, 20.4ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0.], device='cuda:0')
conf: tensor([0.8957, 0.6641, 0.5367], device='cuda:0')
data: tensor([[1.7105e-01, 5.3059e+02, 2.2449e+02, 7.1825e+02, 8.9572e-01, 0.0000e+00],
        [1.3756e+02, 1.7777e+02, 1.2769e+03, 7.2000e+02, 6.6414e-01, 0.0000e+00],
        [3.5612e+02, 6.2951e+02, 4.8456e+02, 7.1415e+02, 5.3665e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([3, 6])
xywh: tensor([[ 112.3304,  624.4178,  224.3187,  187.6641],
        [ 707.2299,  448.8838, 1139.3495,  542.2324],
        [ 420.3391,  671.8281,  128.4337,   84.6365]], device='cuda:0')
xywhn: tensor([[0.0878, 0.8672, 0.1752, 0.2606],
        [0.5525, 0.6234, 0.8901, 0.7531],
        [0.3284, 0.9331, 0.1003, 0.1176]], device='cuda:0')
xyxy: tensor([[1.7105e-01, 5.3059e+02, 2.2449e+02, 7.1825e+02],
        [1.3756e+02, 1.7777e+02, 1.2769e+03, 7.2000e+02],
        [3.5612e+02, 6.2951e+02, 4.8456e+02, 7.1415e+02]], device='cuda:0')
xyxyn: tensor([[1.3363e-04, 7.3692e-01, 1.7538e-01, 9.9757e-01],
        [1.0746e-01, 2.4690e-01, 9.9758e-01, 1.0000e+00],
        [2.7822e-01, 8.7432e-01, 3.7856e-01, 9.9187e-01]], device='cuda:0')

0: 384x640 3 Potholes, 10.1ms
Speed: 4.2ms preprocess, 10.1ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0.], device='cuda:0')
conf: tensor([0.8740, 0.6254, 0.4887], device='cuda:0')
data: tensor([[0.0000e+00, 5.4238e+02, 2.1582e+02, 7.1772e+02, 8.7396e-01, 0.0000e+00],
        [1.3220e+02, 1.7609e+02, 1.2771e+03, 7.2000e+02, 6.2536e-01, 0.0000e+00],
        [3.5169e+02, 6.4706e+02, 4.8359e+02, 7.1870e+02, 4.8872e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([3, 6])
xywh: tensor([[ 107.9100,  630.0481,  215.8199,  175.3345],
        [ 704.6531,  448.0450, 1144.9053,  543.9099],
        [ 417.6365,  682.8800,  131.9027,   71.6475]], device='cuda:0')
xywhn: tensor([[0.0843, 0.8751, 0.1686, 0.2435],
        [0.5505, 0.6223, 0.8945, 0.7554],
        [0.3263, 0.9484, 0.1030, 0.0995]], device='cuda:0')
xyxy: tensor([[   0.0000,  542.3809,  215.8199,  717.7153],
        [ 132.2004,  176.0901, 1277.1057,  720.0000],
        [ 351.6852,  647.0563,  483.5879,  718.7037]], device='cuda:0')
xyxyn: tensor([[0.0000, 0.7533, 0.1686, 0.9968],
        [0.1033, 0.2446, 0.9977, 1.0000],
        [0.2748, 0.8987, 0.3778, 0.9982]], device='cuda:0')

0: 384x640 2 Potholes, 14.5ms
Speed: 1.9ms preprocess, 14.5ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0.], device='cuda:0')
conf: tensor([0.8605, 0.6635], device='cuda:0')
data: tensor([[0.0000e+00, 5.6497e+02, 1.9614e+02, 7.2000e+02, 8.6051e-01, 0.0000e+00],
        [1.0080e+02, 1.7460e+02, 1.2765e+03, 7.2000e+02, 6.6351e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([2, 6])
xywh: tensor([[  98.0681,  642.4832,  196.1362,  155.0336],
        [ 688.6371,  447.3001, 1175.6741,  545.3998]], device='cuda:0')
xywhn: tensor([[0.0766, 0.8923, 0.1532, 0.2153],
        [0.5380, 0.6213, 0.9185, 0.7575]], device='cuda:0')
xyxy: tensor([[   0.0000,  564.9664,  196.1362,  720.0000],
        [ 100.8000,  174.6002, 1276.4741,  720.0000]], device='cuda:0')
xyxyn: tensor([[0.0000, 0.7847, 0.1532, 1.0000],
        [0.0788, 0.2425, 0.9972, 1.0000]], device='cuda:0')

0: 384x640 2 Potholes, 10.0ms
Speed: 3.9ms preprocess, 10.0ms inference, 5.9ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0.], device='cuda:0')
conf: tensor([0.8628, 0.4249], device='cuda:0')
data: tensor([[1.3423e-01, 5.7592e+02, 1.8138e+02, 7.2000e+02, 8.6282e-01, 0.0000e+00],
        [7.6755e+01, 1.7381e+02, 1.2765e+03, 7.2000e+02, 4.2494e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([2, 6])
xywh: tensor([[  90.7579,  647.9592,  181.2474,  144.0815],
        [ 676.6494,  446.9039, 1199.7896,  546.1923]], device='cuda:0')
xywhn: tensor([[0.0709, 0.8999, 0.1416, 0.2001],
        [0.5286, 0.6207, 0.9373, 0.7586]], device='cuda:0')
xyxy: tensor([[1.3423e-01, 5.7592e+02, 1.8138e+02, 7.2000e+02],
        [7.6755e+01, 1.7381e+02, 1.2765e+03, 7.2000e+02]], device='cuda:0')
xyxyn: tensor([[1.0487e-04, 7.9989e-01, 1.4170e-01, 1.0000e+00],
        [5.9965e-02, 2.4140e-01, 9.9730e-01, 1.0000e+00]], device='cuda:0')

0: 384x640 2 Potholes, 12.6ms
Speed: 2.0ms preprocess, 12.6ms inference, 1.9ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0.], device='cuda:0')
conf: tensor([0.8419, 0.5091], device='cuda:0')
data: tensor([[2.8702e-01, 5.8988e+02, 1.7417e+02, 7.2000e+02, 8.4186e-01, 0.0000e+00],
        [6.3478e+01, 1.7885e+02, 1.2794e+03, 7.2000e+02, 5.0907e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([2, 6])
xywh: tensor([[  87.2309,  654.9424,  173.8878,  130.1151],
        [ 671.4142,  449.4240, 1215.8717,  541.1520]], device='cuda:0')
xywhn: tensor([[0.0681, 0.9096, 0.1358, 0.1807],
        [0.5245, 0.6242, 0.9499, 0.7516]], device='cuda:0')
xyxy: tensor([[2.8702e-01, 5.8988e+02, 1.7417e+02, 7.2000e+02],
        [6.3478e+01, 1.7885e+02, 1.2794e+03, 7.2000e+02]], device='cuda:0')
xyxyn: tensor([[2.2423e-04, 8.1928e-01, 1.3607e-01, 1.0000e+00],
        [4.9592e-02, 2.4840e-01, 9.9949e-01, 1.0000e+00]], device='cuda:0')

0: 384x640 2 Potholes, 13.0ms
Speed: 2.3ms preprocess, 13.0ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0.], device='cuda:0')
conf: tensor([0.7950, 0.4302], device='cuda:0')
data: tensor([[8.0385e-01, 6.2115e+02, 1.5558e+02, 7.2000e+02, 7.9503e-01, 0.0000e+00],
        [4.2709e+01, 1.8261e+02, 1.2783e+03, 7.2000e+02, 4.3016e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([2, 6])
xywh: tensor([[  78.1905,  670.5771,  154.7733,   98.8458],
        [ 660.5283,  451.3032, 1235.6387,  537.3937]], device='cuda:0')
xywhn: tensor([[0.0611, 0.9314, 0.1209, 0.1373],
        [0.5160, 0.6268, 0.9653, 0.7464]], device='cuda:0')
xyxy: tensor([[8.0385e-01, 6.2115e+02, 1.5558e+02, 7.2000e+02],
        [4.2709e+01, 1.8261e+02, 1.2783e+03, 7.2000e+02]], device='cuda:0')
xyxyn: tensor([[6.2801e-04, 8.6271e-01, 1.2154e-01, 1.0000e+00],
        [3.3366e-02, 2.5362e-01, 9.9871e-01, 1.0000e+00]], device='cuda:0')

0: 384x640 2 Potholes, 14.4ms
Speed: 2.1ms preprocess, 14.4ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0.], device='cuda:0')
conf: tensor([0.6499, 0.3421], device='cuda:0')
data: tensor([[2.9272e-01, 6.3154e+02, 1.4087e+02, 7.2000e+02, 6.4993e-01, 0.0000e+00],
        [2.6305e+01, 1.7764e+02, 1.2790e+03, 7.2000e+02, 3.4212e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([2, 6])
xywh: tensor([[  70.5820,  675.7722,  140.5786,   88.4556],
        [ 652.6565,  448.8200, 1252.7036,  542.3600]], device='cuda:0')
xywhn: tensor([[0.0551, 0.9386, 0.1098, 0.1229],
        [0.5099, 0.6234, 0.9787, 0.7533]], device='cuda:0')
xyxy: tensor([[2.9272e-01, 6.3154e+02, 1.4087e+02, 7.2000e+02],
        [2.6305e+01, 1.7764e+02, 1.2790e+03, 7.2000e+02]], device='cuda:0')
xyxyn: tensor([[2.2869e-04, 8.7714e-01, 1.1006e-01, 1.0000e+00],
        [2.0551e-02, 2.4672e-01, 9.9923e-01, 1.0000e+00]], device='cuda:0')

0: 384x640 2 Potholes, 10.7ms
Speed: 2.0ms preprocess, 10.7ms inference, 3.5ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0.], device='cuda:0')
conf: tensor([0.5786, 0.5410], device='cuda:0')
data: tensor([[0.0000e+00, 6.5880e+02, 1.0222e+02, 7.2000e+02, 5.7862e-01, 0.0000e+00],
        [0.0000e+00, 1.8416e+02, 1.2800e+03, 7.2000e+02, 5.4101e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([2, 6])
xywh: tensor([[  51.1103,  689.3996,  102.2206,   61.2008],
        [ 640.0000,  452.0798, 1280.0000,  535.8404]], device='cuda:0')
xywhn: tensor([[0.0399, 0.9575, 0.0799, 0.0850],
        [0.5000, 0.6279, 1.0000, 0.7442]], device='cuda:0')
xyxy: tensor([[   0.0000,  658.7992,  102.2206,  720.0000],
        [   0.0000,  184.1596, 1280.0000,  720.0000]], device='cuda:0')
xyxyn: tensor([[0.0000, 0.9150, 0.0799, 1.0000],
        [0.0000, 0.2558, 1.0000, 1.0000]], device='cuda:0')

0: 384x640 3 Potholes, 13.0ms
Speed: 2.1ms preprocess, 13.0ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0.], device='cuda:0')
conf: tensor([0.5385, 0.3662, 0.3356], device='cuda:0')
data: tensor([[0.0000e+00, 1.8518e+02, 1.2800e+03, 7.2000e+02, 5.3848e-01, 0.0000e+00],
        [6.3353e+02, 3.6140e+02, 7.0916e+02, 4.0160e+02, 3.6622e-01, 0.0000e+00],
        [7.2801e+02, 3.1443e+02, 8.4804e+02, 3.5130e+02, 3.3555e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([3, 6])
xywh: tensor([[ 640.0000,  452.5909, 1280.0000,  534.8183],
        [ 671.3433,  381.4973,   75.6240,   40.1954],
        [ 788.0266,  332.8635,  120.0312,   36.8693]], device='cuda:0')
xywhn: tensor([[0.5000, 0.6286, 1.0000, 0.7428],
        [0.5245, 0.5299, 0.0591, 0.0558],
        [0.6156, 0.4623, 0.0938, 0.0512]], device='cuda:0')
xyxy: tensor([[   0.0000,  185.1817, 1280.0000,  720.0000],
        [ 633.5312,  361.3996,  709.1553,  401.5950],
        [ 728.0109,  314.4288,  848.0422,  351.2981]], device='cuda:0')
xyxyn: tensor([[0.0000, 0.2572, 1.0000, 1.0000],
        [0.4949, 0.5019, 0.5540, 0.5578],
        [0.5688, 0.4367, 0.6625, 0.4879]], device='cuda:0')

0: 384x640 2 Potholes, 10.6ms
Speed: 1.9ms preprocess, 10.6ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0.], device='cuda:0')
conf: tensor([0.4234, 0.2900], device='cuda:0')
data: tensor([[0.0000e+00, 1.8449e+02, 1.2800e+03, 7.2000e+02, 4.2345e-01, 0.0000e+00],
        [6.3619e+02, 3.6519e+02, 7.0405e+02, 4.0207e+02, 2.9000e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([2, 6])
xywh: tensor([[ 640.0000,  452.2467, 1280.0000,  535.5066],
        [ 670.1177,  383.6318,   67.8547,   36.8823]], device='cuda:0')
xywhn: tensor([[0.5000, 0.6281, 1.0000, 0.7438],
        [0.5235, 0.5328, 0.0530, 0.0512]], device='cuda:0')
xyxy: tensor([[   0.0000,  184.4934, 1280.0000,  720.0000],
        [ 636.1904,  365.1907,  704.0451,  402.0730]], device='cuda:0')
xyxyn: tensor([[0.0000, 0.2562, 1.0000, 1.0000],
        [0.4970, 0.5072, 0.5500, 0.5584]], device='cuda:0')

0: 384x640 1 Pothole, 11.0ms
Speed: 2.0ms preprocess, 11.0ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0.], device='cuda:0')
conf: tensor([0.3687], device='cuda:0')
data: tensor([[0.0000e+00, 1.8494e+02, 1.2799e+03, 7.2000e+02, 3.6872e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([1, 6])
xywh: tensor([[ 639.9408,  452.4720, 1279.8816,  535.0560]], device='cuda:0')
xywhn: tensor([[0.5000, 0.6284, 0.9999, 0.7431]], device='cuda:0')
xyxy: tensor([[   0.0000,  184.9440, 1279.8816,  720.0000]], device='cuda:0')
xyxyn: tensor([[0.0000, 0.2569, 0.9999, 1.0000]], device='cuda:0')

0: 384x640 1 Pothole, 10.3ms
Speed: 2.0ms preprocess, 10.3ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0.], device='cuda:0')
conf: tensor([0.2646], device='cuda:0')
data: tensor([[5.8154e-01, 1.8727e+02, 1.2800e+03, 7.2000e+02, 2.6457e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([1, 6])
xywh: tensor([[ 640.2908,  453.6342, 1279.4185,  532.7316]], device='cuda:0')
xywhn: tensor([[0.5002, 0.6300, 0.9995, 0.7399]], device='cuda:0')
xyxy: tensor([[5.8154e-01, 1.8727e+02, 1.2800e+03, 7.2000e+02]], device='cuda:0')
xyxyn: tensor([[4.5433e-04, 2.6010e-01, 1.0000e+00, 1.0000e+00]], device='cuda:0')

0: 384x640 5 Potholes, 10.1ms
Speed: 2.0ms preprocess, 10.1ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.3479, 0.3244, 0.3013, 0.2767, 0.2630], device='cuda:0')
data: tensor([[8.8495e+02, 5.2492e+02, 9.8913e+02, 6.0293e+02, 3.4789e-01, 0.0000e+00],
        [7.5650e+01, 4.1640e+02, 2.4606e+02, 4.8140e+02, 3.2439e-01, 0.0000e+00],
        [6.4284e+02, 3.8287e+02, 7.2806e+02, 4.2820e+02, 3.0129e-01, 0.0000e+00],
        [7.3936e+02, 3.2647e+02, 8.7554e+02, 3.6774e+02, 2.7670e-01, 0.0000e+00],
        [4.0063e-01, 1.8922e+02, 1.2762e+03, 7.2000e+02, 2.6304e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([5, 6])
xywh: tensor([[ 937.0400,  563.9203,  104.1775,   78.0103],
        [ 160.8537,  448.9018,  170.4073,   65.0002],
        [ 685.4498,  405.5393,   85.2190,   45.3292],
        [ 807.4515,  347.1021,  136.1804,   41.2717],
        [ 638.2941,  454.6082, 1275.7869,  530.7835]], device='cuda:0')
xywhn: tensor([[0.7321, 0.7832, 0.0814, 0.1083],
        [0.1257, 0.6235, 0.1331, 0.0903],
        [0.5355, 0.5632, 0.0666, 0.0630],
        [0.6308, 0.4821, 0.1064, 0.0573],
        [0.4987, 0.6314, 0.9967, 0.7372]], device='cuda:0')
xyxy: tensor([[8.8495e+02, 5.2492e+02, 9.8913e+02, 6.0293e+02],
        [7.5650e+01, 4.1640e+02, 2.4606e+02, 4.8140e+02],
        [6.4284e+02, 3.8287e+02, 7.2806e+02, 4.2820e+02],
        [7.3936e+02, 3.2647e+02, 8.7554e+02, 3.6774e+02],
        [4.0063e-01, 1.8922e+02, 1.2762e+03, 7.2000e+02]], device='cuda:0')
xyxyn: tensor([[6.9137e-01, 7.2905e-01, 7.7276e-01, 8.3740e-01],
        [5.9102e-02, 5.7834e-01, 1.9223e-01, 6.6861e-01],
        [5.0222e-01, 5.3177e-01, 5.6880e-01, 5.9473e-01],
        [5.7763e-01, 4.5343e-01, 6.8402e-01, 5.1075e-01],
        [3.1300e-04, 2.6280e-01, 9.9702e-01, 1.0000e+00]], device='cuda:0')

0: 384x640 3 Potholes, 11.7ms
Speed: 2.2ms preprocess, 11.7ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0.], device='cuda:0')
conf: tensor([0.5633, 0.3212, 0.3106], device='cuda:0')
data: tensor([[6.4500e+02, 3.8757e+02, 7.3423e+02, 4.3661e+02, 5.6335e-01, 0.0000e+00],
        [7.4411e+02, 3.3294e+02, 8.7803e+02, 3.7360e+02, 3.2119e-01, 0.0000e+00],
        [8.9709e+02, 5.3777e+02, 9.9625e+02, 6.1748e+02, 3.1060e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([3, 6])
xywh: tensor([[689.6140, 412.0901,  89.2339,  49.0447],
        [811.0704, 353.2723, 133.9185,  40.6650],
        [946.6735, 577.6256,  99.1628,  79.7053]], device='cuda:0')
xywhn: tensor([[0.5388, 0.5723, 0.0697, 0.0681],
        [0.6336, 0.4907, 0.1046, 0.0565],
        [0.7396, 0.8023, 0.0775, 0.1107]], device='cuda:0')
xyxy: tensor([[644.9971, 387.5678, 734.2310, 436.6125],
        [744.1111, 332.9398, 878.0296, 373.6048],
        [897.0920, 537.7729, 996.2549, 617.4783]], device='cuda:0')
xyxyn: tensor([[0.5039, 0.5383, 0.5736, 0.6064],
        [0.5813, 0.4624, 0.6860, 0.5189],
        [0.7009, 0.7469, 0.7783, 0.8576]], device='cuda:0')

0: 384x640 2 Potholes, 11.2ms
Speed: 2.0ms preprocess, 11.2ms inference, 1.9ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0.], device='cuda:0')
conf: tensor([0.5162, 0.3130], device='cuda:0')
data: tensor([[6.4423e+02, 3.9575e+02, 7.3685e+02, 4.4897e+02, 5.1623e-01, 0.0000e+00],
        [7.4616e+02, 3.3578e+02, 8.8636e+02, 3.7752e+02, 3.1301e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([2, 6])
xywh: tensor([[690.5401, 422.3594,  92.6205,  53.2220],
        [816.2631, 356.6501, 140.1965,  41.7456]], device='cuda:0')
xywhn: tensor([[0.5395, 0.5866, 0.0724, 0.0739],
        [0.6377, 0.4953, 0.1095, 0.0580]], device='cuda:0')
xyxy: tensor([[644.2299, 395.7484, 736.8503, 448.9705],
        [746.1648, 335.7773, 886.3613, 377.5229]], device='cuda:0')
xyxyn: tensor([[0.5033, 0.5497, 0.5757, 0.6236],
        [0.5829, 0.4664, 0.6925, 0.5243]], device='cuda:0')

0: 384x640 5 Potholes, 11.9ms
Speed: 2.0ms preprocess, 11.9ms inference, 1.9ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.6269, 0.5863, 0.4652, 0.3984, 0.2932], device='cuda:0')
data: tensor([[7.5593e+02, 3.4357e+02, 8.9914e+02, 3.8838e+02, 6.2693e-01, 0.0000e+00],
        [6.5310e+02, 4.0623e+02, 7.5425e+02, 4.6213e+02, 5.8630e-01, 0.0000e+00],
        [6.7817e+02, 5.5787e+02, 1.0676e+03, 7.2000e+02, 4.6525e-01, 0.0000e+00],
        [6.5193e+02, 4.0829e+02, 7.4171e+02, 4.5191e+02, 3.9843e-01, 0.0000e+00],
        [7.4931e+02, 1.8981e+02, 9.7654e+02, 2.2849e+02, 2.9324e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([5, 6])
xywh: tensor([[827.5353, 365.9757, 143.2180,  44.8120],
        [703.6796, 434.1822, 101.1499,  55.8948],
        [872.8653, 638.9353, 389.3988, 162.1294],
        [696.8204, 430.1026,  89.7734,  43.6154],
        [862.9226, 209.1499, 227.2292,  38.6840]], device='cuda:0')
xywhn: tensor([[0.6465, 0.5083, 0.1119, 0.0622],
        [0.5497, 0.6030, 0.0790, 0.0776],
        [0.6819, 0.8874, 0.3042, 0.2252],
        [0.5444, 0.5974, 0.0701, 0.0606],
        [0.6742, 0.2905, 0.1775, 0.0537]], device='cuda:0')
xyxy: tensor([[ 755.9263,  343.5697,  899.1443,  388.3817],
        [ 653.1046,  406.2348,  754.2545,  462.1296],
        [ 678.1659,  557.8706, 1067.5647,  720.0000],
        [ 651.9337,  408.2949,  741.7072,  451.9103],
        [ 749.3080,  189.8079,  976.5372,  228.4919]], device='cuda:0')
xyxyn: tensor([[0.5906, 0.4772, 0.7025, 0.5394],
        [0.5102, 0.5642, 0.5893, 0.6418],
        [0.5298, 0.7748, 0.8340, 1.0000],
        [0.5093, 0.5671, 0.5795, 0.6277],
        [0.5854, 0.2636, 0.7629, 0.3173]], device='cuda:0')

0: 384x640 4 Potholes, 11.6ms
Speed: 2.2ms preprocess, 11.6ms inference, 1.9ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.6647, 0.6070, 0.5577, 0.4496], device='cuda:0')
data: tensor([[6.5278e+02, 4.1173e+02, 7.6331e+02, 4.6526e+02, 6.6469e-01, 0.0000e+00],
        [7.5863e+02, 3.4836e+02, 8.9261e+02, 3.9065e+02, 6.0697e-01, 0.0000e+00],
        [6.5277e+02, 4.1327e+02, 7.4339e+02, 4.5503e+02, 5.5768e-01, 0.0000e+00],
        [6.7997e+02, 5.7376e+02, 1.1047e+03, 7.2000e+02, 4.4962e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([4, 6])
xywh: tensor([[708.0419, 438.4938, 110.5288,  53.5245],
        [825.6205, 369.5049, 133.9786,  42.2888],
        [698.0781, 434.1490,  90.6150,  41.7571],
        [892.3347, 646.8801, 424.7235, 146.2399]], device='cuda:0')
xywhn: tensor([[0.5532, 0.6090, 0.0864, 0.0743],
        [0.6450, 0.5132, 0.1047, 0.0587],
        [0.5454, 0.6030, 0.0708, 0.0580],
        [0.6971, 0.8984, 0.3318, 0.2031]], device='cuda:0')
xyxy: tensor([[ 652.7775,  411.7315,  763.3063,  465.2560],
        [ 758.6312,  348.3605,  892.6099,  390.6493],
        [ 652.7706,  413.2705,  743.3856,  455.0276],
        [ 679.9729,  573.7601, 1104.6964,  720.0000]], device='cuda:0')
xyxyn: tensor([[0.5100, 0.5718, 0.5963, 0.6462],
        [0.5927, 0.4838, 0.6974, 0.5426],
        [0.5100, 0.5740, 0.5808, 0.6320],
        [0.5312, 0.7969, 0.8630, 1.0000]], device='cuda:0')

0: 384x640 5 Potholes, 12.3ms
Speed: 2.2ms preprocess, 12.3ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.6622, 0.5368, 0.3536, 0.2959, 0.2812], device='cuda:0')
data: tensor([[6.5565e+02, 4.1924e+02, 7.6469e+02, 4.7058e+02, 6.6219e-01, 0.0000e+00],
        [7.6050e+02, 3.5282e+02, 9.0564e+02, 3.9578e+02, 5.3678e-01, 0.0000e+00],
        [7.5169e+02, 1.9217e+02, 9.7616e+02, 2.3106e+02, 3.5360e-01, 0.0000e+00],
        [6.6446e+02, 5.9068e+02, 1.1159e+03, 7.2000e+02, 2.9586e-01, 0.0000e+00],
        [6.5531e+02, 4.1706e+02, 7.5483e+02, 4.6005e+02, 2.8124e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([5, 6])
xywh: tensor([[710.1721, 444.9140, 109.0400,  51.3402],
        [833.0701, 374.2960, 145.1420,  42.9619],
        [863.9232, 211.6143, 224.4695,  38.8883],
        [890.1953, 655.3405, 451.4641, 129.3191],
        [705.0692, 438.5551,  99.5168,  42.9969]], device='cuda:0')
xywhn: tensor([[0.5548, 0.6179, 0.0852, 0.0713],
        [0.6508, 0.5199, 0.1134, 0.0597],
        [0.6749, 0.2939, 0.1754, 0.0540],
        [0.6955, 0.9102, 0.3527, 0.1796],
        [0.5508, 0.6091, 0.0777, 0.0597]], device='cuda:0')
xyxy: tensor([[ 655.6521,  419.2439,  764.6921,  470.5841],
        [ 760.4991,  352.8150,  905.6411,  395.7769],
        [ 751.6884,  192.1702,  976.1579,  231.0585],
        [ 664.4633,  590.6809, 1115.9274,  720.0000],
        [ 655.3108,  417.0567,  754.8276,  460.0536]], device='cuda:0')
xyxyn: tensor([[0.5122, 0.5823, 0.5974, 0.6536],
        [0.5941, 0.4900, 0.7075, 0.5497],
        [0.5873, 0.2669, 0.7626, 0.3209],
        [0.5191, 0.8204, 0.8718, 1.0000],
        [0.5120, 0.5792, 0.5897, 0.6390]], device='cuda:0')

0: 384x640 5 Potholes, 12.1ms
Speed: 2.0ms preprocess, 12.1ms inference, 1.8ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.5191, 0.4785, 0.4094, 0.3273, 0.2697], device='cuda:0')
data: tensor([[6.6232e+02, 4.3033e+02, 7.5454e+02, 4.7974e+02, 5.1911e-01, 0.0000e+00],
        [7.7583e+02, 3.6082e+02, 9.2105e+02, 4.0696e+02, 4.7846e-01, 0.0000e+00],
        [6.1493e-01, 4.8124e+02, 2.0263e+02, 5.8672e+02, 4.0943e-01, 0.0000e+00],
        [7.5774e+02, 1.9498e+02, 9.8830e+02, 2.3481e+02, 3.2731e-01, 0.0000e+00],
        [9.8114e+02, 6.3138e+02, 1.1322e+03, 7.1885e+02, 2.6969e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([5, 6])
xywh: tensor([[ 708.4260,  455.0334,   92.2188,   49.4116],
        [ 848.4418,  383.8929,  145.2205,   46.1358],
        [ 101.6221,  533.9782,  202.0144,  105.4808],
        [ 873.0156,  214.8930,  230.5588,   39.8356],
        [1056.6962,  675.1133,  151.1030,   87.4756]], device='cuda:0')
xywhn: tensor([[0.5535, 0.6320, 0.0720, 0.0686],
        [0.6628, 0.5332, 0.1135, 0.0641],
        [0.0794, 0.7416, 0.1578, 0.1465],
        [0.6820, 0.2985, 0.1801, 0.0553],
        [0.8255, 0.9377, 0.1180, 0.1215]], device='cuda:0')
xyxy: tensor([[6.6232e+02, 4.3033e+02, 7.5454e+02, 4.7974e+02],
        [7.7583e+02, 3.6082e+02, 9.2105e+02, 4.0696e+02],
        [6.1493e-01, 4.8124e+02, 2.0263e+02, 5.8672e+02],
        [7.5774e+02, 1.9498e+02, 9.8830e+02, 2.3481e+02],
        [9.8114e+02, 6.3138e+02, 1.1322e+03, 7.1885e+02]], device='cuda:0')
xyxyn: tensor([[5.1743e-01, 5.9768e-01, 5.8948e-01, 6.6630e-01],
        [6.0612e-01, 5.0115e-01, 7.1957e-01, 5.6522e-01],
        [4.8041e-04, 6.6839e-01, 1.5830e-01, 8.1489e-01],
        [5.9198e-01, 2.7080e-01, 7.7211e-01, 3.2613e-01],
        [7.6652e-01, 8.7691e-01, 8.8457e-01, 9.9840e-01]], device='cuda:0')

0: 384x640 5 Potholes, 16.4ms
Speed: 2.0ms preprocess, 16.4ms inference, 2.5ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.4799, 0.4789, 0.4189, 0.3011, 0.2837], device='cuda:0')
data: tensor([[6.6647e+02, 4.3894e+02, 7.6883e+02, 4.9759e+02, 4.7986e-01, 0.0000e+00],
        [7.7757e+02, 3.6361e+02, 9.3071e+02, 4.1231e+02, 4.7890e-01, 0.0000e+00],
        [7.5829e+02, 1.9627e+02, 9.9973e+02, 2.3372e+02, 4.1894e-01, 0.0000e+00],
        [1.0010e+03, 6.4750e+02, 1.1204e+03, 7.2000e+02, 3.0110e-01, 0.0000e+00],
        [6.6604e+02, 4.3940e+02, 7.8035e+02, 5.1717e+02, 2.8375e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([5, 6])
xywh: tensor([[ 717.6478,  468.2625,  102.3597,   58.6487],
        [ 854.1371,  387.9582,  153.1395,   48.6938],
        [ 879.0109,  214.9969,  241.4368,   37.4474],
        [1060.6699,  683.7502,  119.3994,   72.4996],
        [ 723.1965,  478.2845,  114.3054,   77.7683]], device='cuda:0')
xywhn: tensor([[0.5607, 0.6504, 0.0800, 0.0815],
        [0.6673, 0.5388, 0.1196, 0.0676],
        [0.6867, 0.2986, 0.1886, 0.0520],
        [0.8286, 0.9497, 0.0933, 0.1007],
        [0.5650, 0.6643, 0.0893, 0.1080]], device='cuda:0')
xyxy: tensor([[ 666.4680,  438.9382,  768.8277,  497.5869],
        [ 777.5674,  363.6113,  930.7069,  412.3051],
        [ 758.2925,  196.2732,  999.7292,  233.7206],
        [1000.9703,  647.5004, 1120.3696,  720.0000],
        [ 666.0438,  439.4003,  780.3492,  517.1686]], device='cuda:0')
xyxyn: tensor([[0.5207, 0.6096, 0.6006, 0.6911],
        [0.6075, 0.5050, 0.7271, 0.5726],
        [0.5924, 0.2726, 0.7810, 0.3246],
        [0.7820, 0.8993, 0.8753, 1.0000],
        [0.5203, 0.6103, 0.6096, 0.7183]], device='cuda:0')

0: 384x640 3 Potholes, 10.2ms
Speed: 2.0ms preprocess, 10.2ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0.], device='cuda:0')
conf: tensor([0.6217, 0.5159, 0.3100], device='cuda:0')
data: tensor([[6.7011e+02, 4.4775e+02, 7.6836e+02, 5.1148e+02, 6.2167e-01, 0.0000e+00],
        [7.8343e+02, 3.6656e+02, 9.3970e+02, 4.1829e+02, 5.1589e-01, 0.0000e+00],
        [7.6273e+02, 1.9631e+02, 1.0023e+03, 2.3551e+02, 3.0998e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([3, 6])
xywh: tensor([[719.2352, 479.6135,  98.2473,  63.7365],
        [861.5670, 392.4222, 156.2720,  51.7316],
        [882.5095, 215.9115, 239.5508,  39.1970]], device='cuda:0')
xywhn: tensor([[0.5619, 0.6661, 0.0768, 0.0885],
        [0.6731, 0.5450, 0.1221, 0.0718],
        [0.6895, 0.2999, 0.1871, 0.0544]], device='cuda:0')
xyxy: tensor([[ 670.1116,  447.7452,  768.3589,  511.4817],
        [ 783.4310,  366.5564,  939.7029,  418.2880],
        [ 762.7341,  196.3130, 1002.2849,  235.5100]], device='cuda:0')
xyxyn: tensor([[0.5235, 0.6219, 0.6003, 0.7104],
        [0.6121, 0.5091, 0.7341, 0.5810],
        [0.5959, 0.2727, 0.7830, 0.3271]], device='cuda:0')

0: 384x640 3 Potholes, 17.1ms
Speed: 2.7ms preprocess, 17.1ms inference, 3.0ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0.], device='cuda:0')
conf: tensor([0.6127, 0.5482, 0.3485], device='cuda:0')
data: tensor([[6.7339e+02, 4.5342e+02, 7.7066e+02, 5.0718e+02, 6.1273e-01, 0.0000e+00],
        [7.8742e+02, 3.7096e+02, 9.3748e+02, 4.2426e+02, 5.4816e-01, 0.0000e+00],
        [6.6987e+02, 4.5360e+02, 7.9484e+02, 5.2035e+02, 3.4851e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([3, 6])
xywh: tensor([[722.0210, 480.2979,  97.2712,  53.7557],
        [862.4503, 397.6090, 150.0648,  53.3036],
        [732.3590, 486.9766, 124.9697,  66.7526]], device='cuda:0')
xywhn: tensor([[0.5641, 0.6671, 0.0760, 0.0747],
        [0.6738, 0.5522, 0.1172, 0.0740],
        [0.5722, 0.6764, 0.0976, 0.0927]], device='cuda:0')
xyxy: tensor([[673.3854, 453.4200, 770.6566, 507.1758],
        [787.4178, 370.9572, 937.4827, 424.2609],
        [669.8741, 453.6003, 794.8439, 520.3529]], device='cuda:0')
xyxyn: tensor([[0.5261, 0.6298, 0.6021, 0.7044],
        [0.6152, 0.5152, 0.7324, 0.5893],
        [0.5233, 0.6300, 0.6210, 0.7227]], device='cuda:0')

0: 384x640 4 Potholes, 10.1ms
Speed: 3.7ms preprocess, 10.1ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.7277, 0.5369, 0.3035, 0.2887], device='cuda:0')
data: tensor([[6.7557e+02, 4.6820e+02, 8.2348e+02, 5.3551e+02, 7.2774e-01, 0.0000e+00],
        [8.0255e+02, 3.8289e+02, 9.6500e+02, 4.3639e+02, 5.3685e-01, 0.0000e+00],
        [7.6550e+02, 1.9825e+02, 1.0090e+03, 2.3513e+02, 3.0353e-01, 0.0000e+00],
        [3.3993e+02, 4.0091e+02, 5.6303e+02, 4.7539e+02, 2.8869e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([4, 6])
xywh: tensor([[749.5247, 501.8572, 147.9033,  67.3051],
        [883.7745, 409.6423, 162.4561,  53.4956],
        [887.2491, 216.6918, 243.4993,  36.8766],
        [451.4826, 438.1538, 223.1046,  74.4786]], device='cuda:0')
xywhn: tensor([[0.5856, 0.6970, 0.1155, 0.0935],
        [0.6904, 0.5689, 0.1269, 0.0743],
        [0.6932, 0.3010, 0.1902, 0.0512],
        [0.3527, 0.6085, 0.1743, 0.1034]], device='cuda:0')
xyxy: tensor([[ 675.5730,  468.2047,  823.4763,  535.5098],
        [ 802.5465,  382.8945,  965.0026,  436.3901],
        [ 765.4995,  198.2535, 1008.9988,  235.1301],
        [ 339.9303,  400.9145,  563.0349,  475.3931]], device='cuda:0')
xyxyn: tensor([[0.5278, 0.6503, 0.6433, 0.7438],
        [0.6270, 0.5318, 0.7539, 0.6061],
        [0.5980, 0.2754, 0.7883, 0.3266],
        [0.2656, 0.5568, 0.4399, 0.6603]], device='cuda:0')

0: 384x640 5 Potholes, 11.7ms
Speed: 2.0ms preprocess, 11.7ms inference, 2.1ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.5827, 0.5245, 0.4582, 0.3272, 0.2720], device='cuda:0')
data: tensor([[6.8163e+02, 4.7839e+02, 8.0207e+02, 5.3662e+02, 5.8270e-01, 0.0000e+00],
        [8.0368e+02, 3.8606e+02, 9.6709e+02, 4.4284e+02, 5.2453e-01, 0.0000e+00],
        [7.6696e+02, 1.9872e+02, 1.0080e+03, 2.3594e+02, 4.5820e-01, 0.0000e+00],
        [6.8219e+02, 4.8002e+02, 8.0136e+02, 5.6744e+02, 3.2715e-01, 0.0000e+00],
        [7.1231e+02, 5.7728e+02, 8.1843e+02, 6.2979e+02, 2.7199e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([5, 6])
xywh: tensor([[741.8534, 507.5053, 120.4374,  58.2311],
        [885.3859, 414.4493, 163.4105,  56.7753],
        [887.4863, 217.3332, 241.0620,  37.2189],
        [741.7778, 523.7282, 119.1732,  87.4200],
        [765.3711, 603.5355, 106.1125,  52.5134]], device='cuda:0')
xywhn: tensor([[0.5796, 0.7049, 0.0941, 0.0809],
        [0.6917, 0.5756, 0.1277, 0.0789],
        [0.6933, 0.3019, 0.1883, 0.0517],
        [0.5795, 0.7274, 0.0931, 0.1214],
        [0.5979, 0.8382, 0.0829, 0.0729]], device='cuda:0')
xyxy: tensor([[ 681.6347,  478.3898,  802.0721,  536.6208],
        [ 803.6807,  386.0617,  967.0912,  442.8369],
        [ 766.9553,  198.7237, 1008.0173,  235.9426],
        [ 682.1912,  480.0182,  801.3644,  567.4382],
        [ 712.3148,  577.2788,  818.4274,  629.7922]], device='cuda:0')
xyxyn: tensor([[0.5325, 0.6644, 0.6266, 0.7453],
        [0.6279, 0.5362, 0.7555, 0.6151],
        [0.5992, 0.2760, 0.7875, 0.3277],
        [0.5330, 0.6667, 0.6261, 0.7881],
        [0.5565, 0.8018, 0.6394, 0.8747]], device='cuda:0')

0: 384x640 4 Potholes, 9.5ms
Speed: 2.1ms preprocess, 9.5ms inference, 1.9ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.6214, 0.5378, 0.4525, 0.4157], device='cuda:0')
data: tensor([[8.1470e+02, 3.9101e+02, 9.7932e+02, 4.4966e+02, 6.2139e-01, 0.0000e+00],
        [7.7021e+02, 1.9852e+02, 1.0046e+03, 2.3629e+02, 5.3782e-01, 0.0000e+00],
        [6.8412e+02, 4.8556e+02, 7.9729e+02, 5.3799e+02, 4.5254e-01, 0.0000e+00],
        [7.2016e+02, 5.9091e+02, 8.2963e+02, 6.4888e+02, 4.1568e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([4, 6])
xywh: tensor([[897.0099, 420.3305, 164.6129,  58.6497],
        [887.4020, 217.4044, 234.3899,  37.7682],
        [740.7068, 511.7764, 113.1683,  52.4373],
        [774.8932, 619.8973, 109.4644,  57.9733]], device='cuda:0')
xywhn: tensor([[0.7008, 0.5838, 0.1286, 0.0815],
        [0.6933, 0.3020, 0.1831, 0.0525],
        [0.5787, 0.7108, 0.0884, 0.0728],
        [0.6054, 0.8610, 0.0855, 0.0805]], device='cuda:0')
xyxy: tensor([[ 814.7035,  391.0057,  979.3164,  449.6554],
        [ 770.2071,  198.5203, 1004.5970,  236.2885],
        [ 684.1226,  485.5577,  797.2910,  537.9950],
        [ 720.1610,  590.9106,  829.6254,  648.8839]], device='cuda:0')
xyxyn: tensor([[0.6365, 0.5431, 0.7651, 0.6245],
        [0.6017, 0.2757, 0.7848, 0.3282],
        [0.5345, 0.6744, 0.6229, 0.7472],
        [0.5626, 0.8207, 0.6481, 0.9012]], device='cuda:0')

0: 384x640 4 Potholes, 16.2ms
Speed: 5.7ms preprocess, 16.2ms inference, 5.7ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.6908, 0.5850, 0.5294, 0.2826], device='cuda:0')
data: tensor([[8.2020e+02, 3.9698e+02, 1.0058e+03, 4.6665e+02, 6.9077e-01, 0.0000e+00],
        [7.7728e+02, 1.9860e+02, 1.0074e+03, 2.4179e+02, 5.8502e-01, 0.0000e+00],
        [6.9740e+02, 5.0506e+02, 8.3028e+02, 5.7370e+02, 5.2937e-01, 0.0000e+00],
        [7.6960e+02, 3.5698e+02, 8.8857e+02, 3.8870e+02, 2.8260e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([4, 6])
xywh: tensor([[912.9819, 431.8148, 185.5725,  69.6791],
        [892.3475, 220.1956, 230.1313,  43.1885],
        [763.8409, 539.3802, 132.8777,  68.6313],
        [829.0869, 372.8393, 118.9684,  31.7158]], device='cuda:0')
xywhn: tensor([[0.7133, 0.5997, 0.1450, 0.0968],
        [0.6971, 0.3058, 0.1798, 0.0600],
        [0.5968, 0.7491, 0.1038, 0.0953],
        [0.6477, 0.5178, 0.0929, 0.0440]], device='cuda:0')
xyxy: tensor([[ 820.1957,  396.9752, 1005.7682,  466.6543],
        [ 777.2819,  198.6014, 1007.4132,  241.7899],
        [ 697.4020,  505.0646,  830.2797,  573.6959],
        [ 769.6027,  356.9814,  888.5710,  388.6972]], device='cuda:0')
xyxyn: tensor([[0.6408, 0.5514, 0.7858, 0.6481],
        [0.6073, 0.2758, 0.7870, 0.3358],
        [0.5448, 0.7015, 0.6487, 0.7968],
        [0.6013, 0.4958, 0.6942, 0.5399]], device='cuda:0')

0: 384x640 5 Potholes, 10.5ms
Speed: 2.0ms preprocess, 10.5ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.5986, 0.5868, 0.5222, 0.3063, 0.2625], device='cuda:0')
data: tensor([[7.0013e+02, 5.1889e+02, 8.2361e+02, 5.8525e+02, 5.9861e-01, 0.0000e+00],
        [7.8004e+02, 2.0087e+02, 9.9866e+02, 2.4301e+02, 5.8676e-01, 0.0000e+00],
        [8.2453e+02, 4.0642e+02, 1.0197e+03, 4.7273e+02, 5.2221e-01, 0.0000e+00],
        [7.7351e+02, 3.6070e+02, 8.9572e+02, 3.9509e+02, 3.0627e-01, 0.0000e+00],
        [7.4419e+02, 6.3782e+02, 8.7211e+02, 7.1652e+02, 2.6252e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([5, 6])
xywh: tensor([[761.8712, 552.0693, 123.4751,  66.3530],
        [889.3455, 221.9380, 218.6200,  42.1405],
        [922.1282, 439.5754, 195.1932,  66.3115],
        [834.6143, 377.8922, 122.2119,  34.3887],
        [808.1493, 677.1724, 127.9126,  78.7048]], device='cuda:0')
xywhn: tensor([[0.5952, 0.7668, 0.0965, 0.0922],
        [0.6948, 0.3082, 0.1708, 0.0585],
        [0.7204, 0.6105, 0.1525, 0.0921],
        [0.6520, 0.5249, 0.0955, 0.0478],
        [0.6314, 0.9405, 0.0999, 0.1093]], device='cuda:0')
xyxy: tensor([[ 700.1337,  518.8928,  823.6088,  585.2458],
        [ 780.0355,  200.8677,  998.6555,  243.0082],
        [ 824.5316,  406.4197, 1019.7249,  472.7312],
        [ 773.5083,  360.6978,  895.7202,  395.0865],
        [ 744.1930,  637.8200,  872.1056,  716.5248]], device='cuda:0')
xyxyn: tensor([[0.5470, 0.7207, 0.6434, 0.8128],
        [0.6094, 0.2790, 0.7802, 0.3375],
        [0.6442, 0.5645, 0.7967, 0.6566],
        [0.6043, 0.5010, 0.6998, 0.5487],
        [0.5814, 0.8859, 0.6813, 0.9952]], device='cuda:0')

0: 384x640 6 Potholes, 9.4ms
Speed: 2.9ms preprocess, 9.4ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.7279, 0.7125, 0.6233, 0.4776, 0.2937, 0.2931], device='cuda:0')
data: tensor([[8.2993e+02, 4.1576e+02, 1.0251e+03, 4.8260e+02, 7.2792e-01, 0.0000e+00],
        [7.0381e+02, 5.3029e+02, 8.3699e+02, 5.9380e+02, 7.1249e-01, 0.0000e+00],
        [7.8310e+02, 2.0115e+02, 1.0050e+03, 2.4327e+02, 6.2329e-01, 0.0000e+00],
        [7.7864e+02, 3.6412e+02, 9.0507e+02, 4.0024e+02, 4.7763e-01, 0.0000e+00],
        [4.7422e+02, 2.3266e+02, 7.0941e+02, 2.5935e+02, 2.9368e-01, 0.0000e+00],
        [3.6212e+02, 4.4835e+02, 5.7611e+02, 5.1873e+02, 2.9306e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([6, 6])
xywh: tensor([[927.5173, 449.1822, 195.1846,  66.8375],
        [770.4019, 562.0464, 133.1816,  63.5077],
        [894.0392, 222.2124, 221.8821,  42.1170],
        [841.8556, 382.1830, 126.4277,  36.1238],
        [591.8115, 246.0016, 235.1889,  26.6929],
        [469.1158, 483.5432, 213.9976,  70.3826]], device='cuda:0')
xywhn: tensor([[0.7246, 0.6239, 0.1525, 0.0928],
        [0.6019, 0.7806, 0.1040, 0.0882],
        [0.6985, 0.3086, 0.1733, 0.0585],
        [0.6577, 0.5308, 0.0988, 0.0502],
        [0.4624, 0.3417, 0.1837, 0.0371],
        [0.3665, 0.6716, 0.1672, 0.0978]], device='cuda:0')
xyxy: tensor([[ 829.9250,  415.7634, 1025.1096,  482.6010],
        [ 703.8110,  530.2926,  836.9927,  593.8003],
        [ 783.0982,  201.1539, 1004.9803,  243.2709],
        [ 778.6417,  364.1211,  905.0695,  400.2449],
        [ 474.2171,  232.6552,  709.4060,  259.3481],
        [ 362.1169,  448.3519,  576.1146,  518.7344]], device='cuda:0')
xyxyn: tensor([[0.6484, 0.5774, 0.8009, 0.6703],
        [0.5499, 0.7365, 0.6539, 0.8247],
        [0.6118, 0.2794, 0.7851, 0.3379],
        [0.6083, 0.5057, 0.7071, 0.5559],
        [0.3705, 0.3231, 0.5542, 0.3602],
        [0.2829, 0.6227, 0.4501, 0.7205]], device='cuda:0')

0: 384x640 5 Potholes, 9.5ms
Speed: 7.6ms preprocess, 9.5ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.6787, 0.5670, 0.4746, 0.4382, 0.3150], device='cuda:0')
data: tensor([[8.4457e+02, 4.2472e+02, 1.0528e+03, 5.0408e+02, 6.7873e-01, 0.0000e+00],
        [7.2030e+02, 5.5178e+02, 9.2165e+02, 6.4477e+02, 5.6695e-01, 0.0000e+00],
        [3.4963e+02, 4.6203e+02, 5.7811e+02, 5.3835e+02, 4.7456e-01, 0.0000e+00],
        [7.8834e+02, 2.0238e+02, 1.0190e+03, 2.4531e+02, 4.3818e-01, 0.0000e+00],
        [7.2095e+02, 5.4999e+02, 9.2232e+02, 6.8637e+02, 3.1503e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([5, 6])
xywh: tensor([[948.6907, 464.3978, 208.2362,  79.3584],
        [820.9708, 598.2744, 201.3494,  92.9829],
        [463.8701, 500.1934, 228.4789,  76.3219],
        [903.6578, 223.8443, 230.6421,  42.9260],
        [821.6369, 618.1813, 201.3741, 136.3857]], device='cuda:0')
xywhn: tensor([[0.7412, 0.6450, 0.1627, 0.1102],
        [0.6414, 0.8309, 0.1573, 0.1291],
        [0.3624, 0.6947, 0.1785, 0.1060],
        [0.7060, 0.3109, 0.1802, 0.0596],
        [0.6419, 0.8586, 0.1573, 0.1894]], device='cuda:0')
xyxy: tensor([[ 844.5726,  424.7186, 1052.8088,  504.0770],
        [ 720.2961,  551.7830,  921.6455,  644.7659],
        [ 349.6306,  462.0325,  578.1096,  538.3544],
        [ 788.3368,  202.3813, 1018.9789,  245.3073],
        [ 720.9498,  549.9884,  922.3240,  686.3741]], device='cuda:0')
xyxyn: tensor([[0.6598, 0.5899, 0.8225, 0.7001],
        [0.5627, 0.7664, 0.7200, 0.8955],
        [0.2731, 0.6417, 0.4516, 0.7477],
        [0.6159, 0.2811, 0.7961, 0.3407],
        [0.5632, 0.7639, 0.7206, 0.9533]], device='cuda:0')

0: 384x640 5 Potholes, 12.7ms
Speed: 2.1ms preprocess, 12.7ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.6000, 0.4915, 0.4654, 0.4511, 0.3059], device='cuda:0')
data: tensor([[8.5508e+02, 4.3851e+02, 1.0586e+03, 5.1554e+02, 6.0005e-01, 0.0000e+00],
        [7.2979e+02, 5.6600e+02, 9.0922e+02, 6.6195e+02, 4.9151e-01, 0.0000e+00],
        [7.8938e+02, 2.0356e+02, 1.0259e+03, 2.4728e+02, 4.6535e-01, 0.0000e+00],
        [7.9527e+02, 3.8061e+02, 9.3345e+02, 4.1859e+02, 4.5112e-01, 0.0000e+00],
        [3.4108e+02, 4.7466e+02, 5.7985e+02, 5.5167e+02, 3.0594e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([5, 6])
xywh: tensor([[956.8322, 477.0255, 203.5120,  77.0324],
        [819.5051, 613.9781, 179.4331,  95.9465],
        [907.6370, 225.4202, 236.5137,  43.7252],
        [864.3607, 399.5981, 138.1760,  37.9742],
        [460.4656, 513.1631, 238.7667,  77.0039]], device='cuda:0')
xywhn: tensor([[0.7475, 0.6625, 0.1590, 0.1070],
        [0.6402, 0.8527, 0.1402, 0.1333],
        [0.7091, 0.3131, 0.1848, 0.0607],
        [0.6753, 0.5550, 0.1080, 0.0527],
        [0.3597, 0.7127, 0.1865, 0.1069]], device='cuda:0')
xyxy: tensor([[ 855.0762,  438.5093, 1058.5881,  515.5417],
        [ 729.7886,  566.0049,  909.2217,  661.9514],
        [ 789.3801,  203.5576, 1025.8938,  247.2828],
        [ 795.2727,  380.6110,  933.4487,  418.5852],
        [ 341.0823,  474.6612,  579.8490,  551.6651]], device='cuda:0')
xyxyn: tensor([[0.6680, 0.6090, 0.8270, 0.7160],
        [0.5701, 0.7861, 0.7103, 0.9194],
        [0.6167, 0.2827, 0.8015, 0.3434],
        [0.6213, 0.5286, 0.7293, 0.5814],
        [0.2665, 0.6593, 0.4530, 0.7662]], device='cuda:0')

0: 384x640 5 Potholes, 10.0ms
Speed: 2.8ms preprocess, 10.0ms inference, 2.6ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.8091, 0.4852, 0.4663, 0.4058, 0.3087], device='cuda:0')
data: tensor([[8.6102e+02, 4.4499e+02, 1.0782e+03, 5.2835e+02, 8.0911e-01, 0.0000e+00],
        [7.9228e+02, 2.0415e+02, 1.0267e+03, 2.4877e+02, 4.8522e-01, 0.0000e+00],
        [7.9817e+02, 3.8621e+02, 9.3664e+02, 4.2620e+02, 4.6627e-01, 0.0000e+00],
        [2.5727e+02, 4.8383e+02, 5.8045e+02, 5.6490e+02, 4.0577e-01, 0.0000e+00],
        [7.3331e+02, 5.8074e+02, 9.4043e+02, 7.1152e+02, 3.0866e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([5, 6])
xywh: tensor([[969.5951, 486.6658, 217.1506,  83.3613],
        [909.4921, 226.4594, 234.4149,  44.6157],
        [867.4057, 406.2048, 138.4629,  39.9894],
        [418.8628, 524.3647, 323.1826,  81.0756],
        [836.8724, 646.1315, 207.1177, 130.7863]], device='cuda:0')
xywhn: tensor([[0.7575, 0.6759, 0.1696, 0.1158],
        [0.7105, 0.3145, 0.1831, 0.0620],
        [0.6777, 0.5642, 0.1082, 0.0555],
        [0.3272, 0.7283, 0.2525, 0.1126],
        [0.6538, 0.8974, 0.1618, 0.1816]], device='cuda:0')
xyxy: tensor([[ 861.0198,  444.9851, 1078.1704,  528.3464],
        [ 792.2847,  204.1516, 1026.6996,  248.7673],
        [ 798.1743,  386.2101,  936.6371,  426.1996],
        [ 257.2715,  483.8269,  580.4541,  564.9025],
        [ 733.3135,  580.7383,  940.4312,  711.5246]], device='cuda:0')
xyxyn: tensor([[0.6727, 0.6180, 0.8423, 0.7338],
        [0.6190, 0.2835, 0.8021, 0.3455],
        [0.6236, 0.5364, 0.7317, 0.5919],
        [0.2010, 0.6720, 0.4535, 0.7846],
        [0.5729, 0.8066, 0.7347, 0.9882]], device='cuda:0')

0: 384x640 4 Potholes, 11.8ms
Speed: 2.1ms preprocess, 11.8ms inference, 1.9ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.5427, 0.5266, 0.4700, 0.3322], device='cuda:0')
data: tensor([[8.0461e+02, 3.9213e+02, 9.5178e+02, 4.3281e+02, 5.4267e-01, 0.0000e+00],
        [8.6717e+02, 4.5251e+02, 1.0940e+03, 5.3826e+02, 5.2659e-01, 0.0000e+00],
        [7.9309e+02, 2.0441e+02, 1.0402e+03, 2.5044e+02, 4.6997e-01, 0.0000e+00],
        [7.4135e+02, 5.9504e+02, 9.7484e+02, 7.1870e+02, 3.3225e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([4, 6])
xywh: tensor([[878.1998, 412.4727, 147.1699,  40.6768],
        [980.5967, 495.3852, 226.8545,  85.7427],
        [916.6648, 227.4240, 247.1511,  46.0251],
        [858.0970, 656.8732, 233.4847, 123.6626]], device='cuda:0')
xywhn: tensor([[0.6861, 0.5729, 0.1150, 0.0565],
        [0.7661, 0.6880, 0.1772, 0.1191],
        [0.7161, 0.3159, 0.1931, 0.0639],
        [0.6704, 0.9123, 0.1824, 0.1718]], device='cuda:0')
xyxy: tensor([[ 804.6149,  392.1343,  951.7848,  432.8111],
        [ 867.1694,  452.5139, 1094.0239,  538.2565],
        [ 793.0892,  204.4114, 1040.2404,  250.4365],
        [ 741.3547,  595.0419,  974.8394,  718.7045]], device='cuda:0')
xyxyn: tensor([[0.6286, 0.5446, 0.7436, 0.6011],
        [0.6775, 0.6285, 0.8547, 0.7476],
        [0.6196, 0.2839, 0.8127, 0.3478],
        [0.5792, 0.8264, 0.7616, 0.9982]], device='cuda:0')

0: 384x640 9 Potholes, 12.4ms
Speed: 2.1ms preprocess, 12.4ms inference, 2.1ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0., 0., 0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.7631, 0.5769, 0.4300, 0.4222, 0.4042, 0.3642, 0.2948, 0.2670, 0.2662], device='cuda:0')
data: tensor([[8.8499e+02, 4.6691e+02, 1.1241e+03, 5.6678e+02, 7.6314e-01, 0.0000e+00],
        [7.0113e+02, 6.2629e+02, 9.7805e+02, 7.2000e+02, 5.7691e-01, 0.0000e+00],
        [7.9495e+02, 2.0573e+02, 1.0648e+03, 2.5439e+02, 4.3002e-01, 0.0000e+00],
        [8.1907e+02, 4.0158e+02, 9.7075e+02, 4.4915e+02, 4.2221e-01, 0.0000e+00],
        [1.3582e+01, 5.1924e+02, 5.8825e+02, 6.2351e+02, 4.0418e-01, 0.0000e+00],
        [2.6186e+02, 5.1640e+02, 5.8799e+02, 6.1405e+02, 3.6423e-01, 0.0000e+00],
        [3.1245e+02, 3.0146e+02, 4.9212e+02, 3.4534e+02, 2.9480e-01, 0.0000e+00],
        [1.4405e+02, 3.9249e+02, 2.9008e+02, 4.5823e+02, 2.6699e-01, 0.0000e+00],
        [7.9420e+00, 5.2431e+02, 5.8649e+02, 6.6332e+02, 2.6615e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([9, 6])
xywh: tensor([[1004.5370,  516.8450,  239.0903,   99.8740],
        [ 839.5911,  673.1436,  276.9177,   93.7129],
        [ 929.8856,  230.0627,  269.8701,   48.6631],
        [ 894.9116,  425.3642,  151.6860,   47.5760],
        [ 300.9145,  571.3737,  574.6642,  104.2687],
        [ 424.9285,  565.2264,  326.1305,   97.6536],
        [ 402.2848,  323.3986,  179.6670,   43.8866],
        [ 217.0656,  425.3602,  146.0246,   65.7347],
        [ 297.2139,  593.8174,  578.5437,  139.0068]], device='cuda:0')
xywhn: tensor([[0.7848, 0.7178, 0.1868, 0.1387],
        [0.6559, 0.9349, 0.2163, 0.1302],
        [0.7265, 0.3195, 0.2108, 0.0676],
        [0.6991, 0.5908, 0.1185, 0.0661],
        [0.2351, 0.7936, 0.4490, 0.1448],
        [0.3320, 0.7850, 0.2548, 0.1356],
        [0.3143, 0.4492, 0.1404, 0.0610],
        [0.1696, 0.5908, 0.1141, 0.0913],
        [0.2322, 0.8247, 0.4520, 0.1931]], device='cuda:0')
xyxy: tensor([[ 884.9918,  466.9080, 1124.0822,  566.7820],
        [ 701.1322,  626.2871,  978.0499,  720.0000],
        [ 794.9506,  205.7312, 1064.8207,  254.3943],
        [ 819.0686,  401.5762,  970.7546,  449.1522],
        [  13.5824,  519.2394,  588.2466,  623.5081],
        [ 261.8632,  516.3996,  587.9937,  614.0532],
        [ 312.4513,  301.4553,  492.1183,  345.3419],
        [ 144.0533,  392.4928,  290.0779,  458.2275],
        [   7.9420,  524.3140,  586.4857,  663.3208]], device='cuda:0')
xyxyn: tensor([[0.6914, 0.6485, 0.8782, 0.7872],
        [0.5478, 0.8698, 0.7641, 1.0000],
        [0.6211, 0.2857, 0.8319, 0.3533],
        [0.6399, 0.5577, 0.7584, 0.6238],
        [0.0106, 0.7212, 0.4596, 0.8660],
        [0.2046, 0.7172, 0.4594, 0.8529],
        [0.2441, 0.4187, 0.3845, 0.4796],
        [0.1125, 0.5451, 0.2266, 0.6364],
        [0.0062, 0.7282, 0.4582, 0.9213]], device='cuda:0')

0: 384x640 10 Potholes, 14.4ms
Speed: 3.4ms preprocess, 14.4ms inference, 2.7ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0., 0., 0., 0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.7501, 0.5964, 0.5787, 0.5532, 0.4540, 0.4056, 0.3258, 0.3234, 0.2926, 0.2707], device='cuda:0')
data: tensor([[8.8917e+02, 4.7492e+02, 1.1351e+03, 5.7866e+02, 7.5007e-01, 0.0000e+00],
        [8.2353e+02, 4.0969e+02, 9.8133e+02, 4.5780e+02, 5.9644e-01, 0.0000e+00],
        [7.0230e+02, 6.4494e+02, 9.6799e+02, 7.2000e+02, 5.7869e-01, 0.0000e+00],
        [3.2527e+02, 5.2701e+02, 5.9204e+02, 6.2742e+02, 5.5319e-01, 0.0000e+00],
        [7.7601e+02, 6.4484e+02, 9.6121e+02, 7.2000e+02, 4.5402e-01, 0.0000e+00],
        [7.9963e+02, 2.0694e+02, 1.0665e+03, 2.5627e+02, 4.0562e-01, 0.0000e+00],
        [1.5933e+02, 5.2895e+02, 5.9326e+02, 6.3851e+02, 3.2583e-01, 0.0000e+00],
        [3.1446e+02, 3.0108e+02, 4.9954e+02, 3.4437e+02, 3.2338e-01, 0.0000e+00],
        [8.1519e+00, 5.3368e+02, 5.8907e+02, 6.6618e+02, 2.9261e-01, 0.0000e+00],
        [1.3243e+02, 3.9723e+02, 2.8774e+02, 4.6849e+02, 2.7071e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([10, 6])
xywh: tensor([[1012.1341,  526.7883,  245.9327,  103.7385],
        [ 902.4304,  433.7452,  157.8008,   48.1183],
        [ 835.1443,  682.4700,  265.6897,   75.0599],
        [ 458.6531,  577.2135,  266.7726,  100.4062],
        [ 868.6083,  682.4180,  185.1979,   75.1639],
        [ 933.0853,  231.6019,  266.9034,   49.3289],
        [ 376.2952,  583.7319,  433.9288,  109.5557],
        [ 406.9975,  322.7236,  185.0750,   43.2852],
        [ 298.6125,  599.9285,  580.9214,  132.4978],
        [ 210.0862,  432.8610,  155.3075,   71.2549]], device='cuda:0')
xywhn: tensor([[0.7907, 0.7317, 0.1921, 0.1441],
        [0.7050, 0.6024, 0.1233, 0.0668],
        [0.6525, 0.9479, 0.2076, 0.1042],
        [0.3583, 0.8017, 0.2084, 0.1395],
        [0.6786, 0.9478, 0.1447, 0.1044],
        [0.7290, 0.3217, 0.2085, 0.0685],
        [0.2940, 0.8107, 0.3390, 0.1522],
        [0.3180, 0.4482, 0.1446, 0.0601],
        [0.2333, 0.8332, 0.4538, 0.1840],
        [0.1641, 0.6012, 0.1213, 0.0990]], device='cuda:0')
xyxy: tensor([[ 889.1677,  474.9190, 1135.1005,  578.6575],
        [ 823.5300,  409.6860,  981.3308,  457.8043],
        [ 702.2994,  644.9401,  967.9891,  720.0000],
        [ 325.2668,  527.0104,  592.0394,  627.4166],
        [ 776.0093,  644.8361,  961.2072,  720.0000],
        [ 799.6335,  206.9374, 1066.5370,  256.2663],
        [ 159.3308,  528.9541,  593.2596,  638.5098],
        [ 314.4601,  301.0810,  499.5350,  344.3662],
        [   8.1519,  533.6796,  589.0732,  666.1774],
        [ 132.4325,  397.2335,  287.7400,  468.4884]], device='cuda:0')
xyxyn: tensor([[0.6947, 0.6596, 0.8868, 0.8037],
        [0.6434, 0.5690, 0.7667, 0.6358],
        [0.5487, 0.8958, 0.7562, 1.0000],
        [0.2541, 0.7320, 0.4625, 0.8714],
        [0.6063, 0.8956, 0.7509, 1.0000],
        [0.6247, 0.2874, 0.8332, 0.3559],
        [0.1245, 0.7347, 0.4635, 0.8868],
        [0.2457, 0.4182, 0.3903, 0.4783],
        [0.0064, 0.7412, 0.4602, 0.9252],
        [0.1035, 0.5517, 0.2248, 0.6507]], device='cuda:0')

0: 384x640 8 Potholes, 13.1ms
Speed: 3.4ms preprocess, 13.1ms inference, 2.5ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0., 0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.7651, 0.6492, 0.4994, 0.3782, 0.3690, 0.3673, 0.3217, 0.3083], device='cuda:0')
data: tensor([[9.0831e+02, 4.8654e+02, 1.1555e+03, 5.9590e+02, 7.6513e-01, 0.0000e+00],
        [8.3025e+02, 4.1896e+02, 9.9528e+02, 4.6448e+02, 6.4924e-01, 0.0000e+00],
        [2.7799e+02, 5.4579e+02, 6.0005e+02, 6.6059e+02, 4.9939e-01, 0.0000e+00],
        [8.0227e+02, 2.0764e+02, 1.0697e+03, 2.5588e+02, 3.7816e-01, 0.0000e+00],
        [6.8265e+02, 6.2547e+02, 1.0018e+03, 7.2000e+02, 3.6900e-01, 0.0000e+00],
        [3.1434e+02, 3.0519e+02, 4.9360e+02, 3.5508e+02, 3.6729e-01, 0.0000e+00],
        [1.3096e+02, 4.0650e+02, 2.8725e+02, 4.7849e+02, 3.2174e-01, 0.0000e+00],
        [2.6887e+00, 5.4593e+02, 5.9577e+02, 7.1227e+02, 3.0826e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([8, 6])
xywh: tensor([[1031.8826,  541.2172,  247.1524,  109.3594],
        [ 912.7650,  441.7183,  165.0399,   45.5221],
        [ 439.0176,  603.1892,  322.0640,  114.7954],
        [ 935.9714,  231.7627,  267.4033,   48.2404],
        [ 842.2298,  672.7368,  319.1516,   94.5264],
        [ 403.9688,  330.1320,  179.2582,   49.8895],
        [ 209.1062,  442.4971,  156.2861,   71.9885],
        [ 299.2280,  629.0984,  593.0787,  166.3359]], device='cuda:0')
xywhn: tensor([[0.8062, 0.7517, 0.1931, 0.1519],
        [0.7131, 0.6135, 0.1289, 0.0632],
        [0.3430, 0.8378, 0.2516, 0.1594],
        [0.7312, 0.3219, 0.2089, 0.0670],
        [0.6580, 0.9344, 0.2493, 0.1313],
        [0.3156, 0.4585, 0.1400, 0.0693],
        [0.1634, 0.6146, 0.1221, 0.1000],
        [0.2338, 0.8737, 0.4633, 0.2310]], device='cuda:0')
xyxy: tensor([[ 908.3063,  486.5375, 1155.4587,  595.8969],
        [ 830.2451,  418.9572,  995.2850,  464.4793],
        [ 277.9856,  545.7915,  600.0496,  660.5869],
        [ 802.2698,  207.6425, 1069.6731,  255.8829],
        [ 682.6540,  625.4736, 1001.8056,  720.0000],
        [ 314.3397,  305.1873,  493.5979,  355.0768],
        [ 130.9632,  406.5029,  287.2493,  478.4914],
        [   2.6887,  545.9304,  595.7673,  712.2664]], device='cuda:0')
xyxyn: tensor([[0.7096, 0.6757, 0.9027, 0.8276],
        [0.6486, 0.5819, 0.7776, 0.6451],
        [0.2172, 0.7580, 0.4688, 0.9175],
        [0.6268, 0.2884, 0.8357, 0.3554],
        [0.5333, 0.8687, 0.7827, 1.0000],
        [0.2456, 0.4239, 0.3856, 0.4932],
        [0.1023, 0.5646, 0.2244, 0.6646],
        [0.0021, 0.7582, 0.4654, 0.9893]], device='cuda:0')

0: 384x640 4 Potholes, 13.7ms
Speed: 2.2ms preprocess, 13.7ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.7461, 0.4832, 0.4346, 0.4228], device='cuda:0')
data: tensor([[9.2257e+02, 5.1107e+02, 1.1919e+03, 6.2935e+02, 7.4611e-01, 0.0000e+00],
        [2.0480e+01, 5.7037e+02, 6.0769e+02, 7.1412e+02, 4.8324e-01, 0.0000e+00],
        [2.2636e+02, 5.7006e+02, 6.1257e+02, 7.1106e+02, 4.3461e-01, 0.0000e+00],
        [8.4602e+02, 4.3265e+02, 1.0192e+03, 4.8260e+02, 4.2284e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([4, 6])
xywh: tensor([[1057.2345,  570.2101,  269.3228,  118.2765],
        [ 314.0865,  642.2445,  587.2130,  143.7415],
        [ 419.4673,  640.5637,  386.2145,  140.9996],
        [ 932.6271,  457.6284,  173.2063,   49.9470]], device='cuda:0')
xywhn: tensor([[0.8260, 0.7920, 0.2104, 0.1643],
        [0.2454, 0.8920, 0.4588, 0.1996],
        [0.3277, 0.8897, 0.3017, 0.1958],
        [0.7286, 0.6356, 0.1353, 0.0694]], device='cuda:0')
xyxy: tensor([[ 922.5731,  511.0718, 1191.8959,  629.3483],
        [  20.4800,  570.3738,  607.6930,  714.1152],
        [ 226.3600,  570.0639,  612.5746,  711.0635],
        [ 846.0239,  432.6549, 1019.2302,  482.6019]], device='cuda:0')
xyxyn: tensor([[0.7208, 0.7098, 0.9312, 0.8741],
        [0.0160, 0.7922, 0.4748, 0.9918],
        [0.1768, 0.7918, 0.4786, 0.9876],
        [0.6610, 0.6009, 0.7963, 0.6703]], device='cuda:0')

0: 384x640 6 Potholes, 14.7ms
Speed: 2.0ms preprocess, 14.7ms inference, 1.9ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.8192, 0.6703, 0.6477, 0.3805, 0.3792, 0.3026], device='cuda:0')
data: tensor([[9.3723e+02, 5.1936e+02, 1.2158e+03, 6.4593e+02, 8.1919e-01, 0.0000e+00],
        [8.5233e+02, 4.3838e+02, 1.0306e+03, 5.0191e+02, 6.7029e-01, 0.0000e+00],
        [2.5888e+02, 5.8529e+02, 6.1047e+02, 7.2000e+02, 6.4771e-01, 0.0000e+00],
        [8.0809e+02, 2.0845e+02, 1.0894e+03, 2.5828e+02, 3.8047e-01, 0.0000e+00],
        [2.1523e+01, 5.8595e+02, 6.1194e+02, 7.2000e+02, 3.7918e-01, 0.0000e+00],
        [3.0501e+02, 3.1493e+02, 5.0052e+02, 3.7012e+02, 3.0260e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([6, 6])
xywh: tensor([[1076.5083,  582.6416,  278.5615,  126.5676],
        [ 941.4844,  470.1443,  178.3123,   63.5237],
        [ 434.6746,  652.6465,  351.5942,  134.7071],
        [ 948.7314,  233.3671,  281.2906,   49.8349],
        [ 316.7333,  652.9763,  590.4216,  134.0473],
        [ 402.7687,  342.5230,  195.5092,   55.1910]], device='cuda:0')
xywhn: tensor([[0.8410, 0.8092, 0.2176, 0.1758],
        [0.7355, 0.6530, 0.1393, 0.0882],
        [0.3396, 0.9065, 0.2747, 0.1871],
        [0.7412, 0.3241, 0.2198, 0.0692],
        [0.2474, 0.9069, 0.4613, 0.1862],
        [0.3147, 0.4757, 0.1527, 0.0767]], device='cuda:0')
xyxy: tensor([[ 937.2276,  519.3578, 1215.7891,  645.9254],
        [ 852.3282,  438.3824, 1030.6405,  501.9062],
        [ 258.8775,  585.2929,  610.4717,  720.0000],
        [ 808.0861,  208.4496, 1089.3767,  258.2845],
        [  21.5225,  585.9527,  611.9441,  720.0000],
        [ 305.0142,  314.9275,  500.5233,  370.1185]], device='cuda:0')
xyxyn: tensor([[0.7322, 0.7213, 0.9498, 0.8971],
        [0.6659, 0.6089, 0.8052, 0.6971],
        [0.2022, 0.8129, 0.4769, 1.0000],
        [0.6313, 0.2895, 0.8511, 0.3587],
        [0.0168, 0.8138, 0.4781, 1.0000],
        [0.2383, 0.4374, 0.3910, 0.5141]], device='cuda:0')

0: 384x640 6 Potholes, 19.4ms
Speed: 3.9ms preprocess, 19.4ms inference, 1.9ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.8202, 0.6600, 0.5974, 0.4480, 0.4330, 0.3654], device='cuda:0')
data: tensor([[9.4694e+02, 5.3218e+02, 1.2336e+03, 6.6239e+02, 8.2020e-01, 0.0000e+00],
        [8.5943e+02, 4.4779e+02, 1.0438e+03, 5.0713e+02, 6.5996e-01, 0.0000e+00],
        [1.8486e+02, 6.0118e+02, 6.2276e+02, 7.2000e+02, 5.9738e-01, 0.0000e+00],
        [9.0600e+01, 4.3652e+02, 2.6216e+02, 5.2177e+02, 4.4800e-01, 0.0000e+00],
        [2.9859e+02, 3.2043e+02, 5.0011e+02, 3.7535e+02, 4.3305e-01, 0.0000e+00],
        [8.1079e+02, 2.0863e+02, 1.0866e+03, 2.6117e+02, 3.6538e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([6, 6])
xywh: tensor([[1090.2711,  597.2825,  286.6702,  130.2131],
        [ 951.6001,  477.4557,  184.3315,   59.3392],
        [ 403.8116,  660.5906,  437.9012,  118.8187],
        [ 176.3806,  479.1429,  171.5615,   85.2477],
        [ 399.3474,  347.8872,  201.5212,   54.9183],
        [ 948.7186,  234.8992,  275.8611,   52.5369]], device='cuda:0')
xywhn: tensor([[0.8518, 0.8296, 0.2240, 0.1809],
        [0.7434, 0.6631, 0.1440, 0.0824],
        [0.3155, 0.9175, 0.3421, 0.1650],
        [0.1378, 0.6655, 0.1340, 0.1184],
        [0.3120, 0.4832, 0.1574, 0.0763],
        [0.7412, 0.3262, 0.2155, 0.0730]], device='cuda:0')
xyxy: tensor([[ 946.9360,  532.1759, 1233.6062,  662.3890],
        [ 859.4343,  447.7861, 1043.7659,  507.1253],
        [ 184.8610,  601.1813,  622.7622,  720.0000],
        [  90.5998,  436.5190,  262.1613,  521.7667],
        [ 298.5868,  320.4280,  500.1080,  375.3464],
        [ 810.7881,  208.6307, 1086.6492,  261.1676]], device='cuda:0')
xyxyn: tensor([[0.7398, 0.7391, 0.9638, 0.9200],
        [0.6714, 0.6219, 0.8154, 0.7043],
        [0.1444, 0.8350, 0.4865, 1.0000],
        [0.0708, 0.6063, 0.2048, 0.7247],
        [0.2333, 0.4450, 0.3907, 0.5213],
        [0.6334, 0.2898, 0.8489, 0.3627]], device='cuda:0')

0: 384x640 7 Potholes, 9.7ms
Speed: 2.6ms preprocess, 9.7ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.6561, 0.6411, 0.6396, 0.4599, 0.4382, 0.4003, 0.3599], device='cuda:0')
data: tensor([[9.7137e+02, 5.5720e+02, 1.2771e+03, 7.1491e+02, 6.5611e-01, 0.0000e+00],
        [2.5216e+02, 6.3583e+02, 6.3018e+02, 7.2000e+02, 6.4115e-01, 0.0000e+00],
        [8.7647e+02, 4.6337e+02, 1.0755e+03, 5.4098e+02, 6.3958e-01, 0.0000e+00],
        [7.1636e+01, 4.5442e+02, 2.6389e+02, 5.5013e+02, 4.5986e-01, 0.0000e+00],
        [8.1528e+02, 2.0923e+02, 1.1123e+03, 2.6770e+02, 4.3817e-01, 0.0000e+00],
        [4.7013e+02, 2.5668e+02, 7.5124e+02, 2.9285e+02, 4.0029e-01, 0.0000e+00],
        [2.8861e+02, 3.2890e+02, 4.9372e+02, 3.7589e+02, 3.5988e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([7, 6])
xywh: tensor([[1124.2316,  636.0561,  305.7305,  157.7145],
        [ 441.1678,  677.9147,  378.0234,   84.1705],
        [ 976.0010,  502.1778,  199.0590,   77.6117],
        [ 167.7637,  502.2732,  192.2557,   95.7037],
        [ 963.7942,  238.4642,  297.0195,   58.4739],
        [ 610.6857,  274.7653,  281.1049,   36.1745],
        [ 391.1653,  352.3915,  205.1140,   46.9879]], device='cuda:0')
xywhn: tensor([[0.8783, 0.8834, 0.2389, 0.2190],
        [0.3447, 0.9415, 0.2953, 0.1169],
        [0.7625, 0.6975, 0.1555, 0.1078],
        [0.1311, 0.6976, 0.1502, 0.1329],
        [0.7530, 0.3312, 0.2320, 0.0812],
        [0.4771, 0.3816, 0.2196, 0.0502],
        [0.3056, 0.4894, 0.1602, 0.0653]], device='cuda:0')
xyxy: tensor([[ 971.3663,  557.1989, 1277.0968,  714.9133],
        [ 252.1561,  635.8295,  630.1796,  720.0000],
        [ 876.4716,  463.3719, 1075.5305,  540.9836],
        [  71.6358,  454.4213,  263.8915,  550.1251],
        [ 815.2844,  209.2272, 1112.3040,  267.7011],
        [ 470.1333,  256.6780,  751.2382,  292.8525],
        [ 288.6083,  328.8975,  493.7224,  375.8854]], device='cuda:0')
xyxyn: tensor([[0.7589, 0.7739, 0.9977, 0.9929],
        [0.1970, 0.8831, 0.4923, 1.0000],
        [0.6847, 0.6436, 0.8403, 0.7514],
        [0.0560, 0.6311, 0.2062, 0.7641],
        [0.6369, 0.2906, 0.8690, 0.3718],
        [0.3673, 0.3565, 0.5869, 0.4067],
        [0.2255, 0.4568, 0.3857, 0.5221]], device='cuda:0')

0: 384x640 6 Potholes, 9.5ms
Speed: 2.2ms preprocess, 9.5ms inference, 1.9ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.7296, 0.6332, 0.5941, 0.5477, 0.5024, 0.2663], device='cuda:0')
data: tensor([[9.8510e+02, 5.7189e+02, 1.2800e+03, 7.2000e+02, 7.2960e-01, 0.0000e+00],
        [8.8381e+02, 4.7244e+02, 1.0854e+03, 5.4215e+02, 6.3319e-01, 0.0000e+00],
        [8.1651e+02, 2.1023e+02, 1.1093e+03, 2.6803e+02, 5.9407e-01, 0.0000e+00],
        [5.7717e+01, 4.6150e+02, 2.5556e+02, 5.6031e+02, 5.4770e-01, 0.0000e+00],
        [4.7117e+02, 2.5688e+02, 7.5376e+02, 2.9369e+02, 5.0238e-01, 0.0000e+00],
        [2.8522e+02, 3.3316e+02, 4.9660e+02, 3.8476e+02, 2.6630e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([6, 6])
xywh: tensor([[1132.5513,  645.9451,  294.8975,  148.1099],
        [ 984.6118,  507.2938,  201.6006,   69.7161],
        [ 962.9189,  239.1329,  292.8138,   57.7978],
        [ 156.6394,  510.9054,  197.8447,   98.8134],
        [ 612.4654,  275.2871,  282.5944,   36.8087],
        [ 390.9102,  358.9622,  211.3813,   51.6024]], device='cuda:0')
xywhn: tensor([[0.8848, 0.8971, 0.2304, 0.2057],
        [0.7692, 0.7046, 0.1575, 0.0968],
        [0.7523, 0.3321, 0.2288, 0.0803],
        [0.1224, 0.7096, 0.1546, 0.1372],
        [0.4785, 0.3823, 0.2208, 0.0511],
        [0.3054, 0.4986, 0.1651, 0.0717]], device='cuda:0')
xyxy: tensor([[ 985.1025,  571.8901, 1280.0000,  720.0000],
        [ 883.8115,  472.4357, 1085.4121,  542.1518],
        [ 816.5120,  210.2340, 1109.3258,  268.0318],
        [  57.7171,  461.4987,  255.5618,  560.3121],
        [ 471.1682,  256.8828,  753.7626,  293.6914],
        [ 285.2195,  333.1609,  496.6008,  384.7634]], device='cuda:0')
xyxyn: tensor([[0.7696, 0.7943, 1.0000, 1.0000],
        [0.6905, 0.6562, 0.8480, 0.7530],
        [0.6379, 0.2920, 0.8667, 0.3723],
        [0.0451, 0.6410, 0.1997, 0.7782],
        [0.3681, 0.3568, 0.5889, 0.4079],
        [0.2228, 0.4627, 0.3880, 0.5344]], device='cuda:0')

0: 384x640 5 Potholes, 10.2ms
Speed: 2.1ms preprocess, 10.2ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.7296, 0.5999, 0.5720, 0.5586, 0.4290], device='cuda:0')
data: tensor([[3.7102e+01, 4.7292e+02, 2.4874e+02, 5.7627e+02, 7.2961e-01, 0.0000e+00],
        [9.9731e+02, 5.8811e+02, 1.2800e+03, 7.2000e+02, 5.9994e-01, 0.0000e+00],
        [4.7381e+02, 2.5453e+02, 7.6138e+02, 2.9188e+02, 5.7203e-01, 0.0000e+00],
        [8.1646e+02, 2.1085e+02, 1.1224e+03, 2.6977e+02, 5.5864e-01, 0.0000e+00],
        [8.9223e+02, 4.8509e+02, 1.1044e+03, 5.6647e+02, 4.2900e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([5, 6])
xywh: tensor([[ 142.9234,  524.5941,  211.6429,  103.3491],
        [1138.6543,  654.0564,  282.6915,  131.8872],
        [ 617.5968,  273.2010,  287.5659,   37.3512],
        [ 969.4077,  240.3105,  305.8993,   58.9244],
        [ 998.3130,  525.7802,  212.1670,   81.3864]], device='cuda:0')
xywhn: tensor([[0.1117, 0.7286, 0.1653, 0.1435],
        [0.8896, 0.9084, 0.2209, 0.1832],
        [0.4825, 0.3794, 0.2247, 0.0519],
        [0.7573, 0.3338, 0.2390, 0.0818],
        [0.7799, 0.7303, 0.1658, 0.1130]], device='cuda:0')
xyxy: tensor([[  37.1019,  472.9196,  248.7448,  576.2687],
        [ 997.3085,  588.1128, 1280.0000,  720.0000],
        [ 473.8138,  254.5255,  761.3798,  291.8766],
        [ 816.4580,  210.8483, 1122.3573,  269.7728],
        [ 892.2295,  485.0870, 1104.3965,  566.4734]], device='cuda:0')
xyxyn: tensor([[0.0290, 0.6568, 0.1943, 0.8004],
        [0.7791, 0.8168, 1.0000, 1.0000],
        [0.3702, 0.3535, 0.5948, 0.4054],
        [0.6379, 0.2928, 0.8768, 0.3747],
        [0.6971, 0.6737, 0.8628, 0.7868]], device='cuda:0')

0: 384x640 6 Potholes, 15.3ms
Speed: 2.1ms preprocess, 15.3ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.7122, 0.6735, 0.6399, 0.5071, 0.3522, 0.3312], device='cuda:0')
data: tensor([[1.0146e+03, 6.0406e+02, 1.2800e+03, 7.2000e+02, 7.1222e-01, 0.0000e+00],
        [8.2096e+02, 2.1504e+02, 1.1161e+03, 2.7088e+02, 6.7353e-01, 0.0000e+00],
        [9.0562e+02, 4.9452e+02, 1.1226e+03, 5.8298e+02, 6.3993e-01, 0.0000e+00],
        [4.7339e+02, 2.5977e+02, 7.6665e+02, 2.9379e+02, 5.0707e-01, 0.0000e+00],
        [2.6304e+01, 4.8282e+02, 2.3797e+02, 5.8505e+02, 3.5217e-01, 0.0000e+00],
        [2.7396e+02, 3.3928e+02, 4.9138e+02, 3.8811e+02, 3.3123e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([6, 6])
xywh: tensor([[1147.2915,  662.0311,  265.4171,  115.9378],
        [ 968.5378,  242.9605,  295.1467,   55.8443],
        [1014.0926,  538.7490,  216.9398,   88.4674],
        [ 620.0223,  276.7825,  293.2600,   34.0184],
        [ 132.1396,  533.9355,  211.6706,  102.2302],
        [ 382.6692,  363.6964,  217.4235,   48.8293]], device='cuda:0')
xywhn: tensor([[0.8963, 0.9195, 0.2074, 0.1610],
        [0.7567, 0.3374, 0.2306, 0.0776],
        [0.7923, 0.7483, 0.1695, 0.1229],
        [0.4844, 0.3844, 0.2291, 0.0472],
        [0.1032, 0.7416, 0.1654, 0.1420],
        [0.2990, 0.5051, 0.1699, 0.0678]], device='cuda:0')
xyxy: tensor([[1014.5829,  604.0622, 1280.0000,  720.0000],
        [ 820.9645,  215.0384, 1116.1112,  270.8826],
        [ 905.6227,  494.5153, 1122.5625,  582.9827],
        [ 473.3923,  259.7733,  766.6523,  293.7917],
        [  26.3043,  482.8205,  237.9749,  585.0507],
        [ 273.9575,  339.2817,  491.3810,  388.1111]], device='cuda:0')
xyxyn: tensor([[0.7926, 0.8390, 1.0000, 1.0000],
        [0.6414, 0.2987, 0.8720, 0.3762],
        [0.7075, 0.6868, 0.8770, 0.8097],
        [0.3698, 0.3608, 0.5989, 0.4080],
        [0.0206, 0.6706, 0.1859, 0.8126],
        [0.2140, 0.4712, 0.3839, 0.5390]], device='cuda:0')

0: 384x640 7 Potholes, 11.8ms
Speed: 2.2ms preprocess, 11.8ms inference, 2.7ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.7811, 0.7227, 0.6736, 0.5206, 0.4553, 0.4263, 0.3787], device='cuda:0')
data: tensor([[9.2314e+02, 5.1588e+02, 1.1590e+03, 6.0682e+02, 7.8114e-01, 0.0000e+00],
        [1.0493e+03, 6.3813e+02, 1.2800e+03, 7.2000e+02, 7.2271e-01, 0.0000e+00],
        [8.2395e+02, 2.1712e+02, 1.1208e+03, 2.7476e+02, 6.7364e-01, 0.0000e+00],
        [3.6308e+00, 5.0795e+02, 2.1044e+02, 6.2330e+02, 5.2062e-01, 0.0000e+00],
        [4.6950e+02, 2.6712e+02, 7.6969e+02, 3.0357e+02, 4.5529e-01, 0.0000e+00],
        [7.8528e+02, 3.5028e+02, 8.8203e+02, 3.8147e+02, 4.2626e-01, 0.0000e+00],
        [2.6573e+02, 3.4493e+02, 5.0423e+02, 3.9872e+02, 3.7869e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([7, 6])
xywh: tensor([[1041.0625,  561.3488,  235.8442,   90.9407],
        [1164.6267,  679.0668,  230.7467,   81.8664],
        [ 972.3990,  245.9419,  296.8892,   57.6403],
        [ 107.0338,  565.6263,  206.8061,  115.3457],
        [ 619.5974,  285.3408,  300.1907,   36.4498],
        [ 833.6552,  365.8756,   96.7472,   31.1848],
        [ 384.9794,  371.8250,  238.5059,   53.7961]], device='cuda:0')
xywhn: tensor([[0.8133, 0.7797, 0.1843, 0.1263],
        [0.9099, 0.9431, 0.1803, 0.1137],
        [0.7597, 0.3416, 0.2319, 0.0801],
        [0.0836, 0.7856, 0.1616, 0.1602],
        [0.4841, 0.3963, 0.2345, 0.0506],
        [0.6513, 0.5082, 0.0756, 0.0433],
        [0.3008, 0.5164, 0.1863, 0.0747]], device='cuda:0')
xyxy: tensor([[ 923.1404,  515.8785, 1158.9846,  606.8192],
        [1049.2533,  638.1336, 1280.0000,  720.0000],
        [ 823.9545,  217.1217, 1120.8436,  274.7620],
        [   3.6308,  507.9535,  210.4368,  623.2992],
        [ 469.5021,  267.1159,  769.6927,  303.5657],
        [ 785.2816,  350.2832,  882.0288,  381.4680],
        [ 265.7264,  344.9269,  504.2323,  398.7230]], device='cuda:0')
xyxyn: tensor([[0.7212, 0.7165, 0.9055, 0.8428],
        [0.8197, 0.8863, 1.0000, 1.0000],
        [0.6437, 0.3016, 0.8757, 0.3816],
        [0.0028, 0.7055, 0.1644, 0.8657],
        [0.3668, 0.3710, 0.6013, 0.4216],
        [0.6135, 0.4865, 0.6891, 0.5298],
        [0.2076, 0.4791, 0.3939, 0.5538]], device='cuda:0')

0: 384x640 4 Potholes, 9.7ms
Speed: 2.0ms preprocess, 9.7ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.6466, 0.6348, 0.5926, 0.4177], device='cuda:0')
data: tensor([[9.3554e+02, 5.3130e+02, 1.1871e+03, 6.4102e+02, 6.4661e-01, 0.0000e+00],
        [8.2574e+02, 2.1846e+02, 1.1218e+03, 2.7769e+02, 6.3478e-01, 0.0000e+00],
        [4.7275e+02, 2.6954e+02, 7.7263e+02, 3.1184e+02, 5.9265e-01, 0.0000e+00],
        [2.6114e+02, 3.5233e+02, 4.8631e+02, 4.0345e+02, 4.1773e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([4, 6])
xywh: tensor([[1061.3298,  586.1615,  251.5703,  109.7197],
        [ 973.7912,  248.0783,  296.1119,   59.2320],
        [ 622.6879,  290.6890,  299.8831,   42.2944],
        [ 373.7249,  377.8893,  225.1723,   51.1212]], device='cuda:0')
xywhn: tensor([[0.8292, 0.8141, 0.1965, 0.1524],
        [0.7608, 0.3446, 0.2313, 0.0823],
        [0.4865, 0.4037, 0.2343, 0.0587],
        [0.2920, 0.5248, 0.1759, 0.0710]], device='cuda:0')
xyxy: tensor([[ 935.5447,  531.3016, 1187.1150,  641.0214],
        [ 825.7352,  218.4623, 1121.8472,  277.6943],
        [ 472.7464,  269.5417,  772.6295,  311.8362],
        [ 261.1387,  352.3287,  486.3110,  403.4499]], device='cuda:0')
xyxyn: tensor([[0.7309, 0.7379, 0.9274, 0.8903],
        [0.6451, 0.3034, 0.8764, 0.3857],
        [0.3693, 0.3744, 0.6036, 0.4331],
        [0.2040, 0.4893, 0.3799, 0.5603]], device='cuda:0')

0: 384x640 4 Potholes, 11.3ms
Speed: 2.0ms preprocess, 11.3ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.6269, 0.5821, 0.5479, 0.3195], device='cuda:0')
data: tensor([[8.3017e+02, 2.2052e+02, 1.1195e+03, 2.7968e+02, 6.2688e-01, 0.0000e+00],
        [4.6967e+02, 2.7179e+02, 7.8025e+02, 3.1177e+02, 5.8213e-01, 0.0000e+00],
        [9.4992e+02, 5.4441e+02, 1.2092e+03, 6.5371e+02, 5.4786e-01, 0.0000e+00],
        [2.5124e+02, 3.5671e+02, 4.8942e+02, 4.0932e+02, 3.1948e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([4, 6])
xywh: tensor([[ 974.8438,  250.1004,  289.3402,   59.1691],
        [ 624.9613,  291.7806,  310.5835,   39.9863],
        [1079.5623,  599.0626,  259.2854,  109.2970],
        [ 370.3291,  383.0123,  238.1734,   52.6131]], device='cuda:0')
xywhn: tensor([[0.7616, 0.3474, 0.2260, 0.0822],
        [0.4883, 0.4053, 0.2426, 0.0555],
        [0.8434, 0.8320, 0.2026, 0.1518],
        [0.2893, 0.5320, 0.1861, 0.0731]], device='cuda:0')
xyxy: tensor([[ 830.1737,  220.5158, 1119.5139,  279.6849],
        [ 469.6695,  271.7875,  780.2531,  311.7738],
        [ 949.9196,  544.4141, 1209.2050,  653.7111],
        [ 251.2424,  356.7057,  489.4158,  409.3188]], device='cuda:0')
xyxyn: tensor([[0.6486, 0.3063, 0.8746, 0.3885],
        [0.3669, 0.3775, 0.6096, 0.4330],
        [0.7421, 0.7561, 0.9447, 0.9079],
        [0.1963, 0.4954, 0.3824, 0.5685]], device='cuda:0')

0: 384x640 5 Potholes, 9.4ms
Speed: 1.9ms preprocess, 9.4ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.6758, 0.6739, 0.5146, 0.3308, 0.2587], device='cuda:0')
data: tensor([[9.7040e+02, 5.7078e+02, 1.2586e+03, 7.2000e+02, 6.7580e-01, 0.0000e+00],
        [4.6922e+02, 2.7116e+02, 7.8586e+02, 3.1602e+02, 6.7390e-01, 0.0000e+00],
        [8.3590e+02, 2.2166e+02, 1.1267e+03, 2.8261e+02, 5.1457e-01, 0.0000e+00],
        [2.3366e+02, 3.6861e+02, 4.7925e+02, 4.2441e+02, 3.3081e-01, 0.0000e+00],
        [8.0841e+02, 3.6789e+02, 9.0104e+02, 4.0238e+02, 2.5872e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([5, 6])
xywh: tensor([[1114.5159,  645.3909,  288.2246,  149.2181],
        [ 627.5371,  293.5884,  316.6366,   44.8668],
        [ 981.3195,  252.1378,  290.8340,   60.9459],
        [ 356.4563,  396.5117,  245.5866,   55.7933],
        [ 854.7238,  385.1311,   92.6359,   34.4879]], device='cuda:0')
xywhn: tensor([[0.8707, 0.8964, 0.2252, 0.2072],
        [0.4903, 0.4078, 0.2474, 0.0623],
        [0.7667, 0.3502, 0.2272, 0.0846],
        [0.2785, 0.5507, 0.1919, 0.0775],
        [0.6678, 0.5349, 0.0724, 0.0479]], device='cuda:0')
xyxy: tensor([[ 970.4036,  570.7819, 1258.6282,  720.0000],
        [ 469.2188,  271.1550,  785.8554,  316.0219],
        [ 835.9025,  221.6649, 1126.7365,  282.6107],
        [ 233.6630,  368.6150,  479.2496,  424.4083],
        [ 808.4058,  367.8872,  901.0417,  402.3751]], device='cuda:0')
xyxyn: tensor([[0.7581, 0.7928, 0.9833, 1.0000],
        [0.3666, 0.3766, 0.6139, 0.4389],
        [0.6530, 0.3079, 0.8803, 0.3925],
        [0.1825, 0.5120, 0.3744, 0.5895],
        [0.6316, 0.5110, 0.7039, 0.5589]], device='cuda:0')

0: 384x640 4 Potholes, 8.9ms
Speed: 3.2ms preprocess, 8.9ms inference, 2.0ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.8266, 0.7012, 0.7007, 0.3128], device='cuda:0')
data: tensor([[9.8404e+02, 5.8726e+02, 1.2782e+03, 7.2000e+02, 8.2660e-01, 0.0000e+00],
        [8.4016e+02, 2.2433e+02, 1.1195e+03, 2.8414e+02, 7.0119e-01, 0.0000e+00],
        [4.6902e+02, 2.7808e+02, 7.8619e+02, 3.2216e+02, 7.0066e-01, 0.0000e+00],
        [2.3237e+02, 3.7047e+02, 5.0111e+02, 4.3595e+02, 3.1279e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([4, 6])
xywh: tensor([[1131.1316,  653.6301,  294.1758,  132.7397],
        [ 979.8123,  254.2314,  279.2953,   59.8099],
        [ 627.6052,  300.1221,  317.1738,   44.0774],
        [ 366.7409,  403.2100,  268.7420,   65.4730]], device='cuda:0')
xywhn: tensor([[0.8837, 0.9078, 0.2298, 0.1844],
        [0.7655, 0.3531, 0.2182, 0.0831],
        [0.4903, 0.4168, 0.2478, 0.0612],
        [0.2865, 0.5600, 0.2100, 0.0909]], device='cuda:0')
xyxy: tensor([[ 984.0437,  587.2603, 1278.2195,  720.0000],
        [ 840.1647,  224.3264, 1119.4600,  284.1363],
        [ 469.0183,  278.0834,  786.1921,  322.1608],
        [ 232.3699,  370.4735,  501.1119,  435.9465]], device='cuda:0')
xyxyn: tensor([[0.7688, 0.8156, 0.9986, 1.0000],
        [0.6564, 0.3116, 0.8746, 0.3946],
        [0.3664, 0.3862, 0.6142, 0.4474],
        [0.1815, 0.5145, 0.3915, 0.6055]], device='cuda:0')

0: 384x640 5 Potholes, 9.3ms
Speed: 3.2ms preprocess, 9.3ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.7963, 0.7516, 0.6083, 0.5833, 0.4150], device='cuda:0')
data: tensor([[1.0015e+03, 6.0369e+02, 1.2761e+03, 7.2000e+02, 7.9632e-01, 0.0000e+00],
        [4.7313e+02, 2.8434e+02, 7.9044e+02, 3.3304e+02, 7.5158e-01, 0.0000e+00],
        [2.2879e+02, 3.8179e+02, 4.7703e+02, 4.4343e+02, 6.0833e-01, 0.0000e+00],
        [8.4415e+02, 2.2576e+02, 1.1330e+03, 2.8562e+02, 5.8331e-01, 0.0000e+00],
        [8.2075e+02, 3.8163e+02, 9.1593e+02, 4.1446e+02, 4.1497e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([5, 6])
xywh: tensor([[1138.8042,  661.8432,  274.6293,  116.3136],
        [ 631.7879,  308.6935,  317.3093,   48.6992],
        [ 352.9107,  412.6131,  248.2346,   61.6367],
        [ 988.5569,  255.6879,  288.8208,   59.8570],
        [ 868.3409,  398.0465,   95.1753,   32.8304]], device='cuda:0')
xywhn: tensor([[0.8897, 0.9192, 0.2146, 0.1615],
        [0.4936, 0.4287, 0.2479, 0.0676],
        [0.2757, 0.5731, 0.1939, 0.0856],
        [0.7723, 0.3551, 0.2256, 0.0831],
        [0.6784, 0.5528, 0.0744, 0.0456]], device='cuda:0')
xyxy: tensor([[1001.4896,  603.6864, 1276.1189,  720.0000],
        [ 473.1332,  284.3439,  790.4426,  333.0431],
        [ 228.7934,  381.7947,  477.0280,  443.4315],
        [ 844.1465,  225.7594, 1132.9673,  285.6164],
        [ 820.7533,  381.6313,  915.9286,  414.4618]], device='cuda:0')
xyxyn: tensor([[0.7824, 0.8385, 0.9970, 1.0000],
        [0.3696, 0.3949, 0.6175, 0.4626],
        [0.1787, 0.5303, 0.3727, 0.6159],
        [0.6595, 0.3136, 0.8851, 0.3967],
        [0.6412, 0.5300, 0.7156, 0.5756]], device='cuda:0')

0: 384x640 5 Potholes, 11.3ms
Speed: 2.2ms preprocess, 11.3ms inference, 1.9ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.7256, 0.7011, 0.5012, 0.4916, 0.3463], device='cuda:0')
data: tensor([[2.1953e+02, 3.8363e+02, 4.7906e+02, 4.6301e+02, 7.2565e-01, 0.0000e+00],
        [1.0255e+03, 6.3493e+02, 1.2717e+03, 7.2000e+02, 7.0106e-01, 0.0000e+00],
        [4.6825e+02, 2.8120e+02, 8.0169e+02, 3.2907e+02, 5.0123e-01, 0.0000e+00],
        [8.4919e+02, 2.3063e+02, 1.1862e+03, 2.9079e+02, 4.9159e-01, 0.0000e+00],
        [8.3151e+02, 3.9463e+02, 9.2771e+02, 4.2862e+02, 3.4627e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([5, 6])
xywh: tensor([[ 349.2968,  423.3213,  259.5297,   79.3853],
        [1148.6313,  677.4632,  246.2263,   85.0736],
        [ 634.9686,  305.1321,  333.4432,   47.8674],
        [1017.6938,  260.7080,  337.0020,   60.1659],
        [ 879.6086,  411.6216,   96.2029,   33.9921]], device='cuda:0')
xywhn: tensor([[0.2729, 0.5879, 0.2028, 0.1103],
        [0.8974, 0.9409, 0.1924, 0.1182],
        [0.4961, 0.4238, 0.2605, 0.0665],
        [0.7951, 0.3621, 0.2633, 0.0836],
        [0.6872, 0.5717, 0.0752, 0.0472]], device='cuda:0')
xyxy: tensor([[ 219.5320,  383.6286,  479.0616,  463.0139],
        [1025.5182,  634.9264, 1271.7445,  720.0000],
        [ 468.2469,  281.1984,  801.6902,  329.0659],
        [ 849.1929,  230.6250, 1186.1948,  290.7910],
        [ 831.5072,  394.6255,  927.7101,  428.6177]], device='cuda:0')
xyxyn: tensor([[0.1715, 0.5328, 0.3743, 0.6431],
        [0.8012, 0.8818, 0.9936, 1.0000],
        [0.3658, 0.3906, 0.6263, 0.4570],
        [0.6634, 0.3203, 0.9267, 0.4039],
        [0.6496, 0.5481, 0.7248, 0.5953]], device='cuda:0')

0: 384x640 6 Potholes, 12.3ms
Speed: 3.4ms preprocess, 12.3ms inference, 1.8ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.6656, 0.6353, 0.4902, 0.4694, 0.4277, 0.3439], device='cuda:0')
data: tensor([[2.1190e+02, 3.9570e+02, 4.8545e+02, 4.6611e+02, 6.6564e-01, 0.0000e+00],
        [1.0494e+03, 6.5238e+02, 1.2667e+03, 7.2000e+02, 6.3525e-01, 0.0000e+00],
        [4.7031e+02, 2.8787e+02, 8.0334e+02, 3.3354e+02, 4.9017e-01, 0.0000e+00],
        [8.5218e+02, 2.3196e+02, 1.2159e+03, 2.9293e+02, 4.6940e-01, 0.0000e+00],
        [4.7427e+02, 2.8859e+02, 8.0397e+02, 3.5337e+02, 4.2774e-01, 0.0000e+00],
        [8.3601e+02, 3.9875e+02, 9.4891e+02, 4.3688e+02, 3.4387e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([6, 6])
xywh: tensor([[ 348.6738,  430.9051,  273.5564,   70.4193],
        [1158.0618,  686.1921,  217.2300,   67.6158],
        [ 636.8243,  310.7047,  333.0320,   45.6738],
        [1034.0303,  262.4467,  363.7070,   60.9757],
        [ 639.1215,  320.9792,  329.7063,   64.7729],
        [ 892.4563,  417.8160,  112.8979,   38.1294]], device='cuda:0')
xywhn: tensor([[0.2724, 0.5985, 0.2137, 0.0978],
        [0.9047, 0.9530, 0.1697, 0.0939],
        [0.4975, 0.4315, 0.2602, 0.0634],
        [0.8078, 0.3645, 0.2841, 0.0847],
        [0.4993, 0.4458, 0.2576, 0.0900],
        [0.6972, 0.5803, 0.0882, 0.0530]], device='cuda:0')
xyxy: tensor([[ 211.8956,  395.6954,  485.4520,  466.1147],
        [1049.4468,  652.3842, 1266.6768,  720.0000],
        [ 470.3083,  287.8678,  803.3403,  333.5416],
        [ 852.1768,  231.9589, 1215.8838,  292.9346],
        [ 474.2684,  288.5928,  803.9747,  353.3657],
        [ 836.0073,  398.7513,  948.9053,  436.8807]], device='cuda:0')
xyxyn: tensor([[0.1655, 0.5496, 0.3793, 0.6474],
        [0.8199, 0.9061, 0.9896, 1.0000],
        [0.3674, 0.3998, 0.6276, 0.4633],
        [0.6658, 0.3222, 0.9499, 0.4069],
        [0.3705, 0.4008, 0.6281, 0.4908],
        [0.6531, 0.5538, 0.7413, 0.6068]], device='cuda:0')

0: 384x640 3 Potholes, 12.5ms
Speed: 3.7ms preprocess, 12.5ms inference, 2.0ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0.], device='cuda:0')
conf: tensor([0.6763, 0.6646, 0.6585], device='cuda:0')
data: tensor([[8.5461e+02, 2.3218e+02, 1.1907e+03, 2.9568e+02, 6.7628e-01, 0.0000e+00],
        [2.0025e+02, 4.0597e+02, 4.8054e+02, 4.7684e+02, 6.6457e-01, 0.0000e+00],
        [4.6997e+02, 2.8981e+02, 8.0834e+02, 3.3922e+02, 6.5847e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([3, 6])
xywh: tensor([[1022.6558,  263.9305,  336.0963,   63.4996],
        [ 340.3923,  441.4055,  280.2881,   70.8646],
        [ 639.1595,  314.5177,  338.3702,   49.4089]], device='cuda:0')
xywhn: tensor([[0.7989, 0.3666, 0.2626, 0.0882],
        [0.2659, 0.6131, 0.2190, 0.0984],
        [0.4993, 0.4368, 0.2644, 0.0686]], device='cuda:0')
xyxy: tensor([[ 854.6077,  232.1807, 1190.7040,  295.6804],
        [ 200.2483,  405.9731,  480.5364,  476.8378],
        [ 469.9744,  289.8132,  808.3446,  339.2222]], device='cuda:0')
xyxyn: tensor([[0.6677, 0.3225, 0.9302, 0.4107],
        [0.1564, 0.5639, 0.3754, 0.6623],
        [0.3672, 0.4025, 0.6315, 0.4711]], device='cuda:0')

0: 384x640 4 Potholes, 12.6ms
Speed: 2.0ms preprocess, 12.6ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.7473, 0.6856, 0.5965, 0.4242], device='cuda:0')
data: tensor([[4.6729e+02, 2.9628e+02, 8.0983e+02, 3.5056e+02, 7.4731e-01, 0.0000e+00],
        [1.9511e+02, 4.0974e+02, 4.7883e+02, 4.8536e+02, 6.8560e-01, 0.0000e+00],
        [8.5494e+02, 2.3296e+02, 1.2331e+03, 2.9761e+02, 5.9651e-01, 0.0000e+00],
        [8.5148e+02, 4.1377e+02, 9.5911e+02, 4.5276e+02, 4.2424e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([4, 6])
xywh: tensor([[ 638.5615,  323.4203,  342.5339,   54.2721],
        [ 336.9702,  447.5496,  283.7292,   75.6246],
        [1044.0082,  265.2870,  378.1384,   64.6512],
        [ 905.2917,  433.2692,  107.6323,   38.9912]], device='cuda:0')
xywhn: tensor([[0.4989, 0.4492, 0.2676, 0.0754],
        [0.2633, 0.6216, 0.2217, 0.1050],
        [0.8156, 0.3685, 0.2954, 0.0898],
        [0.7073, 0.6018, 0.0841, 0.0542]], device='cuda:0')
xyxy: tensor([[ 467.2945,  296.2843,  809.8284,  350.5564],
        [ 195.1056,  409.7372,  478.8347,  485.3619],
        [ 854.9390,  232.9614, 1233.0774,  297.6126],
        [ 851.4756,  413.7736,  959.1079,  452.7648]], device='cuda:0')
xyxyn: tensor([[0.3651, 0.4115, 0.6327, 0.4869],
        [0.1524, 0.5691, 0.3741, 0.6741],
        [0.6679, 0.3236, 0.9633, 0.4134],
        [0.6652, 0.5747, 0.7493, 0.6288]], device='cuda:0')

0: 384x640 4 Potholes, 11.0ms
Speed: 2.2ms preprocess, 11.0ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.5626, 0.5005, 0.3369, 0.2904], device='cuda:0')
data: tensor([[8.6153e+02, 2.3353e+02, 1.2628e+03, 3.0423e+02, 5.6262e-01, 0.0000e+00],
        [1.7214e+02, 4.2007e+02, 4.8756e+02, 5.0344e+02, 5.0046e-01, 0.0000e+00],
        [4.6313e+02, 2.9967e+02, 8.1424e+02, 3.5854e+02, 3.3692e-01, 0.0000e+00],
        [8.6871e+02, 4.2880e+02, 9.7199e+02, 4.6715e+02, 2.9042e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([4, 6])
xywh: tensor([[1062.1580,  268.8814,  401.2548,   70.6995],
        [ 329.8494,  461.7567,  315.4123,   83.3701],
        [ 638.6838,  329.1028,  351.1097,   58.8712],
        [ 920.3479,  447.9741,  103.2832,   38.3540]], device='cuda:0')
xywhn: tensor([[0.8298, 0.3734, 0.3135, 0.0982],
        [0.2577, 0.6413, 0.2464, 0.1158],
        [0.4990, 0.4571, 0.2743, 0.0818],
        [0.7190, 0.6222, 0.0807, 0.0533]], device='cuda:0')
xyxy: tensor([[ 861.5306,  233.5317, 1262.7854,  304.2311],
        [ 172.1432,  420.0717,  487.5555,  503.4417],
        [ 463.1290,  299.6672,  814.2387,  358.5385],
        [ 868.7063,  428.7971,  971.9895,  467.1511]], device='cuda:0')
xyxyn: tensor([[0.6731, 0.3243, 0.9866, 0.4225],
        [0.1345, 0.5834, 0.3809, 0.6992],
        [0.3618, 0.4162, 0.6361, 0.4980],
        [0.6787, 0.5956, 0.7594, 0.6488]], device='cuda:0')

0: 384x640 4 Potholes, 11.7ms
Speed: 2.6ms preprocess, 11.7ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.7002, 0.6808, 0.5219, 0.3393], device='cuda:0')
data: tensor([[1.6467e+02, 4.2197e+02, 5.1164e+02, 5.1767e+02, 7.0016e-01, 0.0000e+00],
        [4.6566e+02, 3.0553e+02, 8.1249e+02, 3.6583e+02, 6.8080e-01, 0.0000e+00],
        [8.6222e+02, 2.3446e+02, 1.2724e+03, 3.0684e+02, 5.2189e-01, 0.0000e+00],
        [8.7452e+02, 4.3208e+02, 9.7679e+02, 4.7656e+02, 3.3935e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([4, 6])
xywh: tensor([[ 338.1549,  469.8194,  346.9694,   95.7067],
        [ 639.0752,  335.6792,  346.8274,   60.3002],
        [1067.3242,  270.6503,  410.2017,   72.3755],
        [ 925.6506,  454.3184,  102.2705,   44.4769]], device='cuda:0')
xywhn: tensor([[0.2642, 0.6525, 0.2711, 0.1329],
        [0.4993, 0.4662, 0.2710, 0.0838],
        [0.8338, 0.3759, 0.3205, 0.1005],
        [0.7232, 0.6310, 0.0799, 0.0618]], device='cuda:0')
xyxy: tensor([[ 164.6702,  421.9661,  511.6396,  517.6727],
        [ 465.6615,  305.5291,  812.4889,  365.8293],
        [ 862.2234,  234.4625, 1272.4250,  306.8381],
        [ 874.5153,  432.0799,  976.7858,  476.5568]], device='cuda:0')
xyxyn: tensor([[0.1286, 0.5861, 0.3997, 0.7190],
        [0.3638, 0.4243, 0.6348, 0.5081],
        [0.6736, 0.3256, 0.9941, 0.4262],
        [0.6832, 0.6001, 0.7631, 0.6619]], device='cuda:0')

0: 384x640 4 Potholes, 9.5ms
Speed: 2.2ms preprocess, 9.5ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.7087, 0.6531, 0.4982, 0.4907], device='cuda:0')
data: tensor([[1.5967e+02, 4.3645e+02, 4.8099e+02, 5.2984e+02, 7.0871e-01, 0.0000e+00],
        [8.7012e+02, 2.3536e+02, 1.2648e+03, 3.0925e+02, 6.5310e-01, 0.0000e+00],
        [8.7905e+02, 4.4113e+02, 9.8834e+02, 4.8547e+02, 4.9819e-01, 0.0000e+00],
        [4.6275e+02, 3.1367e+02, 8.2641e+02, 3.6995e+02, 4.9074e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([4, 6])
xywh: tensor([[ 320.3314,  483.1455,  321.3187,   93.3868],
        [1067.4604,  272.3054,  394.6723,   73.8983],
        [ 933.6955,  463.3033,  109.2948,   44.3400],
        [ 644.5802,  341.8118,  363.6620,   56.2847]], device='cuda:0')
xywhn: tensor([[0.2503, 0.6710, 0.2510, 0.1297],
        [0.8340, 0.3782, 0.3083, 0.1026],
        [0.7294, 0.6435, 0.0854, 0.0616],
        [0.5036, 0.4747, 0.2841, 0.0782]], device='cuda:0')
xyxy: tensor([[ 159.6720,  436.4521,  480.9907,  529.8389],
        [ 870.1243,  235.3562, 1264.7966,  309.2545],
        [ 879.0481,  441.1334,  988.3429,  485.4733],
        [ 462.7492,  313.6695,  826.4112,  369.9542]], device='cuda:0')
xyxyn: tensor([[0.1247, 0.6062, 0.3758, 0.7359],
        [0.6798, 0.3269, 0.9881, 0.4295],
        [0.6868, 0.6127, 0.7721, 0.6743],
        [0.3615, 0.4357, 0.6456, 0.5138]], device='cuda:0')

0: 384x640 3 Potholes, 8.2ms
Speed: 2.3ms preprocess, 8.2ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0.], device='cuda:0')
conf: tensor([0.8154, 0.7283, 0.6153], device='cuda:0')
data: tensor([[1.5211e+02, 4.4660e+02, 5.2160e+02, 5.5765e+02, 8.1537e-01, 0.0000e+00],
        [4.6017e+02, 3.2158e+02, 8.3364e+02, 3.8133e+02, 7.2833e-01, 0.0000e+00],
        [8.7115e+02, 2.3796e+02, 1.2800e+03, 3.1664e+02, 6.1529e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([3, 6])
xywh: tensor([[ 336.8574,  502.1282,  369.4883,  111.0488],
        [ 646.9053,  351.4533,  373.4791,   59.7535],
        [1075.5757,  277.2992,  408.8486,   78.6752]], device='cuda:0')
xywhn: tensor([[0.2632, 0.6974, 0.2887, 0.1542],
        [0.5054, 0.4881, 0.2918, 0.0830],
        [0.8403, 0.3851, 0.3194, 0.1093]], device='cuda:0')
xyxy: tensor([[ 152.1133,  446.6038,  521.6016,  557.6526],
        [ 460.1657,  321.5765,  833.6448,  381.3301],
        [ 871.1514,  237.9616, 1280.0000,  316.6368]], device='cuda:0')
xyxyn: tensor([[0.1188, 0.6203, 0.4075, 0.7745],
        [0.3595, 0.4466, 0.6513, 0.5296],
        [0.6806, 0.3305, 1.0000, 0.4398]], device='cuda:0')

0: 384x640 4 Potholes, 12.5ms
Speed: 2.0ms preprocess, 12.5ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.8636, 0.6807, 0.6533, 0.3130], device='cuda:0')
data: tensor([[4.5494e+02, 3.2194e+02, 8.3501e+02, 3.9014e+02, 8.6359e-01, 0.0000e+00],
        [1.3033e+02, 4.5477e+02, 5.1693e+02, 5.7052e+02, 6.8066e-01, 0.0000e+00],
        [8.7437e+02, 2.3919e+02, 1.2800e+03, 3.1953e+02, 6.5326e-01, 0.0000e+00],
        [9.0462e+02, 4.6432e+02, 1.0246e+03, 5.1953e+02, 3.1299e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([4, 6])
xywh: tensor([[ 644.9733,  356.0428,  380.0700,   68.1973],
        [ 323.6284,  512.6457,  386.6039,  115.7510],
        [1077.1858,  279.3600,  405.6285,   80.3441],
        [ 964.5977,  491.9268,  119.9453,   55.2053]], device='cuda:0')
xywhn: tensor([[0.5039, 0.4945, 0.2969, 0.0947],
        [0.2528, 0.7120, 0.3020, 0.1608],
        [0.8416, 0.3880, 0.3169, 0.1116],
        [0.7536, 0.6832, 0.0937, 0.0767]], device='cuda:0')
xyxy: tensor([[ 454.9383,  321.9442,  835.0083,  390.1414],
        [ 130.3264,  454.7702,  516.9303,  570.5212],
        [ 874.3715,  239.1879, 1280.0000,  319.5320],
        [ 904.6250,  464.3241, 1024.5703,  519.5294]], device='cuda:0')
xyxyn: tensor([[0.3554, 0.4471, 0.6524, 0.5419],
        [0.1018, 0.6316, 0.4039, 0.7924],
        [0.6831, 0.3322, 1.0000, 0.4438],
        [0.7067, 0.6449, 0.8004, 0.7216]], device='cuda:0')

0: 384x640 4 Potholes, 8.1ms
Speed: 2.2ms preprocess, 8.1ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.8239, 0.7525, 0.7240, 0.2581], device='cuda:0')
data: tensor([[1.2643e+02, 4.6838e+02, 5.1807e+02, 5.8724e+02, 8.2395e-01, 0.0000e+00],
        [8.8417e+02, 2.4207e+02, 1.2800e+03, 3.2301e+02, 7.5250e-01, 0.0000e+00],
        [4.5478e+02, 3.3043e+02, 8.4381e+02, 3.9495e+02, 7.2400e-01, 0.0000e+00],
        [3.2706e-01, 4.0530e+02, 6.9808e+01, 4.6487e+02, 2.5814e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([4, 6])
xywh: tensor([[ 322.2493,  527.8073,  391.6364,  118.8577],
        [1082.0864,  282.5389,  395.8271,   80.9360],
        [ 649.2949,  362.6884,  389.0370,   64.5176],
        [  35.0676,  435.0884,   69.4811,   59.5712]], device='cuda:0')
xywhn: tensor([[0.2518, 0.7331, 0.3060, 0.1651],
        [0.8454, 0.3924, 0.3092, 0.1124],
        [0.5073, 0.5037, 0.3039, 0.0896],
        [0.0274, 0.6043, 0.0543, 0.0827]], device='cuda:0')
xyxy: tensor([[1.2643e+02, 4.6838e+02, 5.1807e+02, 5.8724e+02],
        [8.8417e+02, 2.4207e+02, 1.2800e+03, 3.2301e+02],
        [4.5478e+02, 3.3043e+02, 8.4381e+02, 3.9495e+02],
        [3.2706e-01, 4.0530e+02, 6.9808e+01, 4.6487e+02]], device='cuda:0')
xyxyn: tensor([[9.8774e-02, 6.5053e-01, 4.0474e-01, 8.1561e-01],
        [6.9076e-01, 3.3621e-01, 1.0000e+00, 4.4862e-01],
        [3.5529e-01, 4.5893e-01, 6.5923e-01, 5.4854e-01],
        [2.5551e-04, 5.6292e-01, 5.4538e-02, 6.4566e-01]], device='cuda:0')

0: 384x640 3 Potholes, 9.4ms
Speed: 1.9ms preprocess, 9.4ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0.], device='cuda:0')
conf: tensor([0.8489, 0.7802, 0.6854], device='cuda:0')
data: tensor([[8.8938e+02, 2.4585e+02, 1.2800e+03, 3.3044e+02, 8.4891e-01, 0.0000e+00],
        [9.2743e+01, 4.8779e+02, 5.1701e+02, 6.1971e+02, 7.8019e-01, 0.0000e+00],
        [4.4597e+02, 3.3728e+02, 8.4344e+02, 4.0513e+02, 6.8545e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([3, 6])
xywh: tensor([[1084.6895,  288.1433,  390.6210,   84.5851],
        [ 304.8785,  553.7506,  424.2704,  131.9116],
        [ 644.7053,  371.2026,  397.4663,   67.8535]], device='cuda:0')
xywhn: tensor([[0.8474, 0.4002, 0.3052, 0.1175],
        [0.2382, 0.7691, 0.3315, 0.1832],
        [0.5037, 0.5156, 0.3105, 0.0942]], device='cuda:0')
xyxy: tensor([[ 889.3790,  245.8508, 1280.0000,  330.4359],
        [  92.7433,  487.7948,  517.0137,  619.7064],
        [ 445.9722,  337.2759,  843.4385,  405.1293]], device='cuda:0')
xyxyn: tensor([[0.6948, 0.3415, 1.0000, 0.4589],
        [0.0725, 0.6775, 0.4039, 0.8607],
        [0.3484, 0.4684, 0.6589, 0.5627]], device='cuda:0')

0: 384x640 3 Potholes, 9.1ms
Speed: 2.0ms preprocess, 9.1ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0.], device='cuda:0')
conf: tensor([0.8556, 0.7641, 0.6392], device='cuda:0')
data: tensor([[8.9182e+02, 2.4843e+02, 1.2800e+03, 3.3417e+02, 8.5560e-01, 0.0000e+00],
        [6.9399e+01, 4.9941e+02, 5.2192e+02, 6.3788e+02, 7.6414e-01, 0.0000e+00],
        [4.4044e+02, 3.4256e+02, 8.6980e+02, 4.1174e+02, 6.3916e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([3, 6])
xywh: tensor([[1085.9093,  291.3014,  388.1814,   85.7339],
        [ 295.6572,  568.6445,  452.5171,  138.4722],
        [ 655.1224,  377.1491,  429.3597,   69.1760]], device='cuda:0')
xywhn: tensor([[0.8484, 0.4046, 0.3033, 0.1191],
        [0.2310, 0.7898, 0.3535, 0.1923],
        [0.5118, 0.5238, 0.3354, 0.0961]], device='cuda:0')
xyxy: tensor([[ 891.8186,  248.4344, 1280.0000,  334.1684],
        [  69.3987,  499.4084,  521.9158,  637.8806],
        [ 440.4426,  342.5611,  869.8023,  411.7371]], device='cuda:0')
xyxyn: tensor([[0.6967, 0.3450, 1.0000, 0.4641],
        [0.0542, 0.6936, 0.4077, 0.8859],
        [0.3441, 0.4758, 0.6795, 0.5719]], device='cuda:0')

0: 384x640 4 Potholes, 9.5ms
Speed: 1.9ms preprocess, 9.5ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.9121, 0.8392, 0.7799, 0.3935], device='cuda:0')
data: tensor([[8.9571e+02, 2.5252e+02, 1.2800e+03, 3.3852e+02, 9.1211e-01, 0.0000e+00],
        [4.4249e+02, 3.5045e+02, 8.6160e+02, 4.2034e+02, 8.3916e-01, 0.0000e+00],
        [5.6817e+01, 5.0778e+02, 5.2024e+02, 6.6707e+02, 7.7989e-01, 0.0000e+00],
        [8.5558e+02, 4.5862e+02, 1.1272e+03, 5.9392e+02, 3.9354e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([4, 6])
xywh: tensor([[1087.8533,  295.5204,  384.2933,   86.0025],
        [ 652.0466,  385.3962,  419.1039,   69.8945],
        [ 288.5294,  587.4252,  463.4257,  159.2883],
        [ 991.3708,  526.2722,  271.5856,  135.3002]], device='cuda:0')
xywhn: tensor([[0.8499, 0.4104, 0.3002, 0.1194],
        [0.5094, 0.5353, 0.3274, 0.0971],
        [0.2254, 0.8159, 0.3621, 0.2212],
        [0.7745, 0.7309, 0.2122, 0.1879]], device='cuda:0')
xyxy: tensor([[ 895.7067,  252.5191, 1280.0000,  338.5216],
        [ 442.4946,  350.4489,  861.5985,  420.3434],
        [  56.8166,  507.7810,  520.2422,  667.0693],
        [ 855.5780,  458.6221, 1127.1636,  593.9222]], device='cuda:0')
xyxyn: tensor([[0.6998, 0.3507, 1.0000, 0.4702],
        [0.3457, 0.4867, 0.6731, 0.5838],
        [0.0444, 0.7053, 0.4064, 0.9265],
        [0.6684, 0.6370, 0.8806, 0.8249]], device='cuda:0')

0: 384x640 5 Potholes, 11.1ms
Speed: 2.0ms preprocess, 11.1ms inference, 7.6ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.9485, 0.8328, 0.7766, 0.4596, 0.2589], device='cuda:0')
data: tensor([[9.0324e+02, 2.5335e+02, 1.2800e+03, 3.4245e+02, 9.4852e-01, 0.0000e+00],
        [4.3773e+02, 3.5150e+02, 8.6842e+02, 4.3012e+02, 8.3276e-01, 0.0000e+00],
        [8.8470e+00, 5.1727e+02, 5.1914e+02, 7.2000e+02, 7.7665e-01, 0.0000e+00],
        [8.5605e+02, 4.6578e+02, 1.1276e+03, 6.1018e+02, 4.5961e-01, 0.0000e+00],
        [4.3761e+02, 3.5130e+02, 7.4681e+02, 4.3363e+02, 2.5893e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([5, 6])
xywh: tensor([[1091.6191,  297.8980,  376.7617,   89.0991],
        [ 653.0743,  390.8055,  430.6980,   78.6204],
        [ 263.9929,  618.6332,  510.2916,  202.7335],
        [ 991.8423,  537.9817,  271.5767,  144.3987],
        [ 592.2067,  392.4667,  309.1975,   82.3251]], device='cuda:0')
xywhn: tensor([[0.8528, 0.4137, 0.2943, 0.1237],
        [0.5102, 0.5428, 0.3365, 0.1092],
        [0.2062, 0.8592, 0.3987, 0.2816],
        [0.7749, 0.7472, 0.2122, 0.2006],
        [0.4627, 0.5451, 0.2416, 0.1143]], device='cuda:0')
xyxy: tensor([[ 903.2383,  253.3484, 1280.0000,  342.4475],
        [ 437.7254,  351.4954,  868.4233,  430.1157],
        [   8.8470,  517.2665,  519.1387,  720.0000],
        [ 856.0540,  465.7824, 1127.6306,  610.1810],
        [ 437.6079,  351.3041,  746.8054,  433.6292]], device='cuda:0')
xyxyn: tensor([[0.7057, 0.3519, 1.0000, 0.4756],
        [0.3420, 0.4882, 0.6785, 0.5974],
        [0.0069, 0.7184, 0.4056, 1.0000],
        [0.6688, 0.6469, 0.8810, 0.8475],
        [0.3419, 0.4879, 0.5834, 0.6023]], device='cuda:0')

0: 384x640 4 Potholes, 10.0ms
Speed: 2.0ms preprocess, 10.0ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.9457, 0.8230, 0.8181, 0.4886], device='cuda:0')
data: tensor([[9.0853e+02, 2.5567e+02, 1.2800e+03, 3.4511e+02, 9.4570e-01, 0.0000e+00],
        [4.3059e+02, 3.5821e+02, 8.7524e+02, 4.4806e+02, 8.2300e-01, 0.0000e+00],
        [5.3128e+00, 5.3668e+02, 5.2043e+02, 7.2000e+02, 8.1814e-01, 0.0000e+00],
        [8.8136e+02, 4.8189e+02, 1.1654e+03, 6.4796e+02, 4.8860e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([4, 6])
xywh: tensor([[1094.2661,  300.3890,  371.4678,   89.4446],
        [ 652.9155,  403.1388,  444.6565,   89.8512],
        [ 262.8719,  628.3395,  515.1183,  183.3210],
        [1023.3567,  564.9250,  283.9978,  166.0640]], device='cuda:0')
xywhn: tensor([[0.8549, 0.4172, 0.2902, 0.1242],
        [0.5101, 0.5599, 0.3474, 0.1248],
        [0.2054, 0.8727, 0.4024, 0.2546],
        [0.7995, 0.7846, 0.2219, 0.2306]], device='cuda:0')
xyxy: tensor([[ 908.5322,  255.6667, 1280.0000,  345.1113],
        [ 430.5873,  358.2132,  875.2438,  448.0644],
        [   5.3128,  536.6790,  520.4311,  720.0000],
        [ 881.3578,  481.8930, 1165.3556,  647.9570]], device='cuda:0')
xyxyn: tensor([[0.7098, 0.3551, 1.0000, 0.4793],
        [0.3364, 0.4975, 0.6838, 0.6223],
        [0.0042, 0.7454, 0.4066, 1.0000],
        [0.6886, 0.6693, 0.9104, 0.8999]], device='cuda:0')

0: 384x640 5 Potholes, 9.6ms
Speed: 1.9ms preprocess, 9.6ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.9249, 0.7338, 0.6567, 0.6189, 0.3030], device='cuda:0')
data: tensor([[9.1158e+02, 2.5661e+02, 1.2800e+03, 3.4998e+02, 9.2494e-01, 0.0000e+00],
        [4.2345e+02, 3.6157e+02, 8.8848e+02, 4.5326e+02, 7.3377e-01, 0.0000e+00],
        [3.3323e+00, 5.4414e+02, 5.1759e+02, 7.1985e+02, 6.5671e-01, 0.0000e+00],
        [8.8632e+02, 4.9469e+02, 1.1715e+03, 6.6069e+02, 6.1893e-01, 0.0000e+00],
        [2.0079e+02, 5.5332e+02, 5.1992e+02, 7.1613e+02, 3.0305e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([5, 6])
xywh: tensor([[1095.7881,  303.2952,  368.4239,   93.3661],
        [ 655.9644,  407.4167,  465.0331,   91.6873],
        [ 260.4623,  631.9967,  514.2599,  175.7063],
        [1028.9279,  577.6874,  285.2139,  166.0015],
        [ 360.3550,  634.7291,  319.1285,  162.8083]], device='cuda:0')
xywhn: tensor([[0.8561, 0.4212, 0.2878, 0.1297],
        [0.5125, 0.5659, 0.3633, 0.1273],
        [0.2035, 0.8778, 0.4018, 0.2440],
        [0.8038, 0.8023, 0.2228, 0.2306],
        [0.2815, 0.8816, 0.2493, 0.2261]], device='cuda:0')
xyxy: tensor([[ 911.5761,  256.6122, 1280.0000,  349.9783],
        [ 423.4479,  361.5730,  888.4810,  453.2603],
        [   3.3323,  544.1436,  517.5923,  719.8499],
        [ 886.3209,  494.6866, 1171.5348,  660.6881],
        [ 200.7908,  553.3249,  519.9193,  716.1332]], device='cuda:0')
xyxyn: tensor([[0.7122, 0.3564, 1.0000, 0.4861],
        [0.3308, 0.5022, 0.6941, 0.6295],
        [0.0026, 0.7558, 0.4044, 0.9998],
        [0.6924, 0.6871, 0.9153, 0.9176],
        [0.1569, 0.7685, 0.4062, 0.9946]], device='cuda:0')

0: 384x640 6 Potholes, 9.3ms
Speed: 2.1ms preprocess, 9.3ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.9309, 0.7462, 0.7306, 0.5736, 0.5408, 0.2688], device='cuda:0')
data: tensor([[9.1767e+02, 2.5817e+02, 1.2800e+03, 3.5540e+02, 9.3087e-01, 0.0000e+00],
        [4.3237e+02, 3.6794e+02, 8.9131e+02, 4.6262e+02, 7.4618e-01, 0.0000e+00],
        [1.9493e+02, 5.6585e+02, 5.0867e+02, 7.1935e+02, 7.3061e-01, 0.0000e+00],
        [1.2632e+00, 5.6208e+02, 5.0775e+02, 7.2000e+02, 5.7362e-01, 0.0000e+00],
        [1.0377e+03, 5.9645e+02, 1.1969e+03, 6.7089e+02, 5.4078e-01, 0.0000e+00],
        [1.0262e+03, 5.7148e+02, 1.1921e+03, 6.7935e+02, 2.6876e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([6, 6])
xywh: tensor([[1098.8357,  306.7857,  362.3287,   97.2239],
        [ 661.8397,  415.2846,  458.9427,   94.6802],
        [ 351.7971,  642.6038,  313.7413,  153.4995],
        [ 254.5068,  641.0414,  506.4873,  157.9172],
        [1117.2823,  633.6680,  159.1956,   74.4402],
        [1109.1206,  625.4142,  165.8960,  107.8669]], device='cuda:0')
xywhn: tensor([[0.8585, 0.4261, 0.2831, 0.1350],
        [0.5171, 0.5768, 0.3585, 0.1315],
        [0.2748, 0.8925, 0.2451, 0.2132],
        [0.1988, 0.8903, 0.3957, 0.2193],
        [0.8729, 0.8801, 0.1244, 0.1034],
        [0.8665, 0.8686, 0.1296, 0.1498]], device='cuda:0')
xyxy: tensor([[9.1767e+02, 2.5817e+02, 1.2800e+03, 3.5540e+02],
        [4.3237e+02, 3.6794e+02, 8.9131e+02, 4.6262e+02],
        [1.9493e+02, 5.6585e+02, 5.0867e+02, 7.1935e+02],
        [1.2632e+00, 5.6208e+02, 5.0775e+02, 7.2000e+02],
        [1.0377e+03, 5.9645e+02, 1.1969e+03, 6.7089e+02],
        [1.0262e+03, 5.7148e+02, 1.1921e+03, 6.7935e+02]], device='cuda:0')
xyxyn: tensor([[7.1693e-01, 3.5857e-01, 1.0000e+00, 4.9361e-01],
        [3.3779e-01, 5.1103e-01, 6.9634e-01, 6.4253e-01],
        [1.5229e-01, 7.8591e-01, 3.9740e-01, 9.9910e-01],
        [9.8686e-04, 7.8067e-01, 3.9668e-01, 1.0000e+00],
        [8.1069e-01, 8.2840e-01, 9.3506e-01, 9.3179e-01],
        [8.0170e-01, 7.9372e-01, 9.3130e-01, 9.4354e-01]], device='cuda:0')

0: 384x640 6 Potholes, 11.3ms
Speed: 2.0ms preprocess, 11.3ms inference, 1.9ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.8753, 0.7871, 0.4674, 0.4158, 0.3280, 0.2518], device='cuda:0')
data: tensor([[9.2280e+02, 2.5938e+02, 1.2800e+03, 3.6350e+02, 8.7534e-01, 0.0000e+00],
        [4.1676e+02, 3.8100e+02, 9.0590e+02, 4.8066e+02, 7.8708e-01, 0.0000e+00],
        [1.8445e+00, 5.9132e+02, 5.0731e+02, 7.2000e+02, 4.6742e-01, 0.0000e+00],
        [9.2243e+02, 5.2626e+02, 1.2432e+03, 7.2000e+02, 4.1576e-01, 0.0000e+00],
        [1.0662e+03, 6.3271e+02, 1.2276e+03, 7.2000e+02, 3.2796e-01, 0.0000e+00],
        [9.4747e+02, 5.7690e+02, 1.2433e+03, 7.2000e+02, 2.5179e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([6, 6])
xywh: tensor([[1101.3994,  311.4398,  357.2012,  104.1119],
        [ 661.3325,  430.8274,  489.1393,   99.6571],
        [ 254.5750,  655.6584,  505.4611,  128.6831],
        [1082.8240,  623.1317,  320.7949,  193.7366],
        [1146.8932,  676.3553,  161.3540,   87.2893],
        [1095.3861,  648.4512,  295.8372,  143.0975]], device='cuda:0')
xywhn: tensor([[0.8605, 0.4326, 0.2791, 0.1446],
        [0.5167, 0.5984, 0.3821, 0.1384],
        [0.1989, 0.9106, 0.3949, 0.1787],
        [0.8460, 0.8655, 0.2506, 0.2691],
        [0.8960, 0.9394, 0.1261, 0.1212],
        [0.8558, 0.9006, 0.2311, 0.1987]], device='cuda:0')
xyxy: tensor([[ 922.7988,  259.3838, 1280.0000,  363.4957],
        [ 416.7629,  380.9989,  905.9022,  480.6560],
        [   1.8445,  591.3169,  507.3055,  720.0000],
        [ 922.4265,  526.2634, 1243.2214,  720.0000],
        [1066.2162,  632.7107, 1227.5702,  720.0000],
        [ 947.4675,  576.9025, 1243.3047,  720.0000]], device='cuda:0')
xyxyn: tensor([[0.7209, 0.3603, 1.0000, 0.5049],
        [0.3256, 0.5292, 0.7077, 0.6676],
        [0.0014, 0.8213, 0.3963, 1.0000],
        [0.7206, 0.7309, 0.9713, 1.0000],
        [0.8330, 0.8788, 0.9590, 1.0000],
        [0.7402, 0.8013, 0.9713, 1.0000]], device='cuda:0')

0: 384x640 2 Potholes, 11.2ms
Speed: 2.1ms preprocess, 11.2ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0.], device='cuda:0')
conf: tensor([0.8601, 0.7192], device='cuda:0')
data: tensor([[9.2855e+02, 2.6071e+02, 1.2800e+03, 3.7091e+02, 8.6011e-01, 0.0000e+00],
        [4.1493e+02, 3.8650e+02, 9.0846e+02, 4.9227e+02, 7.1925e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([2, 6])
xywh: tensor([[1104.2742,  315.8092,  351.4517,  110.2054],
        [ 661.6935,  439.3840,  493.5273,  105.7722]], device='cuda:0')
xywhn: tensor([[0.8627, 0.4386, 0.2746, 0.1531],
        [0.5169, 0.6103, 0.3856, 0.1469]], device='cuda:0')
xyxy: tensor([[ 928.5483,  260.7065, 1280.0000,  370.9119],
        [ 414.9298,  386.4979,  908.4572,  492.2701]], device='cuda:0')
xyxyn: tensor([[0.7254, 0.3621, 1.0000, 0.5152],
        [0.3242, 0.5368, 0.7097, 0.6837]], device='cuda:0')

0: 384x640 4 Potholes, 11.9ms
Speed: 2.9ms preprocess, 11.9ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0., 0.], device='cuda:0')
conf: tensor([0.9095, 0.7529, 0.6177, 0.2878], device='cuda:0')
data: tensor([[9.3142e+02, 2.6237e+02, 1.2800e+03, 3.7519e+02, 9.0950e-01, 0.0000e+00],
        [4.2256e+02, 3.9618e+02, 8.0975e+02, 5.0460e+02, 7.5293e-01, 0.0000e+00],
        [4.2139e+02, 3.9452e+02, 9.8531e+02, 5.0257e+02, 6.1771e-01, 0.0000e+00],
        [0.0000e+00, 6.1246e+02, 5.2803e+02, 7.2000e+02, 2.8775e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([4, 6])
xywh: tensor([[1105.7076,  318.7790,  348.5847,  112.8167],
        [ 616.1569,  450.3857,  387.1849,  108.4203],
        [ 703.3512,  448.5450,  563.9248,  108.0543],
        [ 264.0145,  666.2302,  528.0289,  107.5395]], device='cuda:0')
xywhn: tensor([[0.8638, 0.4427, 0.2723, 0.1567],
        [0.4814, 0.6255, 0.3025, 0.1506],
        [0.5495, 0.6230, 0.4406, 0.1501],
        [0.2063, 0.9253, 0.4125, 0.1494]], device='cuda:0')
xyxy: tensor([[ 931.4153,  262.3706, 1280.0000,  375.1873],
        [ 422.5644,  396.1756,  809.7493,  504.5959],
        [ 421.3888,  394.5179,  985.3136,  502.5721],
        [   0.0000,  612.4605,  528.0289,  720.0000]], device='cuda:0')
xyxyn: tensor([[0.7277, 0.3644, 1.0000, 0.5211],
        [0.3301, 0.5502, 0.6326, 0.7008],
        [0.3292, 0.5479, 0.7698, 0.6980],
        [0.0000, 0.8506, 0.4125, 1.0000]], device='cuda:0')

0: 384x640 2 Potholes, 13.0ms
Speed: 2.4ms preprocess, 13.0ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0.], device='cuda:0')
conf: tensor([0.8379, 0.7900], device='cuda:0')
data: tensor([[9.4147e+02, 2.6309e+02, 1.2784e+03, 3.8311e+02, 8.3786e-01, 0.0000e+00],
        [4.1913e+02, 4.1110e+02, 9.3649e+02, 5.2873e+02, 7.9003e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([2, 6])
xywh: tensor([[1109.9333,  323.0991,  336.9241,  120.0150],
        [ 677.8079,  469.9170,  517.3574,  117.6306]], device='cuda:0')
xywhn: tensor([[0.8671, 0.4487, 0.2632, 0.1667],
        [0.5295, 0.6527, 0.4042, 0.1634]], device='cuda:0')
xyxy: tensor([[ 941.4713,  263.0916, 1278.3954,  383.1066],
        [ 419.1292,  411.1017,  936.4866,  528.7323]], device='cuda:0')
xyxyn: tensor([[0.7355, 0.3654, 0.9987, 0.5321],
        [0.3274, 0.5710, 0.7316, 0.7344]], device='cuda:0')

0: 384x640 3 Potholes, 10.8ms
Speed: 3.0ms preprocess, 10.8ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0.], device='cuda:0')
conf: tensor([0.8469, 0.8419, 0.7637], device='cuda:0')
data: tensor([[9.4546e+02, 2.6574e+02, 1.2793e+03, 3.8935e+02, 8.4695e-01, 0.0000e+00],
        [4.1856e+02, 4.1547e+02, 8.2459e+02, 5.3866e+02, 8.4195e-01, 0.0000e+00],
        [4.1553e+02, 4.2225e+02, 9.4781e+02, 5.3139e+02, 7.6369e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([3, 6])
xywh: tensor([[1112.3562,  327.5446,  333.7922,  123.6136],
        [ 621.5753,  477.0641,  406.0381,  123.1895],
        [ 681.6710,  476.8162,  532.2731,  109.1377]], device='cuda:0')
xywhn: tensor([[0.8690, 0.4549, 0.2608, 0.1717],
        [0.4856, 0.6626, 0.3172, 0.1711],
        [0.5326, 0.6622, 0.4158, 0.1516]], device='cuda:0')
xyxy: tensor([[ 945.4601,  265.7379, 1279.2523,  389.3514],
        [ 418.5562,  415.4694,  824.5944,  538.6588],
        [ 415.5344,  422.2473,  947.8075,  531.3850]], device='cuda:0')
xyxyn: tensor([[0.7386, 0.3691, 0.9994, 0.5408],
        [0.3270, 0.5770, 0.6442, 0.7481],
        [0.3246, 0.5865, 0.7405, 0.7380]], device='cuda:0')

0: 384x640 2 Potholes, 11.4ms
Speed: 1.9ms preprocess, 11.4ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0.], device='cuda:0')
conf: tensor([0.8506, 0.7892], device='cuda:0')
data: tensor([[9.5380e+02, 2.6786e+02, 1.2800e+03, 3.9224e+02, 8.5064e-01, 0.0000e+00],
        [4.0551e+02, 4.2558e+02, 9.5914e+02, 5.5070e+02, 7.8922e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([2, 6])
xywh: tensor([[1116.9003,  330.0491,  326.1941,  124.3850],
        [ 682.3281,  488.1402,  553.6288,  125.1136]], device='cuda:0')
xywhn: tensor([[0.8726, 0.4584, 0.2548, 0.1728],
        [0.5331, 0.6780, 0.4325, 0.1738]], device='cuda:0')
xyxy: tensor([[ 953.8032,  267.8566, 1279.9973,  392.2416],
        [ 405.5137,  425.5834,  959.1425,  550.6970]], device='cuda:0')
xyxyn: tensor([[0.7452, 0.3720, 1.0000, 0.5448],
        [0.3168, 0.5911, 0.7493, 0.7649]], device='cuda:0')

0: 384x640 3 Potholes, 11.1ms
Speed: 2.0ms preprocess, 11.1ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0.], device='cuda:0')
conf: tensor([0.8335, 0.7896, 0.4188], device='cuda:0')
data: tensor([[3.9495e+02, 4.2787e+02, 9.5851e+02, 5.8503e+02, 8.3345e-01, 0.0000e+00],
        [9.6127e+02, 2.6961e+02, 1.2800e+03, 3.9810e+02, 7.8963e-01, 0.0000e+00],
        [9.8494e+02, 6.3560e+02, 1.2800e+03, 7.2000e+02, 4.1881e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([3, 6])
xywh: tensor([[ 676.7313,  506.4480,  563.5538,  157.1621],
        [1120.6373,  333.8514,  318.7254,  128.4893],
        [1132.4717,  677.7977,  295.0567,   84.4047]], device='cuda:0')
xywhn: tensor([[0.5287, 0.7034, 0.4403, 0.2183],
        [0.8755, 0.4637, 0.2490, 0.1785],
        [0.8847, 0.9414, 0.2305, 0.1172]], device='cuda:0')
xyxy: tensor([[ 394.9543,  427.8669,  958.5082,  585.0291],
        [ 961.2746,  269.6068, 1280.0000,  398.0961],
        [ 984.9433,  635.5953, 1280.0000,  720.0000]], device='cuda:0')
xyxyn: tensor([[0.3086, 0.5943, 0.7488, 0.8125],
        [0.7510, 0.3745, 1.0000, 0.5529],
        [0.7695, 0.8828, 1.0000, 1.0000]], device='cuda:0')

0: 384x640 2 Potholes, 12.2ms
Speed: 2.1ms preprocess, 12.2ms inference, 2.1ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0.], device='cuda:0')
conf: tensor([0.7811, 0.7498], device='cuda:0')
data: tensor([[3.8530e+02, 4.4931e+02, 9.8204e+02, 6.1180e+02, 7.8113e-01, 0.0000e+00],
        [9.6873e+02, 2.7706e+02, 1.2800e+03, 4.1397e+02, 7.4981e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([2, 6])
xywh: tensor([[ 683.6718,  530.5585,  596.7417,  162.4924],
        [1124.3651,  345.5172,  311.2698,  136.9108]], device='cuda:0')
xywhn: tensor([[0.5341, 0.7369, 0.4662, 0.2257],
        [0.8784, 0.4799, 0.2432, 0.1902]], device='cuda:0')
xyxy: tensor([[ 385.3009,  449.3123,  982.0426,  611.8047],
        [ 968.7302,  277.0618, 1280.0000,  413.9725]], device='cuda:0')
xyxyn: tensor([[0.3010, 0.6240, 0.7672, 0.8497],
        [0.7568, 0.3848, 1.0000, 0.5750]], device='cuda:0')

0: 384x640 3 Potholes, 14.9ms
Speed: 1.9ms preprocess, 14.9ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0.], device='cuda:0')
conf: tensor([0.7975, 0.7108, 0.3112], device='cuda:0')
data: tensor([[3.8579e+02, 4.5637e+02, 1.0043e+03, 6.2350e+02, 7.9754e-01, 0.0000e+00],
        [9.7113e+02, 2.8393e+02, 1.2800e+03, 4.1158e+02, 7.1084e-01, 0.0000e+00],
        [3.8894e+02, 4.5438e+02, 1.2614e+03, 6.3576e+02, 3.1122e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([3, 6])
xywh: tensor([[ 695.0322,  539.9338,  618.4852,  167.1246],
        [1125.5658,  347.7543,  308.8684,  127.6536],
        [ 825.1891,  545.0664,  872.5042,  181.3772]], device='cuda:0')
xywhn: tensor([[0.5430, 0.7499, 0.4832, 0.2321],
        [0.8793, 0.4830, 0.2413, 0.1773],
        [0.6447, 0.7570, 0.6816, 0.2519]], device='cuda:0')
xyxy: tensor([[ 385.7896,  456.3715, 1004.2748,  623.4962],
        [ 971.1316,  283.9276, 1280.0000,  411.5811],
        [ 388.9370,  454.3778, 1261.4412,  635.7550]], device='cuda:0')
xyxyn: tensor([[0.3014, 0.6338, 0.7846, 0.8660],
        [0.7587, 0.3943, 1.0000, 0.5716],
        [0.3039, 0.6311, 0.9855, 0.8830]], device='cuda:0')

0: 384x640 2 Potholes, 12.1ms
Speed: 2.0ms preprocess, 12.1ms inference, 1.9ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0.], device='cuda:0')
conf: tensor([0.8132, 0.5599], device='cuda:0')
data: tensor([[3.8115e+02, 4.6375e+02, 1.0255e+03, 6.4844e+02, 8.1323e-01, 0.0000e+00],
        [9.7977e+02, 2.8416e+02, 1.2800e+03, 4.2511e+02, 5.5988e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([2, 6])
xywh: tensor([[ 703.3003,  556.0950,  644.3010,  184.6836],
        [1129.8872,  354.6349,  300.2257,  140.9457]], device='cuda:0')
xywhn: tensor([[0.5495, 0.7724, 0.5034, 0.2565],
        [0.8827, 0.4925, 0.2346, 0.1958]], device='cuda:0')
xyxy: tensor([[ 381.1497,  463.7531, 1025.4508,  648.4368],
        [ 979.7743,  284.1620, 1280.0000,  425.1077]], device='cuda:0')
xyxyn: tensor([[0.2978, 0.6441, 0.8011, 0.9006],
        [0.7654, 0.3947, 1.0000, 0.5904]], device='cuda:0')

0: 384x640 2 Potholes, 10.1ms
Speed: 2.0ms preprocess, 10.1ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0.], device='cuda:0')
conf: tensor([0.8355, 0.6010], device='cuda:0')
data: tensor([[3.7895e+02, 4.9051e+02, 1.0914e+03, 6.8026e+02, 8.3553e-01, 0.0000e+00],
        [9.8373e+02, 2.9161e+02, 1.2800e+03, 4.4768e+02, 6.0103e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([2, 6])
xywh: tensor([[ 735.1774,  585.3843,  712.4471,  189.7429],
        [1131.8630,  369.6458,  296.2740,  156.0685]], device='cuda:0')
xywhn: tensor([[0.5744, 0.8130, 0.5566, 0.2635],
        [0.8843, 0.5134, 0.2315, 0.2168]], device='cuda:0')
xyxy: tensor([[ 378.9539,  490.5128, 1091.4010,  680.2557],
        [ 983.7260,  291.6116, 1280.0000,  447.6801]], device='cuda:0')
xyxyn: tensor([[0.2961, 0.6813, 0.8527, 0.9448],
        [0.7685, 0.4050, 1.0000, 0.6218]], device='cuda:0')

0: 384x640 2 Potholes, 11.6ms
Speed: 2.8ms preprocess, 11.6ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0.], device='cuda:0')
conf: tensor([0.8784, 0.4288], device='cuda:0')
data: tensor([[3.7783e+02, 4.9861e+02, 1.0865e+03, 7.0463e+02, 8.7840e-01, 0.0000e+00],
        [9.9166e+02, 2.9288e+02, 1.2800e+03, 4.3029e+02, 4.2877e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([2, 6])
xywh: tensor([[ 732.1638,  601.6189,  708.6769,  206.0212],
        [1135.8311,  361.5848,  288.3378,  137.4017]], device='cuda:0')
xywhn: tensor([[0.5720, 0.8356, 0.5537, 0.2861],
        [0.8874, 0.5022, 0.2253, 0.1908]], device='cuda:0')
xyxy: tensor([[ 377.8253,  498.6083, 1086.5022,  704.6295],
        [ 991.6622,  292.8839, 1280.0000,  430.2856]], device='cuda:0')
xyxyn: tensor([[0.2952, 0.6925, 0.8488, 0.9787],
        [0.7747, 0.4068, 1.0000, 0.5976]], device='cuda:0')

0: 384x640 2 Potholes, 9.1ms
Speed: 1.9ms preprocess, 9.1ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0.], device='cuda:0')
conf: tensor([0.8608, 0.5036], device='cuda:0')
data: tensor([[3.6722e+02, 5.1576e+02, 1.1095e+03, 7.1914e+02, 8.6075e-01, 0.0000e+00],
        [9.9370e+02, 2.9469e+02, 1.2800e+03, 4.3097e+02, 5.0358e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([2, 6])
xywh: tensor([[ 738.3818,  617.4501,  742.3286,  203.3772],
        [1136.8514,  362.8313,  286.2971,  136.2851]], device='cuda:0')
xywhn: tensor([[0.5769, 0.8576, 0.5799, 0.2825],
        [0.8882, 0.5039, 0.2237, 0.1893]], device='cuda:0')
xyxy: tensor([[ 367.2175,  515.7615, 1109.5461,  719.1387],
        [ 993.7029,  294.6887, 1280.0000,  430.9738]], device='cuda:0')
xyxyn: tensor([[0.2869, 0.7163, 0.8668, 0.9988],
        [0.7763, 0.4093, 1.0000, 0.5986]], device='cuda:0')

0: 384x640 2 Potholes, 9.7ms
Speed: 1.9ms preprocess, 9.7ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0.], device='cuda:0')
conf: tensor([0.9021, 0.3444], device='cuda:0')
data: tensor([[3.5267e+02, 5.3946e+02, 1.1814e+03, 7.2000e+02, 9.0212e-01, 0.0000e+00],
        [1.0009e+03, 2.9880e+02, 1.2800e+03, 4.3587e+02, 3.4435e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([2, 6])
xywh: tensor([[ 767.0342,  629.7283,  828.7279,  180.5433],
        [1140.4617,  367.3356,  279.0765,  137.0659]], device='cuda:0')
xywhn: tensor([[0.5992, 0.8746, 0.6474, 0.2508],
        [0.8910, 0.5102, 0.2180, 0.1904]], device='cuda:0')
xyxy: tensor([[ 352.6703,  539.4567, 1181.3982,  720.0000],
        [1000.9235,  298.8026, 1280.0000,  435.8685]], device='cuda:0')
xyxyn: tensor([[0.2755, 0.7492, 0.9230, 1.0000],
        [0.7820, 0.4150, 1.0000, 0.6054]], device='cuda:0')

0: 384x640 2 Potholes, 10.5ms
Speed: 2.1ms preprocess, 10.5ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0.], device='cuda:0')
conf: tensor([0.8667, 0.2833], device='cuda:0')
data: tensor([[3.5172e+02, 5.4953e+02, 1.2137e+03, 7.2000e+02, 8.6669e-01, 0.0000e+00],
        [1.0091e+03, 3.0024e+02, 1.2800e+03, 4.4737e+02, 2.8331e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([2, 6])
xywh: tensor([[ 782.6891,  634.7669,  861.9381,  170.4662],
        [1144.5381,  373.8054,  270.9240,  147.1229]], device='cuda:0')
xywhn: tensor([[0.6115, 0.8816, 0.6734, 0.2368],
        [0.8942, 0.5192, 0.2117, 0.2043]], device='cuda:0')
xyxy: tensor([[ 351.7201,  549.5338, 1213.6582,  720.0000],
        [1009.0760,  300.2439, 1280.0000,  447.3668]], device='cuda:0')
xyxyn: tensor([[0.2748, 0.7632, 0.9482, 1.0000],
        [0.7883, 0.4170, 1.0000, 0.6213]], device='cuda:0')

0: 384x640 3 Potholes, 9.9ms
Speed: 1.8ms preprocess, 9.9ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0.], device='cuda:0')
conf: tensor([0.8032, 0.5536, 0.4118], device='cuda:0')
data: tensor([[3.2435e+02, 5.5960e+02, 1.2419e+03, 7.2000e+02, 8.0317e-01, 0.0000e+00],
        [3.2963e+02, 5.6926e+02, 8.8071e+02, 7.2000e+02, 5.5356e-01, 0.0000e+00],
        [8.6632e+02, 4.3445e+02, 1.0451e+03, 4.9270e+02, 4.1179e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([3, 6])
xywh: tensor([[783.1228, 639.7986, 917.5500, 160.4027],
        [605.1677, 644.6276, 551.0847, 150.7448],
        [955.6893, 463.5735, 178.7378,  58.2538]], device='cuda:0')
xywhn: tensor([[0.6118, 0.8886, 0.7168, 0.2228],
        [0.4728, 0.8953, 0.4305, 0.2094],
        [0.7466, 0.6439, 0.1396, 0.0809]], device='cuda:0')
xyxy: tensor([[ 324.3478,  559.5973, 1241.8978,  720.0000],
        [ 329.6254,  569.2552,  880.7101,  720.0000],
        [ 866.3204,  434.4467, 1045.0582,  492.7004]], device='cuda:0')
xyxyn: tensor([[0.2534, 0.7772, 0.9702, 1.0000],
        [0.2575, 0.7906, 0.6881, 1.0000],
        [0.6768, 0.6034, 0.8165, 0.6843]], device='cuda:0')

0: 384x640 3 Potholes, 11.2ms
Speed: 2.2ms preprocess, 11.2ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0.], device='cuda:0')
conf: tensor([0.7651, 0.6714, 0.3602], device='cuda:0')
data: tensor([[3.3006e+02, 5.7878e+02, 1.2778e+03, 7.2000e+02, 7.6507e-01, 0.0000e+00],
        [3.4096e+02, 5.8673e+02, 8.8203e+02, 7.2000e+02, 6.7144e-01, 0.0000e+00],
        [1.0252e+03, 3.0889e+02, 1.2800e+03, 4.5743e+02, 3.6022e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([3, 6])
xywh: tensor([[ 803.9213,  649.3907,  947.7313,  141.2186],
        [ 611.4957,  653.3672,  541.0747,  133.2656],
        [1152.5951,  383.1578,  254.8098,  148.5364]], device='cuda:0')
xywhn: tensor([[0.6281, 0.9019, 0.7404, 0.1961],
        [0.4777, 0.9075, 0.4227, 0.1851],
        [0.9005, 0.5322, 0.1991, 0.2063]], device='cuda:0')
xyxy: tensor([[ 330.0557,  578.7814, 1277.7870,  720.0000],
        [ 340.9583,  586.7344,  882.0330,  720.0000],
        [1025.1902,  308.8896, 1280.0000,  457.4260]], device='cuda:0')
xyxyn: tensor([[0.2579, 0.8039, 0.9983, 1.0000],
        [0.2664, 0.8149, 0.6891, 1.0000],
        [0.8009, 0.4290, 1.0000, 0.6353]], device='cuda:0')

0: 384x640 3 Potholes, 12.3ms
Speed: 2.0ms preprocess, 12.3ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0.], device='cuda:0')
conf: tensor([0.6804, 0.6285, 0.5406], device='cuda:0')
data: tensor([[3.4886e+02, 6.1269e+02, 1.2800e+03, 7.2000e+02, 6.8036e-01, 0.0000e+00],
        [3.6853e+02, 6.2649e+02, 9.4445e+02, 7.2000e+02, 6.2849e-01, 0.0000e+00],
        [1.0418e+03, 3.1557e+02, 1.2800e+03, 4.7416e+02, 5.4056e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([3, 6])
xywh: tensor([[ 814.4316,  666.3470,  931.1367,  107.3058],
        [ 656.4912,  673.2445,  575.9182,   93.5110],
        [1160.9172,  394.8652,  238.1656,  158.5830]], device='cuda:0')
xywhn: tensor([[0.6363, 0.9255, 0.7275, 0.1490],
        [0.5129, 0.9351, 0.4499, 0.1299],
        [0.9070, 0.5484, 0.1861, 0.2203]], device='cuda:0')
xyxy: tensor([[ 348.8633,  612.6942, 1280.0000,  720.0000],
        [ 368.5321,  626.4890,  944.4503,  720.0000],
        [1041.8344,  315.5737, 1280.0000,  474.1567]], device='cuda:0')
xyxyn: tensor([[0.2725, 0.8510, 1.0000, 1.0000],
        [0.2879, 0.8701, 0.7379, 1.0000],
        [0.8139, 0.4383, 1.0000, 0.6586]], device='cuda:0')

0: 384x640 3 Potholes, 12.3ms
Speed: 2.0ms preprocess, 12.3ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0.], device='cuda:0')
conf: tensor([0.4836, 0.4432, 0.4021], device='cuda:0')
data: tensor([[3.4283e+02, 6.1657e+02, 1.2755e+03, 7.2000e+02, 4.8362e-01, 0.0000e+00],
        [3.7585e+02, 6.3674e+02, 9.3773e+02, 7.2000e+02, 4.4317e-01, 0.0000e+00],
        [1.0444e+03, 3.1727e+02, 1.2800e+03, 4.7873e+02, 4.0214e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([3, 6])
xywh: tensor([[ 809.1753,  668.2838,  932.6982,  103.4324],
        [ 656.7890,  678.3715,  561.8763,   83.2570],
        [1162.1942,  397.9982,  235.6116,  161.4646]], device='cuda:0')
xywhn: tensor([[0.6322, 0.9282, 0.7287, 0.1437],
        [0.5131, 0.9422, 0.4390, 0.1156],
        [0.9080, 0.5528, 0.1841, 0.2243]], device='cuda:0')
xyxy: tensor([[ 342.8261,  616.5676, 1275.5244,  720.0000],
        [ 375.8508,  636.7430,  937.7272,  720.0000],
        [1044.3884,  317.2659, 1280.0000,  478.7305]], device='cuda:0')
xyxyn: tensor([[0.2678, 0.8563, 0.9965, 1.0000],
        [0.2936, 0.8844, 0.7326, 1.0000],
        [0.8159, 0.4406, 1.0000, 0.6649]], device='cuda:0')

0: 384x640 (no detections), 10.2ms
Speed: 3.3ms preprocess, 10.2ms inference, 0.8ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([], device='cuda:0')
conf: tensor([], device='cuda:0')
data: tensor([], device='cuda:0', size=(0, 6))
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([0, 6])
xywh: tensor([], device='cuda:0', size=(0, 4))
xywhn: tensor([], device='cuda:0', size=(0, 4))
xyxy: tensor([], device='cuda:0', size=(0, 4))
xyxyn: tensor([], device='cuda:0', size=(0, 4))

0: 384x640 2 Potholes, 13.1ms
Speed: 5.0ms preprocess, 13.1ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0.], device='cuda:0')
conf: tensor([0.5819, 0.4740], device='cuda:0')
data: tensor([[1.0680e+03, 3.2536e+02, 1.2800e+03, 4.9243e+02, 5.8188e-01, 0.0000e+00],
        [9.6845e+02, 6.6159e+02, 1.2454e+03, 7.2000e+02, 4.7398e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([2, 6])
xywh: tensor([[1174.0210,  408.8918,  211.9580,  167.0682],
        [1106.9149,  690.7931,  276.9268,   58.4138]], device='cuda:0')
xywhn: tensor([[0.9172, 0.5679, 0.1656, 0.2320],
        [0.8648, 0.9594, 0.2163, 0.0811]], device='cuda:0')
xyxy: tensor([[1068.0420,  325.3577, 1280.0000,  492.4259],
        [ 968.4515,  661.5862, 1245.3783,  720.0000]], device='cuda:0')
xyxyn: tensor([[0.8344, 0.4519, 1.0000, 0.6839],
        [0.7566, 0.9189, 0.9730, 1.0000]], device='cuda:0')

0: 384x640 2 Potholes, 8.9ms
Speed: 3.3ms preprocess, 8.9ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0.], device='cuda:0')
conf: tensor([0.4070, 0.3368], device='cuda:0')
data: tensor([[8.9377e+02, 5.0765e+02, 1.1789e+03, 6.0668e+02, 4.0701e-01, 0.0000e+00],
        [1.0740e+03, 3.2766e+02, 1.2800e+03, 5.0055e+02, 3.3681e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([2, 6])
xywh: tensor([[1036.3160,  557.1621,  285.0823,   99.0325],
        [1177.0150,  414.1035,  205.9700,  172.8923]], device='cuda:0')
xywhn: tensor([[0.8096, 0.7738, 0.2227, 0.1375],
        [0.9195, 0.5751, 0.1609, 0.2401]], device='cuda:0')
xyxy: tensor([[ 893.7749,  507.6459, 1178.8572,  606.6783],
        [1074.0300,  327.6573, 1280.0000,  500.5496]], device='cuda:0')
xyxyn: tensor([[0.6983, 0.7051, 0.9210, 0.8426],
        [0.8391, 0.4551, 1.0000, 0.6952]], device='cuda:0')

0: 384x640 2 Potholes, 10.9ms
Speed: 2.0ms preprocess, 10.9ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0.], device='cuda:0')
conf: tensor([0.5035, 0.3142], device='cuda:0')
data: tensor([[8.9880e+02, 5.1841e+02, 1.2066e+03, 6.2807e+02, 5.0346e-01, 0.0000e+00],
        [1.0784e+03, 3.3164e+02, 1.2797e+03, 5.1088e+02, 3.1420e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([2, 6])
xywh: tensor([[1052.7091,  573.2410,  307.8196,  109.6611],
        [1179.0735,  421.2609,  201.3203,  179.2375]], device='cuda:0')
xywhn: tensor([[0.8224, 0.7962, 0.2405, 0.1523],
        [0.9212, 0.5851, 0.1573, 0.2489]], device='cuda:0')
xyxy: tensor([[ 898.7993,  518.4104, 1206.6189,  628.0715],
        [1078.4133,  331.6422, 1279.7336,  510.8797]], device='cuda:0')
xyxyn: tensor([[0.7022, 0.7200, 0.9427, 0.8723],
        [0.8425, 0.4606, 0.9998, 0.7096]], device='cuda:0')

0: 384x640 3 Potholes, 9.6ms
Speed: 2.0ms preprocess, 9.6ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0.], device='cuda:0')
conf: tensor([0.5429, 0.3606, 0.3238], device='cuda:0')
data: tensor([[1.1055e+03, 3.4084e+02, 1.2798e+03, 5.2656e+02, 5.4291e-01, 0.0000e+00],
        [9.3389e+02, 5.4420e+02, 1.2581e+03, 6.6641e+02, 3.6056e-01, 0.0000e+00],
        [1.4769e+01, 5.2107e+02, 1.2770e+03, 7.2000e+02, 3.2379e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([3, 6])
xywh: tensor([[1192.6226,  433.7001,  174.2915,  185.7175],
        [1096.0162,  605.3046,  324.2454,  122.2029],
        [ 645.9080,  620.5340, 1262.2783,  198.9320]], device='cuda:0')
xywhn: tensor([[0.9317, 0.6024, 0.1362, 0.2579],
        [0.8563, 0.8407, 0.2533, 0.1697],
        [0.5046, 0.8619, 0.9862, 0.2763]], device='cuda:0')
xyxy: tensor([[1105.4768,  340.8414, 1279.7683,  526.5589],
        [ 933.8936,  544.2031, 1258.1389,  666.4060],
        [  14.7688,  521.0680, 1277.0471,  720.0000]], device='cuda:0')
xyxyn: tensor([[0.8637, 0.4734, 0.9998, 0.7313],
        [0.7296, 0.7558, 0.9829, 0.9256],
        [0.0115, 0.7237, 0.9977, 1.0000]], device='cuda:0')

0: 384x640 1 Pothole, 10.2ms
Speed: 6.9ms preprocess, 10.2ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0.], device='cuda:0')
conf: tensor([0.5546], device='cuda:0')
data: tensor([[1.1134e+03, 3.4970e+02, 1.2799e+03, 5.2553e+02, 5.5465e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([1, 6])
xywh: tensor([[1196.6364,  437.6138,  166.4729,  175.8275]], device='cuda:0')
xywhn: tensor([[0.9349, 0.6078, 0.1301, 0.2442]], device='cuda:0')
xyxy: tensor([[1113.3999,  349.7000, 1279.8728,  525.5275]], device='cuda:0')
xyxyn: tensor([[0.8698, 0.4857, 0.9999, 0.7299]], device='cuda:0')

0: 384x640 3 Potholes, 8.5ms
Speed: 1.9ms preprocess, 8.5ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0., 0.], device='cuda:0')
conf: tensor([0.4422, 0.3564, 0.2943], device='cuda:0')
data: tensor([[1.1171e+03, 3.5020e+02, 1.2800e+03, 5.3076e+02, 4.4223e-01, 0.0000e+00],
        [1.4323e+01, 1.5416e+02, 1.2771e+03, 7.2000e+02, 3.5640e-01, 0.0000e+00],
        [2.1420e+02, 4.7688e+02, 3.8775e+02, 5.1930e+02, 2.9430e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([3, 6])
xywh: tensor([[1198.5098,  440.4781,  162.8813,  180.5615],
        [ 645.6907,  437.0786, 1262.7363,  565.8427],
        [ 300.9714,  498.0928,  173.5479,   42.4193]], device='cuda:0')
xywhn: tensor([[0.9363, 0.6118, 0.1273, 0.2508],
        [0.5044, 0.6071, 0.9865, 0.7859],
        [0.2351, 0.6918, 0.1356, 0.0589]], device='cuda:0')
xyxy: tensor([[1117.0691,  350.1973, 1279.9504,  530.7588],
        [  14.3225,  154.1573, 1277.0588,  720.0000],
        [ 214.1974,  476.8831,  387.7453,  519.3024]], device='cuda:0')
xyxyn: tensor([[0.8727, 0.4864, 1.0000, 0.7372],
        [0.0112, 0.2141, 0.9977, 1.0000],
        [0.1673, 0.6623, 0.3029, 0.7213]], device='cuda:0')

0: 384x640 2 Potholes, 10.1ms
Speed: 2.0ms preprocess, 10.1ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0.], device='cuda:0')
conf: tensor([0.3166, 0.3073], device='cuda:0')
data: tensor([[9.9465e+02, 5.9532e+02, 1.2781e+03, 7.2000e+02, 3.1663e-01, 0.0000e+00],
        [1.1281e+03, 3.5469e+02, 1.2800e+03, 5.3969e+02, 3.0728e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([2, 6])
xywh: tensor([[1136.3503,  657.6577,  283.4033,  124.6845],
        [1204.0542,  447.1915,  151.8916,  185.0021]], device='cuda:0')
xywhn: tensor([[0.8878, 0.9134, 0.2214, 0.1732],
        [0.9407, 0.6211, 0.1187, 0.2569]], device='cuda:0')
xyxy: tensor([[ 994.6487,  595.3155, 1278.0520,  720.0000],
        [1128.1084,  354.6904, 1280.0000,  539.6925]], device='cuda:0')
xyxyn: tensor([[0.7771, 0.8268, 0.9985, 1.0000],
        [0.8813, 0.4926, 1.0000, 0.7496]], device='cuda:0')

0: 384x640 1 Pothole, 10.1ms
Speed: 3.0ms preprocess, 10.1ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0.], device='cuda:0')
conf: tensor([0.6305], device='cuda:0')
data: tensor([[176.3625, 508.2316, 386.3248, 566.1827,   0.6305,   0.0000]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([1, 6])
xywh: tensor([[281.3436, 537.2072, 209.9623,  57.9512]], device='cuda:0')
xywhn: tensor([[0.2198, 0.7461, 0.1640, 0.0805]], device='cuda:0')
xyxy: tensor([[176.3625, 508.2316, 386.3248, 566.1827]], device='cuda:0')
xyxyn: tensor([[0.1378, 0.7059, 0.3018, 0.7864]], device='cuda:0')

0: 384x640 2 Potholes, 9.1ms
Speed: 1.9ms preprocess, 9.1ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0.], device='cuda:0')
conf: tensor([0.6676, 0.5309], device='cuda:0')
data: tensor([[1.6788e+02, 5.1930e+02, 3.8275e+02, 5.8180e+02, 6.6760e-01, 0.0000e+00],
        [1.1596e+03, 3.6056e+02, 1.2794e+03, 5.1466e+02, 5.3094e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([2, 6])
xywh: tensor([[ 275.3136,  550.5521,  214.8630,   62.5056],
        [1219.4696,  437.6071,  119.8276,  154.1014]], device='cuda:0')
xywhn: tensor([[0.2151, 0.7647, 0.1679, 0.0868],
        [0.9527, 0.6078, 0.0936, 0.2140]], device='cuda:0')
xyxy: tensor([[ 167.8821,  519.2993,  382.7451,  581.8049],
        [1159.5558,  360.5563, 1279.3834,  514.6578]], device='cuda:0')
xyxyn: tensor([[0.1312, 0.7212, 0.2990, 0.8081],
        [0.9059, 0.5008, 0.9995, 0.7148]], device='cuda:0')

0: 384x640 2 Potholes, 10.5ms
Speed: 1.9ms preprocess, 10.5ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0.], device='cuda:0')
conf: tensor([0.7492, 0.5787], device='cuda:0')
data: tensor([[1.6171e+02, 5.3085e+02, 3.7831e+02, 6.0162e+02, 7.4920e-01, 0.0000e+00],
        [1.1738e+03, 3.6316e+02, 1.2800e+03, 5.0957e+02, 5.7871e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([2, 6])
xywh: tensor([[ 270.0094,  566.2359,  216.5927,   70.7688],
        [1226.9036,  436.3638,  106.1548,  146.4138]], device='cuda:0')
xywhn: tensor([[0.2109, 0.7864, 0.1692, 0.0983],
        [0.9585, 0.6061, 0.0829, 0.2034]], device='cuda:0')
xyxy: tensor([[ 161.7130,  530.8515,  378.3058,  601.6203],
        [1173.8262,  363.1569, 1279.9810,  509.5707]], device='cuda:0')
xyxyn: tensor([[0.1263, 0.7373, 0.2956, 0.8356],
        [0.9171, 0.5044, 1.0000, 0.7077]], device='cuda:0')

0: 384x640 2 Potholes, 8.0ms
Speed: 2.1ms preprocess, 8.0ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)
Detections: ultralytics.engine.results.Boxes object with attributes:

cls: tensor([0., 0.], device='cuda:0')
conf: tensor([0.5671, 0.3248], device='cuda:0')
data: tensor([[9.1279e+01, 5.5944e+02, 3.7518e+02, 6.4268e+02, 5.6706e-01, 0.0000e+00],
        [1.1897e+03, 3.8094e+02, 1.2800e+03, 5.2812e+02, 3.2481e-01, 0.0000e+00]], device='cuda:0')
id: None
is_track: False
orig_shape: (720, 1280)
shape: torch.Size([2, 6])
xywh: tensor([[ 233.2314,  601.0612,  283.9048,   83.2445],
        [1234.8444,  454.5284,   90.2473,  147.1837]], device='cuda:0')
xywhn: tensor([[0.1822, 0.8348, 0.2218, 0.1156],
        [0.9647, 0.6313, 0.0705, 0.2044]], device='cuda:0')
xyxy: tensor([[  91.2790,  559.4390,  375.1837,  642.6835],
        [1189.7207,  380.9366, 1279.9680,  528.1203]], device='cuda:0')
xyxyn: tensor([[0.0713, 0.7770, 0.2931, 0.8926],
        [0.9295, 0.5291, 1.0000, 0.7335]], device='cuda:0')
Output video exists: True
Output video size: 27223070 bytes

```

```
<IPython.core.display.Video object>
```

```python
import cv2
import numpy as np
from collections import deque
from ultralytics import YOLO
import matplotlib.pyplot as plt
from IPython.display import Video

# Define paths for input and output videos
video_path = '/content/drive/MyDrive/Pothole_Segmentation_YOLOv8-1/sample_video.mp4'
output_video_path = '/content/drive/MyDrive/road_damage_assessment1.mp4'

# Load the trained model
best_model = YOLO('/content/drive/MyDrive/runs/detect/train2/weights/best.pt')

# Define font and colors for annotation
font = cv2.FONT_HERSHEY_SIMPLEX
font_scale = 1
text_position = (40, 80)
font_color = (255, 255, 255)    # White text
background_color = (255, 0, 0)  # Red background for text

# Initialize deque for averaging damage percentage
damage_deque = deque(maxlen=10)

# Initialize lists to store test metrics
num_detections = []
average_confidences = []

# Open the video
cap = cv2.VideoCapture(video_path)
width, height = int(cap.get(3)), int(cap.get(4))

# Define the codec and VideoWriter object for .mp4 output
fourcc = cv2.VideoWriter_fourcc(*'mp4v')
out = cv2.VideoWriter(output_video_path, fourcc, 20.0, (width, height))

# Process video frames
while cap.isOpened():
    ret, frame = cap.read()
    if not ret:
        break

    # Perform detection on the frame
    results = best_model.predict(source=frame, imgsz=640, conf=0.25)

    # Process and annotate the frame with bounding boxes
    processed_frame = results[0].plot()

    # Calculate the damage percentage based on mask areas
    percentage_damage = 0
    if results[0].masks is not None:
        total_area = 0
        masks = results[0].masks.data.cpu().numpy()
        image_area = frame.shape[0] * frame.shape[1]  # total number of pixels in the image
        for mask in masks:
            binary_mask = (mask > 0).astype(np.uint8) * 255
            contours, _ = cv2.findContours(binary_mask, cv2.RETR_TREE, cv2.CHAIN_APPROX_SIMPLE)
            for contour in contours:
                total_area += cv2.contourArea(contour)

        percentage_damage = (total_area / image_area) * 100

    # Update deque and calculate smoothed damage percentage
    damage_deque.append(percentage_damage)
    smoothed_percentage_damage = sum(damage_deque) / len(damage_deque)

    # Draw damage percentage text on the processed frame
    cv2.line(processed_frame, (text_position[0], text_position[1] - 10),
             (text_position[0] + 350, text_position[1] - 10), background_color, 40)
    cv2.putText(processed_frame, f'Road Damage: {smoothed_percentage_damage:.2f}%',
                text_position, font, font_scale, font_color, 2, cv2.LINE_AA)

    # Collect test metrics: number of detections and average confidence
    num_detections.append(len(results[0].boxes))
    if len(results[0].boxes) > 0:
        avg_conf = results[0].boxes.conf.mean().item()
        average_confidences.append(avg_conf)
    else:
        average_confidences.append(0)

    # Write the processed frame to the output video
    out.write(processed_frame)

cap.release()
out.release()

# Verify if the output video was created and its size
import os
print(f"Output video exists: {os.path.exists(output_video_path)}")
print(f"Output video size: {os.path.getsize(output_video_path)} bytes")

# Display the processed video within the notebook
Video(output_video_path, embed=True, width=960)

# Plot metrics for test data
plt.figure(figsize=(18, 6))

# Plot Number of Detections
plt.subplot(1, 2, 1)
plt.plot(num_detections, label='Number of Detections')
plt.xlabel('Frame')
plt.ylabel('Count')
plt.title('Number of Detections per Frame (Test)')
plt.legend()

# Plot Average Confidence
plt.subplot(1, 2, 2)
plt.plot(average_confidences, label='Average Confidence')
plt.xlabel('Frame')
plt.ylabel('Confidence')
plt.title('Average Confidence per Frame (Test)')
plt.legend()

plt.tight_layout()
plt.show()

```

```

0: 384x640 8 Potholes, 12.4ms
Speed: 2.0ms preprocess, 12.4ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 8 Potholes, 6.8ms
Speed: 2.1ms preprocess, 6.8ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 7.1ms
Speed: 2.1ms preprocess, 7.1ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 7.0ms
Speed: 2.5ms preprocess, 7.0ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 7.8ms
Speed: 2.0ms preprocess, 7.8ms inference, 1.1ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 7.4ms
Speed: 1.9ms preprocess, 7.4ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 8 Potholes, 6.8ms
Speed: 2.2ms preprocess, 6.8ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 9.7ms
Speed: 2.1ms preprocess, 9.7ms inference, 1.1ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 7.1ms
Speed: 2.2ms preprocess, 7.1ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 7.0ms
Speed: 1.5ms preprocess, 7.0ms inference, 1.1ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 7.2ms
Speed: 2.2ms preprocess, 7.2ms inference, 1.1ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 7.5ms
Speed: 2.0ms preprocess, 7.5ms inference, 1.1ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 7.5ms
Speed: 2.6ms preprocess, 7.5ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 8.0ms
Speed: 2.0ms preprocess, 8.0ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 7.6ms
Speed: 2.0ms preprocess, 7.6ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 11.1ms
Speed: 2.0ms preprocess, 11.1ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 10.5ms
Speed: 2.0ms preprocess, 10.5ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 8 Potholes, 9.2ms
Speed: 3.1ms preprocess, 9.2ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 9 Potholes, 8.3ms
Speed: 1.8ms preprocess, 8.3ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 17.0ms
Speed: 2.8ms preprocess, 17.0ms inference, 2.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 9 Potholes, 9.7ms
Speed: 2.4ms preprocess, 9.7ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 8 Potholes, 9.2ms
Speed: 2.3ms preprocess, 9.2ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 10.3ms
Speed: 2.6ms preprocess, 10.3ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 8 Potholes, 7.1ms
Speed: 2.2ms preprocess, 7.1ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 7.5ms
Speed: 2.0ms preprocess, 7.5ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 8.4ms
Speed: 1.9ms preprocess, 8.4ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 7.5ms
Speed: 2.0ms preprocess, 7.5ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 7.3ms
Speed: 2.0ms preprocess, 7.3ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 9.0ms
Speed: 2.0ms preprocess, 9.0ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 7.5ms
Speed: 1.9ms preprocess, 7.5ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 7.4ms
Speed: 2.0ms preprocess, 7.4ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 8.3ms
Speed: 3.0ms preprocess, 8.3ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 7.7ms
Speed: 2.4ms preprocess, 7.7ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 9.4ms
Speed: 1.8ms preprocess, 9.4ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 7.2ms
Speed: 2.1ms preprocess, 7.2ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 6.9ms
Speed: 2.6ms preprocess, 6.9ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 7.3ms
Speed: 2.1ms preprocess, 7.3ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 6.6ms
Speed: 1.8ms preprocess, 6.6ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 9.1ms
Speed: 2.0ms preprocess, 9.1ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 6.5ms
Speed: 3.1ms preprocess, 6.5ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 7.4ms
Speed: 2.0ms preprocess, 7.4ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 8 Potholes, 7.5ms
Speed: 4.9ms preprocess, 7.5ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 6.8ms
Speed: 1.6ms preprocess, 6.8ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 8 Potholes, 7.3ms
Speed: 1.9ms preprocess, 7.3ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 8 Potholes, 11.8ms
Speed: 2.1ms preprocess, 11.8ms inference, 1.8ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 9.4ms
Speed: 3.1ms preprocess, 9.4ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 10.4ms
Speed: 2.1ms preprocess, 10.4ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 9 Potholes, 10.7ms
Speed: 3.6ms preprocess, 10.7ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 9 Potholes, 13.6ms
Speed: 2.1ms preprocess, 13.6ms inference, 3.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 8 Potholes, 10.4ms
Speed: 2.4ms preprocess, 10.4ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 10.8ms
Speed: 4.5ms preprocess, 10.8ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 9.3ms
Speed: 2.1ms preprocess, 9.3ms inference, 1.8ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 11.6ms
Speed: 2.7ms preprocess, 11.6ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 9.7ms
Speed: 1.7ms preprocess, 9.7ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 7.0ms
Speed: 2.4ms preprocess, 7.0ms inference, 1.1ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 8.1ms
Speed: 2.2ms preprocess, 8.1ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 6.4ms
Speed: 1.8ms preprocess, 6.4ms inference, 1.1ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 6.9ms
Speed: 2.3ms preprocess, 6.9ms inference, 1.1ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 11.1ms
Speed: 2.3ms preprocess, 11.1ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 6.8ms
Speed: 2.0ms preprocess, 6.8ms inference, 1.1ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 6.5ms
Speed: 1.6ms preprocess, 6.5ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 7.4ms
Speed: 2.0ms preprocess, 7.4ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 8 Potholes, 7.1ms
Speed: 2.4ms preprocess, 7.1ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 6.9ms
Speed: 2.1ms preprocess, 6.9ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 8.5ms
Speed: 2.0ms preprocess, 8.5ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 7.2ms
Speed: 2.1ms preprocess, 7.2ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 7.1ms
Speed: 2.0ms preprocess, 7.1ms inference, 1.1ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 9.8ms
Speed: 2.3ms preprocess, 9.8ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 7.0ms
Speed: 2.4ms preprocess, 7.0ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 6.4ms
Speed: 2.1ms preprocess, 6.4ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 8 Potholes, 9.2ms
Speed: 2.2ms preprocess, 9.2ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 6.6ms
Speed: 1.6ms preprocess, 6.6ms inference, 1.1ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 10.6ms
Speed: 2.4ms preprocess, 10.6ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 10.5ms
Speed: 2.0ms preprocess, 10.5ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 8 Potholes, 9.2ms
Speed: 2.0ms preprocess, 9.2ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 9.0ms
Speed: 2.2ms preprocess, 9.0ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 13.9ms
Speed: 2.8ms preprocess, 13.9ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 16.2ms
Speed: 2.4ms preprocess, 16.2ms inference, 1.8ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 9.3ms
Speed: 3.4ms preprocess, 9.3ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 10.6ms
Speed: 2.1ms preprocess, 10.6ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 9.1ms
Speed: 3.2ms preprocess, 9.1ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 10.7ms
Speed: 2.1ms preprocess, 10.7ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 9.5ms
Speed: 2.0ms preprocess, 9.5ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 7.0ms
Speed: 2.3ms preprocess, 7.0ms inference, 1.1ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 6.7ms
Speed: 3.5ms preprocess, 6.7ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 12.6ms
Speed: 1.9ms preprocess, 12.6ms inference, 1.8ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 11.4ms
Speed: 3.6ms preprocess, 11.4ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 11.8ms
Speed: 2.1ms preprocess, 11.8ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 11.1ms
Speed: 2.1ms preprocess, 11.1ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 8.4ms
Speed: 1.9ms preprocess, 8.4ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 10.1ms
Speed: 2.1ms preprocess, 10.1ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 13.2ms
Speed: 3.2ms preprocess, 13.2ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 9.6ms
Speed: 2.0ms preprocess, 9.6ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 12.5ms
Speed: 2.0ms preprocess, 12.5ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 8 Potholes, 9.2ms
Speed: 2.7ms preprocess, 9.2ms inference, 2.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 8 Potholes, 8.5ms
Speed: 2.3ms preprocess, 8.5ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 10.6ms
Speed: 2.0ms preprocess, 10.6ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 14.6ms
Speed: 2.1ms preprocess, 14.6ms inference, 2.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 11.1ms
Speed: 2.0ms preprocess, 11.1ms inference, 1.8ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 10.9ms
Speed: 1.9ms preprocess, 10.9ms inference, 2.0ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 8.6ms
Speed: 2.0ms preprocess, 8.6ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 26.7ms
Speed: 2.0ms preprocess, 26.7ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 17.3ms
Speed: 2.0ms preprocess, 17.3ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 10.0ms
Speed: 4.0ms preprocess, 10.0ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 8.0ms
Speed: 1.9ms preprocess, 8.0ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 12.6ms
Speed: 2.0ms preprocess, 12.6ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 8 Potholes, 10.1ms
Speed: 2.0ms preprocess, 10.1ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 8.9ms
Speed: 2.0ms preprocess, 8.9ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 7.9ms
Speed: 2.3ms preprocess, 7.9ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 8 Potholes, 9.0ms
Speed: 1.9ms preprocess, 9.0ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 7.7ms
Speed: 2.0ms preprocess, 7.7ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 8.1ms
Speed: 1.9ms preprocess, 8.1ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 8.0ms
Speed: 2.2ms preprocess, 8.0ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 8.6ms
Speed: 1.9ms preprocess, 8.6ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 9.8ms
Speed: 2.0ms preprocess, 9.8ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 11.4ms
Speed: 2.6ms preprocess, 11.4ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 10.2ms
Speed: 3.0ms preprocess, 10.2ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 13.1ms
Speed: 3.1ms preprocess, 13.1ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 18.2ms
Speed: 2.0ms preprocess, 18.2ms inference, 4.4ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 12.3ms
Speed: 2.9ms preprocess, 12.3ms inference, 1.8ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 12.6ms
Speed: 2.1ms preprocess, 12.6ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 9.9ms
Speed: 2.0ms preprocess, 9.9ms inference, 1.9ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 10.0ms
Speed: 2.6ms preprocess, 10.0ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 11.7ms
Speed: 2.1ms preprocess, 11.7ms inference, 2.0ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 17.7ms
Speed: 3.1ms preprocess, 17.7ms inference, 1.9ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 10.9ms
Speed: 2.5ms preprocess, 10.9ms inference, 1.9ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 8 Potholes, 8.4ms
Speed: 2.0ms preprocess, 8.4ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 12.9ms
Speed: 2.0ms preprocess, 12.9ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 8.7ms
Speed: 2.0ms preprocess, 8.7ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 9.3ms
Speed: 1.9ms preprocess, 9.3ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 8.8ms
Speed: 2.0ms preprocess, 8.8ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 8.2ms
Speed: 2.0ms preprocess, 8.2ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 8.5ms
Speed: 2.5ms preprocess, 8.5ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 8.3ms
Speed: 2.4ms preprocess, 8.3ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 10.7ms
Speed: 2.5ms preprocess, 10.7ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 8.4ms
Speed: 2.0ms preprocess, 8.4ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 8.2ms
Speed: 2.4ms preprocess, 8.2ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 13.8ms
Speed: 3.2ms preprocess, 13.8ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 12.2ms
Speed: 4.5ms preprocess, 12.2ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 13.3ms
Speed: 3.3ms preprocess, 13.3ms inference, 2.7ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 21.6ms
Speed: 3.2ms preprocess, 21.6ms inference, 2.1ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 11.9ms
Speed: 2.7ms preprocess, 11.9ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 14.0ms
Speed: 5.2ms preprocess, 14.0ms inference, 2.1ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 8.6ms
Speed: 2.0ms preprocess, 8.6ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 8.1ms
Speed: 2.4ms preprocess, 8.1ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 7.9ms
Speed: 2.3ms preprocess, 7.9ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 8.0ms
Speed: 2.2ms preprocess, 8.0ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 11.6ms
Speed: 2.3ms preprocess, 11.6ms inference, 2.0ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 9.5ms
Speed: 2.1ms preprocess, 9.5ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 13.4ms
Speed: 2.8ms preprocess, 13.4ms inference, 2.0ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 12.2ms
Speed: 2.9ms preprocess, 12.2ms inference, 1.8ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 8.5ms
Speed: 2.1ms preprocess, 8.5ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 9.6ms
Speed: 2.7ms preprocess, 9.6ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 8.4ms
Speed: 2.4ms preprocess, 8.4ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 8.9ms
Speed: 2.2ms preprocess, 8.9ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 2 Potholes, 13.8ms
Speed: 4.5ms preprocess, 13.8ms inference, 1.8ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 2 Potholes, 11.3ms
Speed: 2.1ms preprocess, 11.3ms inference, 1.8ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 8.8ms
Speed: 3.4ms preprocess, 8.8ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 19.0ms
Speed: 2.0ms preprocess, 19.0ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 10.8ms
Speed: 2.0ms preprocess, 10.8ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 12.0ms
Speed: 4.2ms preprocess, 12.0ms inference, 2.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 13.3ms
Speed: 5.1ms preprocess, 13.3ms inference, 1.8ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 10.7ms
Speed: 2.0ms preprocess, 10.7ms inference, 2.1ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 15.5ms
Speed: 3.2ms preprocess, 15.5ms inference, 2.9ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 13.2ms
Speed: 2.0ms preprocess, 13.2ms inference, 1.9ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 11.5ms
Speed: 2.1ms preprocess, 11.5ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 21.0ms
Speed: 4.2ms preprocess, 21.0ms inference, 2.8ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 8 Potholes, 21.6ms
Speed: 4.4ms preprocess, 21.6ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 12.5ms
Speed: 2.0ms preprocess, 12.5ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 11.7ms
Speed: 4.6ms preprocess, 11.7ms inference, 2.0ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 13.5ms
Speed: 2.1ms preprocess, 13.5ms inference, 2.0ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 11.7ms
Speed: 3.9ms preprocess, 11.7ms inference, 5.1ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 10.5ms
Speed: 2.0ms preprocess, 10.5ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 14.3ms
Speed: 2.0ms preprocess, 14.3ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 12.9ms
Speed: 4.6ms preprocess, 12.9ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 8.8ms
Speed: 2.2ms preprocess, 8.8ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 6.8ms
Speed: 2.4ms preprocess, 6.8ms inference, 1.1ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 9.0ms
Speed: 2.1ms preprocess, 9.0ms inference, 1.9ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 10.8ms
Speed: 2.1ms preprocess, 10.8ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 12.8ms
Speed: 2.1ms preprocess, 12.8ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 1 Pothole, 9.6ms
Speed: 3.0ms preprocess, 9.6ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 10.6ms
Speed: 2.5ms preprocess, 10.6ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 12.4ms
Speed: 2.4ms preprocess, 12.4ms inference, 1.9ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 9.4ms
Speed: 1.9ms preprocess, 9.4ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 9.2ms
Speed: 2.1ms preprocess, 9.2ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 (no detections), 8.9ms
Speed: 2.0ms preprocess, 8.9ms inference, 0.8ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 8.3ms
Speed: 2.0ms preprocess, 8.3ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 1 Pothole, 7.3ms
Speed: 2.1ms preprocess, 7.3ms inference, 1.1ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 2 Potholes, 8.8ms
Speed: 2.1ms preprocess, 8.8ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 7.2ms
Speed: 2.2ms preprocess, 7.2ms inference, 1.1ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 7.1ms
Speed: 2.3ms preprocess, 7.1ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 8.3ms
Speed: 2.3ms preprocess, 8.3ms inference, 1.1ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 6.9ms
Speed: 3.3ms preprocess, 6.9ms inference, 1.1ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 8.0ms
Speed: 2.1ms preprocess, 8.0ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 7.0ms
Speed: 2.6ms preprocess, 7.0ms inference, 1.1ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 15.1ms
Speed: 4.0ms preprocess, 15.1ms inference, 2.1ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 6.7ms
Speed: 2.2ms preprocess, 6.7ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 10.2ms
Speed: 2.0ms preprocess, 10.2ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 7.7ms
Speed: 2.1ms preprocess, 7.7ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 7.1ms
Speed: 2.1ms preprocess, 7.1ms inference, 1.1ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 8.0ms
Speed: 1.9ms preprocess, 8.0ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 7.2ms
Speed: 2.9ms preprocess, 7.2ms inference, 1.1ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 7.1ms
Speed: 2.5ms preprocess, 7.1ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 8.9ms
Speed: 2.1ms preprocess, 8.9ms inference, 1.1ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 7.1ms
Speed: 2.1ms preprocess, 7.1ms inference, 1.1ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 8.1ms
Speed: 2.3ms preprocess, 8.1ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 7.1ms
Speed: 2.9ms preprocess, 7.1ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 6.5ms
Speed: 2.1ms preprocess, 6.5ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 10.0ms
Speed: 2.1ms preprocess, 10.0ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 10.7ms
Speed: 1.9ms preprocess, 10.7ms inference, 1.8ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 9.7ms
Speed: 2.6ms preprocess, 9.7ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 11.5ms
Speed: 1.9ms preprocess, 11.5ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 11.2ms
Speed: 2.1ms preprocess, 11.2ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 9.5ms
Speed: 1.9ms preprocess, 9.5ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 11.2ms
Speed: 2.7ms preprocess, 11.2ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 9.7ms
Speed: 2.3ms preprocess, 9.7ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 9.4ms
Speed: 2.2ms preprocess, 9.4ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 10.1ms
Speed: 3.2ms preprocess, 10.1ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 10.7ms
Speed: 1.9ms preprocess, 10.7ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 9.7ms
Speed: 2.3ms preprocess, 9.7ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 7.0ms
Speed: 2.0ms preprocess, 7.0ms inference, 1.1ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 8.3ms
Speed: 2.1ms preprocess, 8.3ms inference, 1.1ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 7.2ms
Speed: 2.3ms preprocess, 7.2ms inference, 1.1ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 8.2ms
Speed: 2.0ms preprocess, 8.2ms inference, 1.1ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 12.9ms
Speed: 2.0ms preprocess, 12.9ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 7.9ms
Speed: 1.9ms preprocess, 7.9ms inference, 2.0ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 2 Potholes, 6.9ms
Speed: 3.0ms preprocess, 6.9ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 8.8ms
Speed: 1.9ms preprocess, 8.8ms inference, 1.1ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 6.6ms
Speed: 1.5ms preprocess, 6.6ms inference, 1.1ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 8.8ms
Speed: 1.9ms preprocess, 8.8ms inference, 1.1ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 7.5ms
Speed: 1.9ms preprocess, 7.5ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 7.6ms
Speed: 1.9ms preprocess, 7.6ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 7.0ms
Speed: 2.1ms preprocess, 7.0ms inference, 1.1ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 7.8ms
Speed: 2.0ms preprocess, 7.8ms inference, 2.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 7.3ms
Speed: 2.3ms preprocess, 7.3ms inference, 1.1ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 8.3ms
Speed: 2.0ms preprocess, 8.3ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 8.3ms
Speed: 2.3ms preprocess, 8.3ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 9.6ms
Speed: 2.1ms preprocess, 9.6ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 9.2ms
Speed: 2.5ms preprocess, 9.2ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 8 Potholes, 10.6ms
Speed: 1.9ms preprocess, 10.6ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 9.5ms
Speed: 1.8ms preprocess, 9.5ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 13.0ms
Speed: 3.4ms preprocess, 13.0ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 9.6ms
Speed: 3.3ms preprocess, 9.6ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 8.8ms
Speed: 2.1ms preprocess, 8.8ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 9.9ms
Speed: 1.9ms preprocess, 9.9ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 6.5ms
Speed: 1.7ms preprocess, 6.5ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 9.3ms
Speed: 2.4ms preprocess, 9.3ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 9.8ms
Speed: 3.2ms preprocess, 9.8ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 6.6ms
Speed: 2.0ms preprocess, 6.6ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 7.1ms
Speed: 2.8ms preprocess, 7.1ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 9.1ms
Speed: 1.9ms preprocess, 9.1ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 7.4ms
Speed: 1.9ms preprocess, 7.4ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 7.2ms
Speed: 1.9ms preprocess, 7.2ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 7.9ms
Speed: 1.9ms preprocess, 7.9ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 10.5ms
Speed: 3.4ms preprocess, 10.5ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 7.4ms
Speed: 2.0ms preprocess, 7.4ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 8.6ms
Speed: 2.0ms preprocess, 8.6ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 10.1ms
Speed: 1.9ms preprocess, 10.1ms inference, 1.8ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 7.5ms
Speed: 2.1ms preprocess, 7.5ms inference, 1.1ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 8.4ms
Speed: 2.1ms preprocess, 8.4ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 7.4ms
Speed: 2.1ms preprocess, 7.4ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 6.7ms
Speed: 2.2ms preprocess, 6.7ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 10.2ms
Speed: 2.1ms preprocess, 10.2ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 8.1ms
Speed: 2.8ms preprocess, 8.1ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 9.4ms
Speed: 2.0ms preprocess, 9.4ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 11.5ms
Speed: 2.0ms preprocess, 11.5ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 9.2ms
Speed: 2.0ms preprocess, 9.2ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 10.7ms
Speed: 2.7ms preprocess, 10.7ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 10.5ms
Speed: 2.2ms preprocess, 10.5ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 9.2ms
Speed: 2.5ms preprocess, 9.2ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 8.9ms
Speed: 2.5ms preprocess, 8.9ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 2 Potholes, 13.3ms
Speed: 2.6ms preprocess, 13.3ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 9.6ms
Speed: 2.5ms preprocess, 9.6ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 8.5ms
Speed: 2.2ms preprocess, 8.5ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 10.1ms
Speed: 1.9ms preprocess, 10.1ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 9.5ms
Speed: 2.0ms preprocess, 9.5ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 10.2ms
Speed: 1.9ms preprocess, 10.2ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 6.6ms
Speed: 3.9ms preprocess, 6.6ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 9.1ms
Speed: 1.9ms preprocess, 9.1ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 6.9ms
Speed: 2.3ms preprocess, 6.9ms inference, 1.1ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 7.2ms
Speed: 2.2ms preprocess, 7.2ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 2 Potholes, 8.5ms
Speed: 2.5ms preprocess, 8.5ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 2 Potholes, 7.2ms
Speed: 2.5ms preprocess, 7.2ms inference, 1.1ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 2 Potholes, 7.6ms
Speed: 1.6ms preprocess, 7.6ms inference, 1.1ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 2 Potholes, 11.4ms
Speed: 4.1ms preprocess, 11.4ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 2 Potholes, 6.6ms
Speed: 2.0ms preprocess, 6.6ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 2 Potholes, 9.4ms
Speed: 4.9ms preprocess, 9.4ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 14.7ms
Speed: 2.3ms preprocess, 14.7ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 2 Potholes, 8.5ms
Speed: 2.3ms preprocess, 8.5ms inference, 1.1ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 1 Pothole, 7.2ms
Speed: 2.4ms preprocess, 7.2ms inference, 1.1ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 1 Pothole, 8.5ms
Speed: 2.3ms preprocess, 8.5ms inference, 1.1ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 6.8ms
Speed: 1.6ms preprocess, 6.8ms inference, 1.1ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 7.9ms
Speed: 2.0ms preprocess, 7.9ms inference, 1.1ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 2 Potholes, 8.8ms
Speed: 2.3ms preprocess, 8.8ms inference, 1.1ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 10.0ms
Speed: 2.1ms preprocess, 10.0ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 10.2ms
Speed: 2.0ms preprocess, 10.2ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 11.1ms
Speed: 1.9ms preprocess, 11.1ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 9.4ms
Speed: 1.8ms preprocess, 9.4ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 9.9ms
Speed: 2.1ms preprocess, 9.9ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 9.4ms
Speed: 2.8ms preprocess, 9.4ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 9.6ms
Speed: 2.2ms preprocess, 9.6ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 12.1ms
Speed: 2.8ms preprocess, 12.1ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 9.4ms
Speed: 3.4ms preprocess, 9.4ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 9.7ms
Speed: 2.0ms preprocess, 9.7ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 8.4ms
Speed: 2.6ms preprocess, 8.4ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 8.8ms
Speed: 2.0ms preprocess, 8.8ms inference, 1.1ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 8.2ms
Speed: 1.9ms preprocess, 8.2ms inference, 1.1ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 8.8ms
Speed: 2.1ms preprocess, 8.8ms inference, 2.9ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 7.6ms
Speed: 1.9ms preprocess, 7.6ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 7.5ms
Speed: 1.9ms preprocess, 7.5ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 7.7ms
Speed: 1.8ms preprocess, 7.7ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 9 Potholes, 7.3ms
Speed: 2.1ms preprocess, 7.3ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 10 Potholes, 6.6ms
Speed: 1.5ms preprocess, 6.6ms inference, 1.1ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 8 Potholes, 11.6ms
Speed: 1.6ms preprocess, 11.6ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 7.9ms
Speed: 2.0ms preprocess, 7.9ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 8.1ms
Speed: 2.1ms preprocess, 8.1ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 8.6ms
Speed: 3.2ms preprocess, 8.6ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 9.1ms
Speed: 2.0ms preprocess, 9.1ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 7.7ms
Speed: 2.1ms preprocess, 7.7ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 10.0ms
Speed: 2.4ms preprocess, 10.0ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 9.1ms
Speed: 2.3ms preprocess, 9.1ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 7.0ms
Speed: 1.7ms preprocess, 7.0ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 9.5ms
Speed: 4.6ms preprocess, 9.5ms inference, 1.8ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 10.2ms
Speed: 2.1ms preprocess, 10.2ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 11.1ms
Speed: 2.1ms preprocess, 11.1ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 9.3ms
Speed: 2.1ms preprocess, 9.3ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 8.7ms
Speed: 1.8ms preprocess, 8.7ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 10.7ms
Speed: 2.5ms preprocess, 10.7ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 10.5ms
Speed: 3.9ms preprocess, 10.5ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 9.2ms
Speed: 4.9ms preprocess, 9.2ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 9.5ms
Speed: 6.3ms preprocess, 9.5ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 10.4ms
Speed: 3.7ms preprocess, 10.4ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 15.3ms
Speed: 2.1ms preprocess, 15.3ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 7.3ms
Speed: 2.3ms preprocess, 7.3ms inference, 2.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 7.4ms
Speed: 2.0ms preprocess, 7.4ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 8.2ms
Speed: 1.9ms preprocess, 8.2ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 7.4ms
Speed: 2.2ms preprocess, 7.4ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 7.3ms
Speed: 1.8ms preprocess, 7.3ms inference, 1.1ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 9.6ms
Speed: 1.9ms preprocess, 9.6ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 7.7ms
Speed: 1.9ms preprocess, 7.7ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 8.4ms
Speed: 1.9ms preprocess, 8.4ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 11.6ms
Speed: 1.9ms preprocess, 11.6ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 10.7ms
Speed: 2.0ms preprocess, 10.7ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 9.9ms
Speed: 2.0ms preprocess, 9.9ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 10.3ms
Speed: 2.1ms preprocess, 10.3ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 2 Potholes, 7.6ms
Speed: 2.1ms preprocess, 7.6ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 7.3ms
Speed: 2.2ms preprocess, 7.3ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 2 Potholes, 9.3ms
Speed: 1.9ms preprocess, 9.3ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 8.7ms
Speed: 2.1ms preprocess, 8.7ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 2 Potholes, 8.5ms
Speed: 2.1ms preprocess, 8.5ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 12.3ms
Speed: 2.1ms preprocess, 12.3ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 2 Potholes, 8.6ms
Speed: 4.8ms preprocess, 8.6ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 11.4ms
Speed: 2.2ms preprocess, 11.4ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 2 Potholes, 11.8ms
Speed: 2.1ms preprocess, 11.8ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 2 Potholes, 11.8ms
Speed: 2.8ms preprocess, 11.8ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 2 Potholes, 12.4ms
Speed: 2.1ms preprocess, 12.4ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 2 Potholes, 10.8ms
Speed: 2.5ms preprocess, 10.8ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 2 Potholes, 9.9ms
Speed: 2.2ms preprocess, 9.9ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 2 Potholes, 11.1ms
Speed: 2.1ms preprocess, 11.1ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 10.4ms
Speed: 4.5ms preprocess, 10.4ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 9.8ms
Speed: 4.9ms preprocess, 9.8ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 9.5ms
Speed: 2.1ms preprocess, 9.5ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 9.0ms
Speed: 2.1ms preprocess, 9.0ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 (no detections), 6.6ms
Speed: 1.9ms preprocess, 6.6ms inference, 0.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 2 Potholes, 9.4ms
Speed: 2.0ms preprocess, 9.4ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 2 Potholes, 7.2ms
Speed: 2.2ms preprocess, 7.2ms inference, 1.1ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 2 Potholes, 6.2ms
Speed: 3.3ms preprocess, 6.2ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 8.9ms
Speed: 2.1ms preprocess, 8.9ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 1 Pothole, 8.1ms
Speed: 2.4ms preprocess, 8.1ms inference, 1.1ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 7.0ms
Speed: 2.3ms preprocess, 7.0ms inference, 1.1ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 2 Potholes, 7.5ms
Speed: 1.9ms preprocess, 7.5ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 1 Pothole, 13.1ms
Speed: 1.9ms preprocess, 13.1ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 2 Potholes, 7.9ms
Speed: 2.0ms preprocess, 7.9ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 2 Potholes, 7.2ms
Speed: 2.8ms preprocess, 7.2ms inference, 1.1ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 2 Potholes, 9.0ms
Speed: 2.3ms preprocess, 9.0ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)
Output video exists: True
Output video size: 27223070 bytes

```

```
<Figure size 1800x600 with 2 Axes>
```

```python
import cv2
import numpy as np
from collections import deque
from ultralytics import YOLO
import matplotlib.pyplot as plt
import os
from IPython.display import Video, display

# Define paths for input and output videos
video_path = '/content/drive/MyDrive/Pothole_Segmentation_YOLOv8-1/sample_video.mp4'
output_video_path = '/content/drive/MyDrive/road_damage_assessment.mp4'
output_image_dir = '/content/drive/MyDrive/runs/detect/test_frames'  # Output directory for frames

# Create the output directory if it doesn't exist
os.makedirs(output_image_dir, exist_ok=True)

# Load the trained model
best_model = YOLO('/content/drive/MyDrive/runs/detect/train2/weights/best.pt')

# Define font and colors for annotation
font = cv2.FONT_HERSHEY_SIMPLEX
font_scale = 1
text_position = (40, 80)
font_color = (255, 255, 255)    # White text
background_color = (255, 0, 0)  # Red background for text

# Initialize deque for averaging damage percentage
damage_deque = deque(maxlen=10)

# Initialize lists to store metrics for plotting
num_detections = []
average_confidences = []

# Open the video
cap = cv2.VideoCapture(video_path)
width, height = int(cap.get(3)), int(cap.get(4))

# Define the codec and VideoWriter object for .mp4 output
fourcc = cv2.VideoWriter_fourcc(*'mp4v')
out = cv2.VideoWriter(output_video_path, fourcc, 20.0, (width, height))

# Frame counter for saving images
frame_counter = 0

# Process video frames
while cap.isOpened():
    ret, frame = cap.read()
    if not ret:
        break

    # Perform detection on the frame
    results = best_model.predict(source=frame, imgsz=640, conf=0.25)

    # Process and annotate the frame with bounding boxes
    processed_frame = results[0].plot()

    # Calculate the damage percentage based on mask areas
    percentage_damage = 0
    if results[0].masks is not None:
        total_area = 0
        masks = results[0].masks.data.cpu().numpy()
        image_area = frame.shape[0] * frame.shape[1]  # total number of pixels in the image
        for mask in masks:
            binary_mask = (mask > 0).astype(np.uint8) * 255
            contours, _ = cv2.findContours(binary_mask, cv2.RETR_TREE, cv2.CHAIN_APPROX_SIMPLE)
            for contour in contours:
                total_area += cv2.contourArea(contour)

        percentage_damage = (total_area / image_area) * 100

    # Update deque and calculate smoothed damage percentage
    damage_deque.append(percentage_damage)
    smoothed_percentage_damage = sum(damage_deque) / len(damage_deque)

    # Draw damage percentage text on the processed frame
    cv2.line(processed_frame, (text_position[0], text_position[1] - 10),
             (text_position[0] + 350, text_position[1] - 10), background_color, 40)
    cv2.putText(processed_frame, f'Road Damage: {smoothed_percentage_damage:.2f}%',
                text_position, font, font_scale, font_color, 2, cv2.LINE_AA)

    # Save the processed frame as an image in the output directory
    frame_filename = os.path.join(output_image_dir, f"frame_{frame_counter:05d}.jpg")
    cv2.imwrite(frame_filename, processed_frame)
    frame_counter += 1

    # Collect test metrics: number of detections and average confidence
    num_detections.append(len(results[0].boxes))
    if len(results[0].boxes) > 0:
        avg_conf = results[0].boxes.conf.mean().item()
        average_confidences.append(avg_conf)
    else:
        average_confidences.append(0)

    # Write the processed frame to the output video
    out.write(processed_frame)

cap.release()
out.release()

# Verify if the output video was created and its size
print(f"Output video exists: {os.path.exists(output_video_path)}")
print(f"Output video size: {os.path.getsize(output_video_path)} bytes")

# Display the processed video within the notebook
display(Video(output_video_path, embed=True, width=960))

# Plot metrics for test data
plt.figure(figsize=(18, 6))

# Plot Number of Detections
plt.subplot(1, 2, 1)
plt.plot(num_detections, label='Number of Detections')
plt.xlabel('Frame')
plt.ylabel('Count')
plt.title('Number of Detections per Frame (Test)')
plt.legend()

# Plot Average Confidence
plt.subplot(1, 2, 2)
plt.plot(average_confidences, label='Average Confidence')
plt.xlabel('Frame')
plt.ylabel('Confidence')
plt.title('Average Confidence per Frame (Test)')
plt.legend()

plt.tight_layout()
plt.show()

```

```

0: 384x640 8 Potholes, 8.5ms
Speed: 1.6ms preprocess, 8.5ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 8 Potholes, 8.3ms
Speed: 2.0ms preprocess, 8.3ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 6.5ms
Speed: 2.0ms preprocess, 6.5ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 6.6ms
Speed: 2.0ms preprocess, 6.6ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 8.6ms
Speed: 2.0ms preprocess, 8.6ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 7.5ms
Speed: 2.0ms preprocess, 7.5ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 8 Potholes, 6.9ms
Speed: 1.7ms preprocess, 6.9ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 7.3ms
Speed: 2.1ms preprocess, 7.3ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 6.7ms
Speed: 1.7ms preprocess, 6.7ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 6.7ms
Speed: 1.6ms preprocess, 6.7ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 6.7ms
Speed: 1.6ms preprocess, 6.7ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 13.1ms
Speed: 1.9ms preprocess, 13.1ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 10.8ms
Speed: 1.6ms preprocess, 10.8ms inference, 1.9ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 11.1ms
Speed: 3.3ms preprocess, 11.1ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 7.6ms
Speed: 2.1ms preprocess, 7.6ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 10.4ms
Speed: 2.9ms preprocess, 10.4ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 10.9ms
Speed: 3.4ms preprocess, 10.9ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 8 Potholes, 10.0ms
Speed: 2.4ms preprocess, 10.0ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 9 Potholes, 9.3ms
Speed: 1.7ms preprocess, 9.3ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 6.6ms
Speed: 2.0ms preprocess, 6.6ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 9 Potholes, 8.9ms
Speed: 2.0ms preprocess, 8.9ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 8 Potholes, 10.2ms
Speed: 2.4ms preprocess, 10.2ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 7.6ms
Speed: 2.4ms preprocess, 7.6ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 8 Potholes, 9.2ms
Speed: 2.8ms preprocess, 9.2ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 6.9ms
Speed: 1.8ms preprocess, 6.9ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 7.1ms
Speed: 2.2ms preprocess, 7.1ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 8.6ms
Speed: 1.9ms preprocess, 8.6ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 7.4ms
Speed: 2.8ms preprocess, 7.4ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 8.2ms
Speed: 2.0ms preprocess, 8.2ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 6.6ms
Speed: 2.0ms preprocess, 6.6ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 6.7ms
Speed: 2.2ms preprocess, 6.7ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 8.3ms
Speed: 1.9ms preprocess, 8.3ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 14.7ms
Speed: 2.4ms preprocess, 14.7ms inference, 4.9ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 6.8ms
Speed: 3.0ms preprocess, 6.8ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 12.9ms
Speed: 2.6ms preprocess, 12.9ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 12.6ms
Speed: 3.4ms preprocess, 12.6ms inference, 2.0ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 10.4ms
Speed: 3.1ms preprocess, 10.4ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 10.0ms
Speed: 2.0ms preprocess, 10.0ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 8.2ms
Speed: 4.4ms preprocess, 8.2ms inference, 1.8ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 7.5ms
Speed: 2.2ms preprocess, 7.5ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 8.7ms
Speed: 2.2ms preprocess, 8.7ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 8 Potholes, 7.8ms
Speed: 2.2ms preprocess, 7.8ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 6.9ms
Speed: 1.7ms preprocess, 6.9ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 8 Potholes, 6.8ms
Speed: 2.0ms preprocess, 6.8ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 8 Potholes, 8.6ms
Speed: 2.0ms preprocess, 8.6ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 9.2ms
Speed: 1.9ms preprocess, 9.2ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 8.6ms
Speed: 2.1ms preprocess, 8.6ms inference, 2.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 9 Potholes, 9.3ms
Speed: 1.9ms preprocess, 9.3ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 9 Potholes, 10.6ms
Speed: 1.9ms preprocess, 10.6ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 8 Potholes, 8.0ms
Speed: 2.6ms preprocess, 8.0ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 8.9ms
Speed: 2.2ms preprocess, 8.9ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 7.6ms
Speed: 2.4ms preprocess, 7.6ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 12.0ms
Speed: 2.0ms preprocess, 12.0ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 7.3ms
Speed: 2.1ms preprocess, 7.3ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 10.6ms
Speed: 2.7ms preprocess, 10.6ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 11.2ms
Speed: 2.1ms preprocess, 11.2ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 10.7ms
Speed: 2.5ms preprocess, 10.7ms inference, 1.9ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 11.3ms
Speed: 2.7ms preprocess, 11.3ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 12.8ms
Speed: 2.6ms preprocess, 12.8ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 7.7ms
Speed: 2.1ms preprocess, 7.7ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 6.8ms
Speed: 1.6ms preprocess, 6.8ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 9.1ms
Speed: 2.2ms preprocess, 9.1ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 8 Potholes, 7.3ms
Speed: 1.6ms preprocess, 7.3ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 6.5ms
Speed: 1.9ms preprocess, 6.5ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 8.0ms
Speed: 2.0ms preprocess, 8.0ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 8.5ms
Speed: 1.6ms preprocess, 8.5ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 7.7ms
Speed: 2.5ms preprocess, 7.7ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 7.4ms
Speed: 2.0ms preprocess, 7.4ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 6.8ms
Speed: 2.1ms preprocess, 6.8ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 6.8ms
Speed: 2.7ms preprocess, 6.8ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 8 Potholes, 8.3ms
Speed: 2.5ms preprocess, 8.3ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 7.4ms
Speed: 2.6ms preprocess, 7.4ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 10.4ms
Speed: 2.0ms preprocess, 10.4ms inference, 1.9ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 11.4ms
Speed: 3.7ms preprocess, 11.4ms inference, 2.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 8 Potholes, 9.1ms
Speed: 2.2ms preprocess, 9.1ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 10.0ms
Speed: 2.8ms preprocess, 10.0ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 10.3ms
Speed: 2.8ms preprocess, 10.3ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 12.1ms
Speed: 2.1ms preprocess, 12.1ms inference, 3.8ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 8.4ms
Speed: 2.0ms preprocess, 8.4ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 8.2ms
Speed: 2.4ms preprocess, 8.2ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 7.0ms
Speed: 1.7ms preprocess, 7.0ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 6.9ms
Speed: 1.6ms preprocess, 6.9ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 9.2ms
Speed: 3.3ms preprocess, 9.2ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 7.0ms
Speed: 1.8ms preprocess, 7.0ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 7.0ms
Speed: 2.0ms preprocess, 7.0ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 7.9ms
Speed: 3.0ms preprocess, 7.9ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 7.5ms
Speed: 2.5ms preprocess, 7.5ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 9.5ms
Speed: 2.5ms preprocess, 9.5ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 6.9ms
Speed: 2.0ms preprocess, 6.9ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 6.8ms
Speed: 2.0ms preprocess, 6.8ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 7.0ms
Speed: 1.5ms preprocess, 7.0ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 8.4ms
Speed: 2.7ms preprocess, 8.4ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 14.4ms
Speed: 2.0ms preprocess, 14.4ms inference, 1.9ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 11.9ms
Speed: 2.8ms preprocess, 11.9ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 8 Potholes, 11.6ms
Speed: 2.3ms preprocess, 11.6ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 8 Potholes, 9.0ms
Speed: 2.1ms preprocess, 9.0ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 9.6ms
Speed: 2.1ms preprocess, 9.6ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 7.2ms
Speed: 2.0ms preprocess, 7.2ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 6.6ms
Speed: 1.7ms preprocess, 6.6ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 6.8ms
Speed: 1.6ms preprocess, 6.8ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 7.6ms
Speed: 3.8ms preprocess, 7.6ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 8.5ms
Speed: 2.5ms preprocess, 8.5ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 7.1ms
Speed: 1.6ms preprocess, 7.1ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 7.8ms
Speed: 2.1ms preprocess, 7.8ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 7.2ms
Speed: 1.8ms preprocess, 7.2ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 6.9ms
Speed: 1.6ms preprocess, 6.9ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 8 Potholes, 8.9ms
Speed: 2.4ms preprocess, 8.9ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 11.1ms
Speed: 2.3ms preprocess, 11.1ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 7.3ms
Speed: 1.7ms preprocess, 7.3ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 8 Potholes, 7.5ms
Speed: 2.0ms preprocess, 7.5ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 6.9ms
Speed: 2.1ms preprocess, 6.9ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 7.3ms
Speed: 3.0ms preprocess, 7.3ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 10.9ms
Speed: 2.6ms preprocess, 10.9ms inference, 2.0ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 10.9ms
Speed: 2.3ms preprocess, 10.9ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 11.1ms
Speed: 2.2ms preprocess, 11.1ms inference, 2.1ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 11.1ms
Speed: 2.8ms preprocess, 11.1ms inference, 1.9ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 10.2ms
Speed: 4.8ms preprocess, 10.2ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 14.3ms
Speed: 2.1ms preprocess, 14.3ms inference, 1.9ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 11.5ms
Speed: 2.1ms preprocess, 11.5ms inference, 1.8ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 14.0ms
Speed: 2.8ms preprocess, 14.0ms inference, 2.1ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 11.5ms
Speed: 2.1ms preprocess, 11.5ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 8.7ms
Speed: 3.3ms preprocess, 8.7ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 8.7ms
Speed: 3.5ms preprocess, 8.7ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 11.1ms
Speed: 2.1ms preprocess, 11.1ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 10.3ms
Speed: 2.1ms preprocess, 10.3ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 11.2ms
Speed: 1.9ms preprocess, 11.2ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 8 Potholes, 9.2ms
Speed: 2.0ms preprocess, 9.2ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 15.4ms
Speed: 3.9ms preprocess, 15.4ms inference, 7.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 14.4ms
Speed: 2.0ms preprocess, 14.4ms inference, 2.1ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 11.2ms
Speed: 2.1ms preprocess, 11.2ms inference, 1.9ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 9.0ms
Speed: 1.9ms preprocess, 9.0ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 11.7ms
Speed: 2.7ms preprocess, 11.7ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 8.4ms
Speed: 2.3ms preprocess, 8.4ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 9.1ms
Speed: 2.0ms preprocess, 9.1ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 8.5ms
Speed: 1.9ms preprocess, 8.5ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 9.7ms
Speed: 2.0ms preprocess, 9.7ms inference, 1.8ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 11.4ms
Speed: 4.4ms preprocess, 11.4ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 14.4ms
Speed: 2.0ms preprocess, 14.4ms inference, 1.8ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 10.8ms
Speed: 2.2ms preprocess, 10.8ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 9.5ms
Speed: 2.0ms preprocess, 9.5ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 13.8ms
Speed: 2.0ms preprocess, 13.8ms inference, 1.8ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 9.3ms
Speed: 1.9ms preprocess, 9.3ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 8.1ms
Speed: 2.1ms preprocess, 8.1ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 11.0ms
Speed: 4.4ms preprocess, 11.0ms inference, 1.8ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 13.2ms
Speed: 2.0ms preprocess, 13.2ms inference, 1.9ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 14.4ms
Speed: 2.1ms preprocess, 14.4ms inference, 1.9ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 12.5ms
Speed: 4.6ms preprocess, 12.5ms inference, 3.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 9.4ms
Speed: 2.0ms preprocess, 9.4ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 11.0ms
Speed: 2.2ms preprocess, 11.0ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 12.4ms
Speed: 3.8ms preprocess, 12.4ms inference, 1.9ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 9.0ms
Speed: 2.5ms preprocess, 9.0ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 9.2ms
Speed: 2.8ms preprocess, 9.2ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 9.2ms
Speed: 2.4ms preprocess, 9.2ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 8.4ms
Speed: 2.2ms preprocess, 8.4ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 8.0ms
Speed: 2.3ms preprocess, 8.0ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 2 Potholes, 9.8ms
Speed: 3.0ms preprocess, 9.8ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 2 Potholes, 10.2ms
Speed: 1.8ms preprocess, 10.2ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 12.1ms
Speed: 2.3ms preprocess, 12.1ms inference, 2.8ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 12.2ms
Speed: 2.4ms preprocess, 12.2ms inference, 1.8ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 13.3ms
Speed: 4.3ms preprocess, 13.3ms inference, 3.1ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 15.0ms
Speed: 2.0ms preprocess, 15.0ms inference, 2.1ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 20.3ms
Speed: 2.1ms preprocess, 20.3ms inference, 3.9ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 9.4ms
Speed: 4.9ms preprocess, 9.4ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 10.9ms
Speed: 2.1ms preprocess, 10.9ms inference, 1.8ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 11.7ms
Speed: 2.8ms preprocess, 11.7ms inference, 1.9ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 13.4ms
Speed: 2.3ms preprocess, 13.4ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 17.7ms
Speed: 2.1ms preprocess, 17.7ms inference, 1.8ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 8 Potholes, 10.8ms
Speed: 2.1ms preprocess, 10.8ms inference, 1.8ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 10.5ms
Speed: 2.2ms preprocess, 10.5ms inference, 1.8ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 10.1ms
Speed: 3.0ms preprocess, 10.1ms inference, 2.0ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 10.1ms
Speed: 2.2ms preprocess, 10.1ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 11.2ms
Speed: 2.3ms preprocess, 11.2ms inference, 1.8ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 11.1ms
Speed: 2.2ms preprocess, 11.1ms inference, 1.8ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 15.8ms
Speed: 6.4ms preprocess, 15.8ms inference, 2.1ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 9.5ms
Speed: 2.7ms preprocess, 9.5ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 9.9ms
Speed: 3.0ms preprocess, 9.9ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 16.9ms
Speed: 4.2ms preprocess, 16.9ms inference, 1.9ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 10.3ms
Speed: 2.1ms preprocess, 10.3ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 9.6ms
Speed: 3.2ms preprocess, 9.6ms inference, 1.8ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 9.8ms
Speed: 2.8ms preprocess, 9.8ms inference, 1.8ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 1 Pothole, 9.9ms
Speed: 2.9ms preprocess, 9.9ms inference, 1.8ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 12.1ms
Speed: 2.2ms preprocess, 12.1ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 11.3ms
Speed: 2.8ms preprocess, 11.3ms inference, 1.8ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 12.0ms
Speed: 2.2ms preprocess, 12.0ms inference, 1.8ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 12.6ms
Speed: 9.0ms preprocess, 12.6ms inference, 1.9ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 (no detections), 11.7ms
Speed: 2.0ms preprocess, 11.7ms inference, 0.8ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 13.1ms
Speed: 5.7ms preprocess, 13.1ms inference, 1.8ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 1 Pothole, 22.9ms
Speed: 2.1ms preprocess, 22.9ms inference, 2.0ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 2 Potholes, 12.0ms
Speed: 2.8ms preprocess, 12.0ms inference, 1.8ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 9.5ms
Speed: 3.8ms preprocess, 9.5ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 8.0ms
Speed: 2.3ms preprocess, 8.0ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 6.9ms
Speed: 2.1ms preprocess, 6.9ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 7.6ms
Speed: 2.3ms preprocess, 7.6ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 9.1ms
Speed: 2.1ms preprocess, 9.1ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 11.2ms
Speed: 2.2ms preprocess, 11.2ms inference, 3.1ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 8.8ms
Speed: 3.2ms preprocess, 8.8ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 12.2ms
Speed: 2.4ms preprocess, 12.2ms inference, 3.8ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 7.1ms
Speed: 2.2ms preprocess, 7.1ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 8.4ms
Speed: 2.3ms preprocess, 8.4ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 12.3ms
Speed: 2.3ms preprocess, 12.3ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 7.3ms
Speed: 2.0ms preprocess, 7.3ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 6.6ms
Speed: 1.7ms preprocess, 6.6ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 7.7ms
Speed: 2.3ms preprocess, 7.7ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 8.4ms
Speed: 3.0ms preprocess, 8.4ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 11.1ms
Speed: 2.2ms preprocess, 11.1ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 11.0ms
Speed: 2.4ms preprocess, 11.0ms inference, 1.9ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 9.9ms
Speed: 2.0ms preprocess, 9.9ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 9.8ms
Speed: 2.2ms preprocess, 9.8ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 11.5ms
Speed: 1.9ms preprocess, 11.5ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 8.1ms
Speed: 2.2ms preprocess, 8.1ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 10.7ms
Speed: 2.0ms preprocess, 10.7ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 6.9ms
Speed: 2.1ms preprocess, 6.9ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 9.2ms
Speed: 1.9ms preprocess, 9.2ms inference, 3.8ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 9.0ms
Speed: 2.1ms preprocess, 9.0ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 9.0ms
Speed: 2.0ms preprocess, 9.0ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 6.9ms
Speed: 1.6ms preprocess, 6.9ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 8.5ms
Speed: 1.9ms preprocess, 8.5ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 10.1ms
Speed: 1.9ms preprocess, 10.1ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 9.2ms
Speed: 1.9ms preprocess, 9.2ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 6.9ms
Speed: 1.6ms preprocess, 6.9ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 8.4ms
Speed: 1.9ms preprocess, 8.4ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 9.4ms
Speed: 1.9ms preprocess, 9.4ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 7.9ms
Speed: 1.9ms preprocess, 7.9ms inference, 2.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 8.9ms
Speed: 2.1ms preprocess, 8.9ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 10.3ms
Speed: 1.9ms preprocess, 10.3ms inference, 1.8ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 11.1ms
Speed: 2.1ms preprocess, 11.1ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 2 Potholes, 9.9ms
Speed: 1.7ms preprocess, 9.9ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 12.5ms
Speed: 2.6ms preprocess, 12.5ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 11.0ms
Speed: 2.1ms preprocess, 11.0ms inference, 1.9ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 9.2ms
Speed: 2.5ms preprocess, 9.2ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 11.8ms
Speed: 2.8ms preprocess, 11.8ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 7.8ms
Speed: 2.2ms preprocess, 7.8ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 9.0ms
Speed: 2.4ms preprocess, 9.0ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 7.5ms
Speed: 2.5ms preprocess, 7.5ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 6.7ms
Speed: 1.6ms preprocess, 6.7ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 8.6ms
Speed: 1.9ms preprocess, 8.6ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 8.8ms
Speed: 2.8ms preprocess, 8.8ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 7.7ms
Speed: 2.9ms preprocess, 7.7ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 7.7ms
Speed: 2.1ms preprocess, 7.7ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 8 Potholes, 7.0ms
Speed: 1.5ms preprocess, 7.0ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 7.2ms
Speed: 1.9ms preprocess, 7.2ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 7.6ms
Speed: 2.0ms preprocess, 7.6ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 6.5ms
Speed: 2.0ms preprocess, 6.5ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 10.8ms
Speed: 3.7ms preprocess, 10.8ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 11.1ms
Speed: 2.2ms preprocess, 11.1ms inference, 1.8ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 9.6ms
Speed: 2.0ms preprocess, 9.6ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 9.6ms
Speed: 4.3ms preprocess, 9.6ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 9.7ms
Speed: 2.2ms preprocess, 9.7ms inference, 1.9ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 9.6ms
Speed: 2.0ms preprocess, 9.6ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 7.2ms
Speed: 2.8ms preprocess, 7.2ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 11.2ms
Speed: 2.0ms preprocess, 11.2ms inference, 3.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 7.7ms
Speed: 2.9ms preprocess, 7.7ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 11.7ms
Speed: 2.7ms preprocess, 11.7ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 7.3ms
Speed: 1.9ms preprocess, 7.3ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 7.1ms
Speed: 2.0ms preprocess, 7.1ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 8.5ms
Speed: 1.9ms preprocess, 8.5ms inference, 1.8ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 7.4ms
Speed: 2.2ms preprocess, 7.4ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 8.1ms
Speed: 1.9ms preprocess, 8.1ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 7.0ms
Speed: 1.6ms preprocess, 7.0ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 8.9ms
Speed: 2.7ms preprocess, 8.9ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 7.3ms
Speed: 2.2ms preprocess, 7.3ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 6.9ms
Speed: 1.7ms preprocess, 6.9ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 10.5ms
Speed: 1.8ms preprocess, 10.5ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 9.7ms
Speed: 3.1ms preprocess, 9.7ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 9.9ms
Speed: 2.0ms preprocess, 9.9ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 10.2ms
Speed: 2.0ms preprocess, 10.2ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 6.6ms
Speed: 1.5ms preprocess, 6.6ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 8.7ms
Speed: 2.1ms preprocess, 8.7ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 7.6ms
Speed: 1.7ms preprocess, 7.6ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 8.8ms
Speed: 2.2ms preprocess, 8.8ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 7.4ms
Speed: 2.5ms preprocess, 7.4ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 2 Potholes, 8.9ms
Speed: 2.4ms preprocess, 8.9ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 6.7ms
Speed: 4.0ms preprocess, 6.7ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 7.4ms
Speed: 1.8ms preprocess, 7.4ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 7.1ms
Speed: 2.1ms preprocess, 7.1ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 9.1ms
Speed: 2.6ms preprocess, 9.1ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 8.0ms
Speed: 2.2ms preprocess, 8.0ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 11.1ms
Speed: 2.6ms preprocess, 11.1ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 7.5ms
Speed: 2.1ms preprocess, 7.5ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 7.1ms
Speed: 2.3ms preprocess, 7.1ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 6.8ms
Speed: 1.7ms preprocess, 6.8ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 2 Potholes, 9.7ms
Speed: 9.5ms preprocess, 9.7ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 2 Potholes, 9.3ms
Speed: 2.0ms preprocess, 9.3ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 2 Potholes, 9.6ms
Speed: 2.1ms preprocess, 9.6ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 2 Potholes, 9.8ms
Speed: 3.1ms preprocess, 9.8ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 2 Potholes, 13.4ms
Speed: 2.9ms preprocess, 13.4ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 2 Potholes, 6.7ms
Speed: 1.7ms preprocess, 6.7ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 7.3ms
Speed: 2.1ms preprocess, 7.3ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 2 Potholes, 7.1ms
Speed: 2.2ms preprocess, 7.1ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 1 Pothole, 13.1ms
Speed: 2.6ms preprocess, 13.1ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 1 Pothole, 12.5ms
Speed: 2.1ms preprocess, 12.5ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 13.6ms
Speed: 2.1ms preprocess, 13.6ms inference, 1.8ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 6.9ms
Speed: 2.5ms preprocess, 6.9ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 2 Potholes, 9.8ms
Speed: 2.1ms preprocess, 9.8ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 7.7ms
Speed: 2.1ms preprocess, 7.7ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 7.1ms
Speed: 2.0ms preprocess, 7.1ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 7.8ms
Speed: 2.6ms preprocess, 7.8ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 6.6ms
Speed: 1.7ms preprocess, 6.6ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 7.3ms
Speed: 2.2ms preprocess, 7.3ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 7.4ms
Speed: 2.1ms preprocess, 7.4ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 10.1ms
Speed: 2.2ms preprocess, 10.1ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 16.9ms
Speed: 2.9ms preprocess, 16.9ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 11.7ms
Speed: 2.8ms preprocess, 11.7ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 10.4ms
Speed: 2.6ms preprocess, 10.4ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 12.5ms
Speed: 4.8ms preprocess, 12.5ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 7.2ms
Speed: 2.1ms preprocess, 7.2ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 7.0ms
Speed: 2.0ms preprocess, 7.0ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 13.4ms
Speed: 2.2ms preprocess, 13.4ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 6.9ms
Speed: 2.2ms preprocess, 6.9ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 7.1ms
Speed: 2.1ms preprocess, 7.1ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 7.0ms
Speed: 1.6ms preprocess, 7.0ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 9 Potholes, 7.5ms
Speed: 2.0ms preprocess, 7.5ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 10 Potholes, 6.8ms
Speed: 2.3ms preprocess, 6.8ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 8 Potholes, 6.9ms
Speed: 2.0ms preprocess, 6.9ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 7.3ms
Speed: 2.1ms preprocess, 7.3ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 8.5ms
Speed: 2.9ms preprocess, 8.5ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 8.7ms
Speed: 2.6ms preprocess, 8.7ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 10.2ms
Speed: 3.4ms preprocess, 10.2ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 7.3ms
Speed: 2.1ms preprocess, 7.3ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 11.3ms
Speed: 3.7ms preprocess, 11.3ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 11.9ms
Speed: 2.4ms preprocess, 11.9ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 7 Potholes, 11.1ms
Speed: 2.3ms preprocess, 11.1ms inference, 1.8ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 11.0ms
Speed: 3.5ms preprocess, 11.0ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 9.4ms
Speed: 2.9ms preprocess, 9.4ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 8.5ms
Speed: 2.5ms preprocess, 8.5ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 10.9ms
Speed: 2.4ms preprocess, 10.9ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 8.0ms
Speed: 2.2ms preprocess, 8.0ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 7.8ms
Speed: 2.2ms preprocess, 7.8ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 8.9ms
Speed: 2.4ms preprocess, 8.9ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 8.5ms
Speed: 2.2ms preprocess, 8.5ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 12.8ms
Speed: 2.2ms preprocess, 12.8ms inference, 2.0ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 16.9ms
Speed: 2.1ms preprocess, 16.9ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 9.8ms
Speed: 2.3ms preprocess, 9.8ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 8.2ms
Speed: 2.2ms preprocess, 8.2ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 8.3ms
Speed: 2.2ms preprocess, 8.3ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 9.2ms
Speed: 2.1ms preprocess, 9.2ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 10.2ms
Speed: 2.2ms preprocess, 10.2ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 7.5ms
Speed: 1.6ms preprocess, 7.5ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 12.0ms
Speed: 2.6ms preprocess, 12.0ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 9.8ms
Speed: 2.1ms preprocess, 9.8ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 11.4ms
Speed: 3.2ms preprocess, 11.4ms inference, 2.0ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 10.7ms
Speed: 3.2ms preprocess, 10.7ms inference, 1.8ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 5 Potholes, 7.2ms
Speed: 3.0ms preprocess, 7.2ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 7.8ms
Speed: 2.8ms preprocess, 7.8ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 6 Potholes, 8.6ms
Speed: 2.5ms preprocess, 8.6ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 2 Potholes, 7.0ms
Speed: 1.7ms preprocess, 7.0ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 4 Potholes, 7.9ms
Speed: 1.9ms preprocess, 7.9ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 2 Potholes, 7.2ms
Speed: 1.8ms preprocess, 7.2ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 7.1ms
Speed: 2.0ms preprocess, 7.1ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 2 Potholes, 6.8ms
Speed: 1.6ms preprocess, 6.8ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 8.4ms
Speed: 2.0ms preprocess, 8.4ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 2 Potholes, 7.1ms
Speed: 1.8ms preprocess, 7.1ms inference, 3.1ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 8.4ms
Speed: 2.4ms preprocess, 8.4ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 2 Potholes, 7.3ms
Speed: 2.1ms preprocess, 7.3ms inference, 2.0ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 2 Potholes, 8.9ms
Speed: 2.1ms preprocess, 8.9ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 2 Potholes, 7.6ms
Speed: 2.2ms preprocess, 7.6ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 2 Potholes, 9.0ms
Speed: 1.9ms preprocess, 9.0ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 2 Potholes, 16.8ms
Speed: 2.8ms preprocess, 16.8ms inference, 1.8ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 2 Potholes, 14.4ms
Speed: 2.1ms preprocess, 14.4ms inference, 1.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 16.2ms
Speed: 2.1ms preprocess, 16.2ms inference, 1.7ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 9.2ms
Speed: 2.3ms preprocess, 9.2ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 13.3ms
Speed: 2.0ms preprocess, 13.3ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 6.6ms
Speed: 1.7ms preprocess, 6.6ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 (no detections), 7.5ms
Speed: 2.5ms preprocess, 7.5ms inference, 0.6ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 2 Potholes, 7.6ms
Speed: 2.2ms preprocess, 7.6ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 2 Potholes, 12.5ms
Speed: 2.3ms preprocess, 12.5ms inference, 1.4ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 2 Potholes, 6.7ms
Speed: 1.7ms preprocess, 6.7ms inference, 1.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 10.3ms
Speed: 2.2ms preprocess, 10.3ms inference, 3.2ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 1 Pothole, 7.1ms
Speed: 2.1ms preprocess, 7.1ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 3 Potholes, 12.5ms
Speed: 2.1ms preprocess, 12.5ms inference, 1.9ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 2 Potholes, 7.9ms
Speed: 2.0ms preprocess, 7.9ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 1 Pothole, 8.9ms
Speed: 2.1ms preprocess, 8.9ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 2 Potholes, 11.2ms
Speed: 2.6ms preprocess, 11.2ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 2 Potholes, 6.7ms
Speed: 2.4ms preprocess, 6.7ms inference, 1.5ms postprocess per image at shape (1, 3, 384, 640)

0: 384x640 2 Potholes, 6.9ms
Speed: 2.4ms preprocess, 6.9ms inference, 1.3ms postprocess per image at shape (1, 3, 384, 640)
Output video exists: True
Output video size: 27223070 bytes

```

```
<IPython.core.display.Video object>
```

```
<Figure size 1800x600 with 2 Axes>
```