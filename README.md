# Image-Sharpening-using-Knowledge-Distillation
This project aims to enhance image clarity using a lightweight AI model designed for real-time video conferencing scenarios. A high-capacity teacher model (DnCNN) is used to distill knowledge into a compact student model, achieving high performance while maintaining fast inference.
## Files in the Repo

| File | Description |
| ---- | ----------- |

 `evaluate_student.py` --> Trains Teacher & Student models  
 `visualization.py` --> Loads models, visualizes output  
 `images/` --> Sample outputs for README
 `requirements.txt` --> Project Dependencies
 `.gitignore` –-> To ignore weights, cache, and environment folders
 `ssim_comparison_report.csv` –-> Example SSIM results
 `MOS.csv` –-> Example Mean Opinion Scores

## Performance

| Metric | Value |
| ------ | ----- |

SSIM (Teacher) --> 0.9367
SSIM (Student) --> 0.9207
Student vs Ground Truth --> 0.9264
FPS (CPU) --> ~13.64

## Dataset

- Dataset: `Helen` from [DBlur] https://www.kaggle.com/datasets/jishnuparayilshibu/a-curated-list-of-image-deblurring-datasets
- Used 1300 train / 165 validation / 165 test images
- Format: Paired `blur/` and `sharp/` folders

## How to Use

```bash
pip install -r requirements.txt
python evaluate_student.py
```

## Author

**Poojala Renuka**  
ECE Dept.,
GITAM Bengaluru
