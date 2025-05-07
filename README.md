# HW3 - Instance Segmentation with Mask R-CNN

This project implements an instance segmentation pipeline using Mask R-CNN with a ResNet-50 backbone for detecting and segmenting individual cells in microscopy images. It was developed in a single Python notebook for Homework 3 of the NYCU course *Visual Recognition using Deep Learning (Spring 2025)*.

---

## 📁 Folder Structure

Your working directory should look like this:

```
HW3/
├── HW3_code.ipynb
├── utils.py
├── hw3-data-release/
│   ├── train/
│   ├── test_release/
│   └── test_image_name_to_ids.json

```

---

## Set up

### 1. Clone the repository

```bash
git clone https://github.com/mariep00/535521-HW3.git
cd 535521-HW3
```

### 2. Set up the environment

Use Python 3.9 or higher. You can install the dependencies using pip:

```bash
pip install -r requirements.txt
```


---

## 📂 Where to Change the Path 

You should update the paths inside the notebook to match the path of your folder.

Under "Load the data and change the paths HERE":

```python
# Define paths
archive_path = "/<pathtothefolder>/HW3/hw3-data-release.tar.gz"
extract_dir = "/<pathtothefolder>/HW3/hw3-data-release"  # target folder

```

---

## Submission

After running inference, a results file is generated:

```
test-results.json
```

---

## 📊 Evaluation

- `AP50` (IoU ≥ 0.5) is the main metric from codabench

- Here a snapshot of the competion result:

<img width="1053" alt="Screenshot 2025-05-07 at 23 49 28" src="https://github.com/user-attachments/assets/0b4a1ac6-d9c7-4115-8b07-482a94c895d8" />

---

## 📚 References

- [Mask R-CNN](https://arxiv.org/abs/1703.06870)
- [COCO Dataset Format](https://cocodataset.org/#format-results)
- [PyTorch ReduceLROnPlateau](https://pytorch.org/docs/stable/generated/torch.optim.lr_scheduler.ReduceLROnPlateau.html)

---

## ✍️ Author

Marie P.  
Student ID: 313551818  
NYCU Spring 2025  

