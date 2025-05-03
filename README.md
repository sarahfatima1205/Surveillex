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

⚙️ Installation
Clone the Repository

bash
Copy
Edit
git clone https://github.com/sarahfatima1205/Surveillex.git
cd Surveillex
Install Dependencies

Make sure Python 3.6+ is installed. Then, install the required packages:

bash
Copy
Edit
pip install -r requirements.txt
🧠 Model Overview
Surveillex uses a deep learning model for temporal and spatial feature extraction from video sequences to identify anomalies effectively. More details on the architecture will be added soon.

🚀 Running the Project
Prepare the dataset as outlined in the Dataset Setup section.

Train the model:

bash
Copy
Edit
python train.py
Evaluate the model:

bash
Copy
Edit
python evaluate.py
Note: Replace script names as per your actual file names if different.

📂 Project Structure
bash
Copy
Edit
Surveillex/
├── checkpoints/        # Saved model checkpoints
├── list/               # Dataset list directory
├── results/            # Evaluation outputs
├── src/                # Core source code
├── dataset.py          # Custom dataset script
├── requirements.txt    # Python dependencies
└── README.md           # Project documentation
📊 Results
Evaluation metrics and visualizations will be added in upcoming updates.

🤝 Contributing
Pull requests are welcome! For major changes, please open an issue first to discuss your ideas.

📄 License
This project is licensed under the MIT License - see the LICENSE file for details.

📬 Contact
For questions or feedback, feel free to reach out to @sarahfatima1205.

vbnet
Copy
Edit

Let me know if you'd like help auto-generating badges (build status, license, etc.) for the top of the README.







