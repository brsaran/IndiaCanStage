# India-Can-Stage

**India-Can-Stage** is a low-resource oriented digital cancer staging platform developed to support standardized cancer staging for **hospital-based and population-based cancer registries** and to aid **clinical decision-making** in India and similar LMIC settings.

The tool implements **deterministic, rule-based staging logic** derived from **AJCC 8th and 9th edition guidelines** and enables automated derivation of multiple staging systems from structured clinical inputs.

---

## Key Features

- **Supports 44 cancer sites** relevant to Indian cancer registries
- **Single data entry** generates staging outputs for both **AJCC 8th and 9th editions**
- Generates:
  - **AJCC TNM**
  - **AJCC Composite Stage Group**
  - **Essential TNM (ETNM)**
  - **SEER Summary Stage (SSS)**
- **Rule-based deterministic engine** ensuring reproducible and auditable results
- **Built-in validation** to prevent invalid or unrealistic TNM combinations
- Incorporates **AJCC-defined site-specific prognostic variables**, including:
  - **Age** (thyroid cancer)
  - **PSA** (prostate cancer)
  - **Tumor grade** (appendix, prostate, bone)
  - **Serum markers** such as **LDH, AFP, and hCG** (testicular cancer)
- Designed for **low-resource settings** with incomplete clinical documentation
- **Modular architecture** enabling easy updates for future AJCC revisions

---

## System Architecture

- **Backend**: Python 3.12–based modular rule engine
- **Frontend**: Streamlit-based interactive interface
- **Logic Layer**: Site-specific AJCC rule matrices
- **Output**: Structured **JSON** for interoperability

The architecture ensures **transparency, traceability, and scalability**, enabling deployment across hospitals, registries, and academic institutions.

---

## Web Application

A fully functional web deployment of **India-Can-Stage** is currently available.

**India-Can-Stage Web Application:**  
Access the webversion here [India-can-Stage](http://103.154.184.110:8501/). The production system is centrally hosted on secure **ICMR-NCDIR servers** to ensure controlled access, centralized version management, and uniform updates.

---

## API and Standalone Deployment

- **Authenticated API endpoints** are available for integration with:
  - Hospital Information Systems (HIS)
  - Electronic Health Records (EHR)
  - Cancer registry software
- **Standalone offline deployment** and **public API documentation** will be updated soon

These deployment options support district hospitals, medical colleges, and registry environments with limited infrastructure.

---

## Intended Users

- **Hospital-Based Cancer Registries (HBCR)**
- **Population-Based Cancer Registries (PBCR)**
- **Clinicians and oncology care teams**
- **Public health researchers**
- **Digital health and registry software developers**

---

## Use Cases

- **Standardized cancer staging** at the point of care
- **Mapping TNM data** to SEER Summary Stage for population-based reporting
- **Improving completeness and consistency** of registry staging data
- **Supporting clinical decision-making** and multidisciplinary discussions
- **Enabling interoperable cancer data workflows**

---

## Project Status and Roadmap

- **Rule engine implemented and validated** against AJCC staging logic
- **Web-based application operational**
- **Standalone version** release planned
- **API documentation and integration examples** to be released soon

---

## Related Publication

**India-Can-Stage: Development of a Low Resource-Oriented Cancer Staging Tool to Support Cancer Registries and Clinical Decision-Making**  
Manuscript under review

---

## Acknowledgements

Developed under the guidance of the **Indian Council of Medical Research – National Centre for Disease Informatics and Research (ICMR-NCDIR)**, with framework guidance drawn from the **International Agency for Research on Cancer (IARC)** CanStaging initiative  (https://github.com/IARC-CSU/CanStaging),  to strengthen standardized cancer staging, registry data quality, and digital oncology infrastructure in low-resource settings.
