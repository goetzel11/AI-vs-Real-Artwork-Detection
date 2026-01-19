<div align="center">
  <img src="trueorigin.jpeg" alt="TrueOrigin Logo" width="200" style="margin-bottom: 0px;">
  <h1 style="margin-top: 0px;">TrueOrigin</h1>
  <p><i>AI vs Real Artwork Detection System</i></p>

  <a href="https://huggingface.co/spaces/goetzel11/TrueOrigin"><img src="https://img.shields.io/badge/Demo-HuggingFace-yellow?style=for-the-badge&logo=huggingface" alt="HuggingFace Space"></a>
  <img src="https://img.shields.io/badge/Python-3.9%2B-blue?style=for-the-badge&logo=python" alt="Python Version">
  <img src="https://img.shields.io/badge/Framework-TensorFlow-orange?style=for-the-badge&logo=tensorflow" alt="TensorFlow">
</div>

---

## 📖 Overview

**TrueOrigin** adalah solusi teknologi berbasis Computer Vision yang dirancang untuk mendeteksi apakah sebuah karya seni merupakan hasil buatan manusia atau *Generative AI*.

Tool ini dikembangkan khusus untuk membantu organisasi atau penyelenggara kompetisi seni dalam melakukan **filtrasi awal (early filtering)**. Dengan menggunakan arsitektur **MobileNetV2** yang dioptimasi, TrueOrigin membantu juri menyaring karya yang masuk sebelum tahap kurasi mendalam, meminimalkan kecurangan, dan menjaga integritas kompetisi seni.

## 🚩 Problem Statement

Maraknya *Generative AI* menciptakan tantangan baru dalam dunia seni:
1.  **Ambiguitas Visual:** Karya digital modern makin sulit dibedakan dengan karya AI secara kasat mata.
2.  **Integritas Kompetisi:** Risiko lolosnya karya AI di kategori non-AI (*False Negative*) dapat merusak kredibilitas lomba.
3.  **Inefisiensi:** Memeriksa ribuan karya secara manual memakan waktu dan sumber daya yang sangat besar.

> **Solusi Kami:** TrueOrigin hadir sebagai "gatekeeper" cerdas yang memprioritaskan deteksi karya berpotensi AI, sehingga verifikasi manusia bisa lebih fokus dan efisien.

## 🎯 Key Objectives

* ✅ **High-Volume Filtering:** Menyaring ribuan karya visual secara cepat.
* ✅ **Minimize False Negatives:** Fokus pada pendeteksian AI agar tidak ada karya 'palsu' yang lolos ke tahap final.
* ✅ **Efficient Workflow:** Mengarahkan karya yang terindikasi AI untuk pemeriksaan lanjutan, mengurangi beban kerja manual reviewer.

## 💾 Dataset

Dataset yang digunakan bersumber dari Kaggle dan gabungan sumber publik lainnya:
* **Sumber:** [Kaggle - AI and Human Art Classification](https://www.kaggle.com/datasets/kausthubkannan/ai-and-human-art-classification/discussion/479343)
* **Komposisi:** Campuran dataset HuggingFace, Pinterest, dan koleksi publik lainnya.

## 🛠️ Tech Stack

Proyek ini dibangun menggunakan ekosistem Python yang kuat:

**Core & Deep Learning**
![TensorFlow](https://img.shields.io/badge/TensorFlow-%23FF6F00.svg?style=flat&logo=TensorFlow&logoColor=white)
![Keras](https://img.shields.io/badge/Keras-%23D00000.svg?style=flat&logo=Keras&logoColor=white)
![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=flat&logo=numpy&logoColor=white)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=flat&logo=pandas&logoColor=white)

**Computer Vision & Processing**
![OpenCV](https://img.shields.io/badge/PIL-Python_Imaging-green?style=flat)
![MobileNetV2](https://img.shields.io/badge/Model-MobileNetV2-blue?style=flat)

**Deployment & Tools**
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat&logo=Streamlit&logoColor=white)
![HuggingFace](https://img.shields.io/badge/HuggingFace-yellow?style=flat&logo=huggingface&logoColor=black)
![VSCode](https://img.shields.io/badge/Visual%20Studio%20Code-0078d7.svg?style=flat&logo=visual-studio-code&logoColor=white)

## ⚙️ Methodology Pipeline

1.  **Data Acquisition**: Pengumpulan dataset (AI vs Non-AI).
2.  **Preprocessing**: Resize, Normalisasi, Augmentasi, dan Split Data.
3.  **Modeling**: Transfer Learning menggunakan **MobileNetV2** (Feature Extractor) + Custom Classification Head.
4.  **Evaluation**: Analisis Confusion Matrix & Classification Report.
5.  **Deployment**: Implementasi antarmuka pengguna dengan Streamlit.

## 📂 Project Structure

```text
├── deployment/              # File konfigurasi untuk deployment
├── EDA.ipynb                # Notebook untuk Exploratory Data Analysis
├── Model_Inference.ipynb    # Notebook pengujian model
├── Model_Training.ipynb     # Notebook pelatihan model utama
├── requirements.txt         # Daftar library yang dibutuhkan
└── README.md                # Dokumentasi proyek

``` 

## Team Members

<table align="center">
  <tr>
    <td align="center" width="220">
      <img src="https://github.com/UngiiiKiat.png" width="110" height="110" style="border-radius: 50%;" />
      <h3>Rangga Irwanto Putra Kiat</h3>     
      <p><b>Role:</b> Data Analyst</p>
      <a href="https://github.com/UngiiiKiat">GitHub</a> • 
      <a href="www.linkedin.com/in/rangga-kiat">LinkedIn</a>
    </td>

   <td align="center" width="220">
      <img src="https://github.com/afzanurhakim.png" width="110" height="110" style="border-radius: 50%;" />
      <h3>Muhammad Afza Nur Hakim</h3>
      <p><b>Role:</b> Data Scientist</p>
      <a href="https://github.com/afzanurhakim">GitHub</a> • 
      <a href="https://www.linkedin.com/in/LINKEDIN2/">LinkedIn</a>
    </td>

   <td align="center" width="220">
      <img src="https://github.com/Ghulaaaam.png" width="110" height="110" style="border-radius: 50%;" />
      <h3>Achmad Ghulam Habib Al-widani</h3>
      <p><b>Role:</b> Data Scientist</p>
      <a href="https://github.com/Ghulaaaam">GitHub</a> • 
      <a href="https://www.linkedin.com/in/LINKEDIN3/">LinkedIn</a>
    </td>

   <td align="center" width="220">
      <img src="https://github.com/goetzel11.png" width="110" height="110" style="border-radius: 50%;" />
      <h3>Muhammad Aldzahabi Mawarid</h3>
      <p><b>Role:</b> Data Engineering</p>
      <a href="https://github.com/goetzel11">GitHub</a> • 
      <a href="https://www.linkedin.com/in/LINKEDIN4/">LinkedIn</a>
    </td>
  </tr>
</table>

<div align="center"> <p>Made with ❤️ by TrueOrigin Team</p> </div>