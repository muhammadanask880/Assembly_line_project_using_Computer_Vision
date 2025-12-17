# 🏭 Assembly Line Packaging Analysis (Google Colab)

This repository contains an **Assembly Line analysis project** focused on monitoring and validating **packaging steps** in a production workflow using a structured, notebook-based pipeline.

The project is intentionally built to run on **Google Colab** and works with data that is **provided externally via a downloadable link**.

---

## ✨ What This Project Is About

This is an **Assembly Line Packaging Analysis project** that works with **video-based production data**.

In this project:

* I provide a **packaging line video** that can be used for testing and analysis
* Each video frame is **captured and labeled** using **Label Studio**
* Labels represent critical packaging states in the assembly line

The core focus is on tracking and validating **three key packaging stages**:

1. **Empty** – container/unit before filling
2. **Put** – product placed or filling in progress
3. **Full** – container/unit completely filled and ready

All required data (videos, frames, labels, and related files) are **already prepared and shared via a Drive link**.

---

## 🧠 What This Project Shows You

* How an assembly line **video** can be converted into frame-level data
* How each frame is **manually labeled** (Empty / Put / Full) using **Label Studio**
* How labeled frames are processed programmatically
* Validation of correct packaging state transitions
* Detection of missing or incorrect packaging steps
* A reproducible workflow for **video-based manufacturing analytics**

---

## 📌 Prerequisites

Before starting, make sure you have:

* A **Google account**
* Access to **Google Drive**
* A **data download link provided by me**
* Basic familiarity with Google Colab

No local setup is required.

---

## ▶️ How to Run This Project (Google Colab)

### 1️⃣ Open the Notebook in Google Colab

* Go to **Google Colab**
* Click **File → Open notebook**
* Open via **GitHub** or upload the notebook manually

---

### 2️⃣ Mount Google Drive

```python
from google.colab import drive
drive.mount('/content/drive')
```

Grant permissions when prompted.

---

### 3️⃣ Download Data & Upload to Google Drive

All required data is provided via the following Google Drive link:

🔗 **Data Link:**
[https://drive.google.com/drive/folders/1iCYJwMGwTm0qipXoAdWibpsSS57RvF_q?usp=sharing](https://drive.google.com/drive/folders/1iCYJwMGwTm0qipXoAdWibpsSS57RvF_q?usp=sharing)

This link contains:

* Raw assembly line video(s)
* Extracted video frames
* Frame-level labels created using **Label Studio**
* Supporting metadata and files

**Steps:**

1. Download the entire folder from the link above
2. Upload the folder to your **Google Drive**
3. Keep the folder structure **exactly the same**

Example Drive path:

```python
data_path = '/content/drive/MyDrive/assembly_line_data'
```

📌 **Important:**

* Do **not** rename files or folders
* Do **not** modify internal structure
* Upload everything **as-is**

---

### 4️⃣ Install Required Libraries

All required dependencies are installed inside the notebook.

```python
pip install -r requirements.txt
```

---

### 5️⃣ Run the Notebook

Run cells **top to bottom**:

* Use **Runtime → Run all**
* Or execute step-by-step to understand each stage

The notebook will process the assembly line data and generate results automatically.

---

## 📂 Outputs

The notebook generates structured outputs such as:

* Processed assembly line records
* Step-level summaries (Empty / Put / Full)
* Validation results for packaging flow
* Logs or intermediate artifacts (if enabled)

Outputs are saved directly to **Google Drive**.

---

## 🧪 Recommended Usage

* Use **High-RAM runtime** for larger datasets
* Keep raw data unchanged for reproducibility
* Rerun the notebook if new assembly line data is added

---

## 🏗️ Use Cases

* Assembly line monitoring
* Packaging process validation
* Manufacturing quality checks
* Process analytics & experimentation

---

## 📜 License

This project is released under the **MIT License**.

---

## 💬 Final Note

This repository is designed as a **practical assembly line analytics example**, showing how packaging steps can be captured, validated, and analyzed using a clean Google Colab workflow.

Just upload the data, run the notebook, and explore the results 🚀
