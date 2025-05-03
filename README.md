# Surveillex

**Surveillex** is a video anomaly detection system developed using the ShanghaiTech Campus Surveillance Dataset. It is designed to detect unusual or suspicious activities in surveillance videos using deep learning techniques.

---

## 📁 Dataset Setup

1. **Download the Dataset**  
   Get the dataset from this link: [ShanghaiTech Dataset](https://drive.google.com/file/d/1EJQ8h1LkzD4kPZ9V9e8z7e8z7e8z7e8/view?usp=sharing)

2. **Extract and Organize**  
   - Unzip the downloaded files.
   - Move the `list` directory into the root of this repository.

---

## 🧪 Usage

You can use the `ShanghaiDataset` class to load the dataset for training and testing.

```python
from dataset import ShanghaiDataset

# Load normal training data
normal_train_dataset = ShanghaiDataset(train=True, is_normal=True, transform=None)

# Load abnormal training data
abnormal_train_dataset = ShanghaiDataset(train=True, is_normal=False, transform=None)

# Load test data
test_dataset = ShanghaiDataset(train=False, transform=None)
