# 🤖 AI Preprocessing | Fast-moving Consumer Goods

### Perform data preprocessing activities (normalization, cleaning etc.) using AI Tools for business/data analytics team working with an FMCG company.

## 📌 Table of Contents
- <a href="#overview">Overview</a>
- <a href="#dataset">Dataset</a>
- <a href="#tools-technologies">Tools & Technologies</a>
- <a href="#project-structure">Project Structure</a>
- <a href="#data-preprocessing">Data Preproceessing</a>
- <a href="#credits">Credits</a>
- <a href="#author-contact">Author & Contact</a>

<h2><a class="anchor" id="overview"></a>📝 Overview</h2>

This project aims to utilize AI tools (ChatGPT, Google AI Mode) and perform different data preprocessing tasks such as normalization, cleaning and enrichment on raw data provided by FMCG Client.
- Review the raw data and understand metadata
- Use AI tools for data preprocessing and create a data model
- Enrich data with additional features (if possible)


<h2><a class="anchor" id="dataset"></a>📊 Dataset</h2>

`.xlsx` file located in `/data/raw` folder

![raw-dataset](https://github.com/gaurav-patil-git/04_AI_Preprocessing/blob/main/visuals/fmcg-raw-data.png)


<h2><a class="anchor" id="tools-technologies"></a>🛠️ Tools & Technologies</h2>

| Task                 | Tools Used                          |
|----------------------|-------------------------------------|
| Data Preprocessing   | Excel                               |
| ChatGPT         | AI Assistance                       |
| Google AI Mode    | Research                            |

<h2><a class="anchor" id="project-structure"></a>📁 Project Structure</h2>

```
04_AI_Preprocessing/
│
├── data/
│   ├── raw/               # Original, immutable data dumps
│   ├── processed/         # Cleaned & processed datasets
│
├── documents/             # Prompt bank
│
├── visuals/               # Screenshots
│
├── README.md              # High-level project overview
├── .gitignore             # Ignore data, models, logs if using Git

```

<h2><a class="anchor" id="data-preprocessing"></a>🧼 Data Preprocessing</h2>

### Step 1: Project Initialization
- Used **Prompt 1** to initiate the project within the ChatGPT environment.
- Used **Prompt 2** to generate the normalization action plan.

### Step 2: Data Staging and Preparation
- Injected/Staged raw data for normalization in **Power Query**.
- Started with **product-related dimension tables** by sorting rows according to category.

### Step 3: Product Dimension Tables
- Created `dim_category` and `dim_subcategory` tables.
- Identified that the `product` column contained the entire product name, including the brand name.
- Verified **product prices** for variance and confirmed no discrepancies.

### Step 4: Geography Dimension Tables
- Initiated work on **geography-related tables**.
- Created `dim_state`, `dim_city`, and `dim_store` tables.
- Identified opportunities to enrich data with **regions** and **tiers**.

### Step 5: Brand Name Extraction
- Sought approval from the **Sr. Data Scientist** and **Client** to implement AI for brand name extraction.
- Used **Prompt 3** to extract the full brand name from the product column.
- Incorporated an **Excel formula** to include brand names in the dataset.

### Step 6: Fact Table Creation
- Created the `fact_order` table to capture and consolidate order transactions.

### Step 7: Calendar Dimension Tables
- Created the `blank query` as placeholder.
- Used **Prompt 4** to generate Power Query M Code and create a calendar table.

### Step 8: Administrative Zone Binning
- Used **Prompt 5A** to research administrative regions of India.
- Used **Prompt 5B** to transform unstructured data into structured data.
- Enriched `dim_state` by enriching it with `zone` feature.

![final-model](https://github.com/gaurav-patil-git/04_AI_Preprocessing/blob/main/visuals/final-data-model.png)

<h2><a class="anchor" id="credits"></a>🪪 Credits</h2>

The dataset used for this project was taken from [_Get Super AI_](https://www.getsuper.ai/post/3-sales-data-analytics-project-ideas-for-your-resume).

<h2><a class="anchor" id="author-contact"></a>📝 Author & Contact</h2>

**Gaurav Patil** (Data Analyst) 
- 🔗 [LinkedIn](https://www.linkedin.com/in/gaurav-patil-in/)


