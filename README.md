# Novel Deep Learning Architectures for Classification and Segmentation of Brain Tumors from MRI Images

## 📄 Abstract & Overview

This research paper introduces a **Computer-Aided Diagnosis (CAD)** system featuring two novel Deep Learning architectures, **SAETCN** and **SAS-Net**, designed to enhance the accuracy and efficiency of detecting, classifying, and segmenting brain tumors from **MRI images**. The models address the limitations of existing approaches, which often suffer from poor generalization and low validation performance, achieving state-of-the-art results on multiple datasets.

---

## 💡 Introduction to Brain Tumors

Brain tumors represent a significant health challenge, classified by their origin, aggressiveness, and location. Accurate and timely diagnosis is critical for effective treatment planning. The three most common types of brain tumors addressed by this study include:

* **Glioma:** These tumors arise from glial cells (supportive tissue of the brain and spinal cord). They are often highly aggressive and challenging to treat.
* **Meningioma:** These tumors originate in the meninges, the membranes that surround the brain and spinal cord. They are usually benign (non-cancerous) and slow-growing.
* **Pituitary:** These tumors develop in the pituitary gland, a small gland at the base of the brain. They are typically benign but can cause hormonal imbalances and vision problems due to compression.

The emergence of AI, particularly Deep Learning, offers a powerful tool to automate and improve the laborious process of tumor detection and characterization from medical images.

---

![Different Kinds of Brain Tumor](Visualisation/Different_Kinds_of_Brain_Tumors.jpg)
![Processflow Diagram for Brain Tumor Classification of Multiclass Dataset](Visualisation/Processflow_Diagram.jpg)


## 🧠 Proposed Novel Architectures

The framework is built upon the integration of **self-attention mechanisms** to facilitate robust and focused feature extraction in medical imaging data.

### 1. SAETCN (Self-Attention Enhancement Tumor Classification Network)

* **Task:** **Classification** of brain tumors into four categories: **Glioma, Meningioma, Pituitary, and No Tumor (Normal)**.
* **Core Structure:** A deep Convolutional Neural Network (CNN) that merges concepts from **Residual** and **Inception** networks.
* **Key Component:** The **Self Attention Enhancement Block (SAEB)**, which uses skip connections and parallel convolution branches to capture complex, multi-scale spatial features while maintaining efficient gradient flow.
* **Performance:** Achieved an impressive classification accuracy of **99.38%** on the validation dataset.

![SAETCN Architecture Diagram](Visualisation/SAETCN_Full_Architecture.jpg)

### 2. SAS-Net (Self-Attentive Segmentation Network)

* **Task:** **Segmentation** (precise pixel-wise delineation) of the tumor region within the brain MRI.
* **Key Component:** The **Segmental Feature Decoder Block (SFD Block)**, which serves as a decoder to enhance feature map resolution through sophisticated upsampling and feature integration.
* **Integration:** The SFD block contains a complex **Residual Inception module** to combine features at various scales effectively, leading to highly accurate boundary detection.
* **Performance:** Demonstrated an overall pixel accuracy of **99.23%**.

![SAS-Net Segmentation Result](Visualisation/SASNET_Full_Architecture.jpg)

---

## 💻 Technical Details

| Feature | Description |
| :--- | :--- |
| **Implementation** | The models were implemented using the **PyTorch** deep learning framework. |
| **Datasets** | Multiple datasets were used, including a combination of Figshare, SARTAJ, and Br35H for classification, and the **BratS2020** dataset for segmentation. |
| **Key Techniques** | Self-Attention, Residual Connections, Inception Modules. |
| **Evaluation Metrics** | Precision, F1 Score, Recall, ROC-AUC (for classification), and Intersection Over Union (IoU), Dice Similarity Coefficient (DSC), Boundary F1 Score (for segmentation). |

---

## 🔗 Repository and Software Links

The computational codes and model architectures are publicly available. The ultimate goal is to integrate these architectures into an accessible CAD system.

| Resource Type | Link |
| :--- | :--- |
| **Code Repository** | [SAETCN and SAS-NET Architectures (GitHub)](https://github.com/arghadip2002/SAETCN-and-SASNET-Architectures) |
| **Live Software Demo (NeuroGuard Web App)** | [NeuroGuard Web Application (Hugging Face Space)](https://huggingface.co/spaces/arghadip2002/NeuroGuard-Web-Application) |
| **Code Repo of NeuroGuard Web App** | [Github Repo](https://github.com/arghadip2002/NeuroGuard-Web-Application) |


---

## 👨‍💻 Authors

* **[Arghadip Biswas](https://github.com/arghadip2002)**
    * Affiliation: Jadavpur University, Kolkata, India
    * GitHub ID: `arghadip2002`
* **[Sayan Das](https://github.com/Necromancer0912)**
    * Affiliation: IIIT Delhi, Delhi, India
    * GitHub ID: `Necromancer0912`

---

## 📧 Contact

* **Email:** mrarghadipofficial@gmail.com
