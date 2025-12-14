# Deep-Image-Prior-for-Inverse-Problems-in-Imaging
A CNN-based Deep Image Prior framework for solving inverse problems in imaging, demonstrating dataset-free image restoration using PSNR and SSIM evaluation.


## Objectives
- To understand and implement the Deep Image Prior framework.
- To apply DIP for solving inverse imaging problems without pre-trained models.
- To evaluate restoration quality using standard image quality metrics.
- To analyze the effectiveness of CNN architecture as a natural image prior.

---

## Key Features
- Dataset-free image restoration approach  
- CNN-based implicit regularization  
- Supports multiple inverse imaging tasks  
- Evaluation using PSNR and SSIM metrics  
- Implemented using PyTorch and Python  

---

## Inverse Imaging Tasks Covered
- **Image Denoising** – Removing noise from corrupted images  
- **Image Inpainting** – Filling missing or masked regions  
- **Super-Resolution** – Enhancing image resolution  
- **Multimodal Image Fusion** – Combining information from multiple image sources  

---

## Technologies Used
- **Programming Language:** Python  
- **Framework:** PyTorch  
- **Libraries:** NumPy, OpenCV, Matplotlib, scikit-image  
- **Environment:** Google Colab / Jupyter Notebook  

---

## Project Structure
Deep-Image-Prior-for-Inverse-Problems-in-Imaging/
│
├── notebooks/
│ ├── dip_denoising.ipynb
│ ├── dip_inpainting.ipynb
│ └── dip_super_resolution.ipynb
│
├── data/
│ ├── input_images/
│ └── results/
│
├── models/
│ └── cnn_architecture.py
│
├── utils/
│ ├── metrics.py
│ └── helpers.py
│
├── README.md
└── requirements.txt

yaml
Copy code

---

## Methodology
1. Initialize a random noise input to the CNN.
2. Pass the noise through an untrained CNN architecture.
3. Optimize network parameters to minimize reconstruction loss.
4. Stop training early to avoid overfitting to noise.
5. Evaluate restored outputs using PSNR and SSIM metrics.

---

## Evaluation Metrics
- **PSNR (Peak Signal-to-Noise Ratio)**
- **SSIM (Structural Similarity Index Measure)**

These metrics are used to compare restored images with ground truth images.

---

## Results
The Deep Image Prior approach demonstrates effective image restoration across various inverse problems without requiring any external training data. Early stopping plays a crucial role in achieving optimal results by preventing the network from fitting noise.

---

## How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/Deep-Image-Prior-for-Inverse-Problems-in-Imaging.git
Install dependencies:

bash
Copy code
pip install -r requirements.txt
Open the notebooks in Jupyter or Google Colab and run the cells sequentially.

Applications
Medical imaging enhancement

Satellite and remote sensing image restoration

Surveillance and low-quality video enhancement

Scientific and industrial imaging

Future Work
Extend DIP to video restoration with temporal consistency

Experiment with different CNN architectures

Optimize performance for real-time applications

Compare DIP results with supervised learning methods

References
Ulyanov, D., Vedaldi, A., & Lempitsky, V. (2018). Deep Image Prior.

Official Paper: https://arxiv.org/abs/1711.10925

Author
Keerthana H L
B.E. Computer Science (AI-ML)
GitHub: https://github.com/keerthanahl16

License
This project is intended for academic and educational purposes.

