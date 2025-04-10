
```markdown
# 🎥 Azure End-to-End Data Engineering Project — Netflix Dataset (2025 Ready)


## 📁 Project Files

- `1_Autloader.ipynb`: Auto Loader notebook for streaming file ingestion into the Bronze layer.
- `2_silver.ipynb`: Initial Silver layer transformation logic.
- `3_lookupNotebook.ipynb`: Parameterized lookup setup notebook.
- `4_Silver_Data_transformation.ipynb`: Silver layer advanced transformations and cleaning.
- `5_lookup Notebook.ipynb`: Duplicate/alternate lookup logic (backup/variant).
- `7_DLT_notebook.ipynb`: Delta Live Table creation and streaming logic with quality checks.
- `Untitled Notebook 2025-04-08 14_29_57.ipynb`: Miscellaneous notebook for quick testing.
- `Netflix Project.dbc`: Full Databricks archive containing all notebooks (for easy import).
- `pipeline1.zip`: Azure Data Factory pipeline export.
- `pipeline1_support_live.zip`: ADF support files for parameterized data movement.

---


---
## 🔧 Technologies Used

- **Azure Data Factory** – Web, Copy, and Lookup Activities
- **Azure Data Lake (Gen2)** – Bronze, Silver, and Gold data zones
- **Azure Databricks** – Notebooks, Widgets, Delta Tables, DLT
- **Delta Live Tables (DLT)** – Real-time streaming and quality checks
- **REST APIs & HTTP Connections** – Pulling metadata from GitHub
- **CSV Dataset** – Netflix titles data (Kaggle)

---

## 🚀 Key Technical Highlights

- **Azure Data Factory (ADF)**
  - Parameterized pipelines with dynamic inputs
  - Web activity, HTTP connectors, and REST API integration
  - Lookup + Copy activities for controlled pipeline flow

- **Azure Data Lake Storage Gen2**
  - Layered data architecture (Bronze, Silver, Gold)
  - Folder-based structured storage zones

- **Azure Databricks**
  - Auto Loader for streaming ingestion
  - Notebook-driven ETL and transformation logic
  - Widget-based parameterization for flexibility
  - Delta Table write operations with overwrite and append modes

- **Delta Live Tables (DLT)**
  - Real-time data streaming to Gold layer
  - Data quality rules for validation and filtering
  - Streaming table creation with schema enforcement

- **Additional Concepts**
  - Error handling & pipeline debugging in ADF
  - REST API calls for data and metadata pull
  - Use of variables, dictionaries, and control flow in notebooks

---
---

## 🧱 Architecture Overview

```bash
Data Ingestion (CSV + REST API)
        ↓
ADF Pipelines (Web, Copy, Lookup)
        ↓
Databricks Auto Loader (Streaming to Bronze)
        ↓
Delta Tables (Silver with transformation & validation)
        ↓
Delta Live Tables (Gold + Streaming + Quality Rules)
```

---

## 🚀 How to Run

1. **Clone this repo & unzip pipeline files**:
```bash
git clone https://github.com/your-username/azure-netflix-data-eng-2025.git
```

2. **Upload Notebooks**:
   - Import `Netflix Project.dbc` into your Databricks workspace.
   - Or manually upload `.ipynb` notebooks.

3. **Upload Pipelines to Azure Data Factory**:
   - Unzip `pipeline1.zip` and import JSON files into ADF.
   - Set up linked services and datasets using parameterized paths.

4. **Create Storage Containers**:
   - Create `bronze/`, `silver/`, and `gold/` folders in your Data Lake Storage Gen2.

5. **Run Auto Loader Notebook**:
   - Configure widget values (like path and table names).
   - Run streaming job for real-time ingestion.

6. **Run Silver/Gold Notebooks**:
   - Clean and transform data.
   - Load into Delta tables and DLT.

---

## 📊 Features

- ✅ Real-time file ingestion using Auto Loader
- 🛠️ Parameterized pipelines for flexible config
- 📈 Streaming analytics using Delta Live Tables
- 🧪 Data quality checks and conditional filtering
- 🧠 Job-interview-ready skillset with modern tooling

---

## 📸 Demo Screenshots
![image](https://github.com/user-attachments/assets/936af19e-96fb-4fe5-a1bb-dfa1299d4205)

![image](https://github.com/user-attachments/assets/a0417aa1-8933-43a7-84e8-c4d938f1a4eb)

![image](https://github.com/user-attachments/assets/4c284d54-bc8c-413d-97c5-0ff87443e565)

![image](https://github.com/user-attachments/assets/0d0bcfde-d11c-4047-b53f-005aa7ad4a0e)

![image](https://github.com/user-attachments/assets/8ca9ed01-79ca-4d68-9009-40293f9b6217)


![image](https://github.com/user-attachments/assets/721df1fb-af0f-4cf4-a1ca-36cf39a9b1af)

---

## 🧾 Credits

Ansh Lamba
https://github.com/anshlambagit/Netflix_Azure_Data_Engineering_Project/tree/main/RawData_AND_Notebooks
---

## 📜 License

This project is licensed under the MIT License.

---

## ✨ Happy Learning & Building Data Pipelines!
```

