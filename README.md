QUERY DOCUMENT- Databricks Project

Here’s a more detailed and easy-to-follow rewrite of your project explanation, with tables to make the structure clearer:

---

#### Ecommerce Project with Medallion Architecture

I designed an **ecommerce data pipeline** using the **Medallion Architecture** in Databricks. The project is organized into three layers:

### 🏗️ Medallion Layers

| Layer   | Purpose | Data State |
|---------|---------|------------|
| **Bronze** | Stores raw data exactly as received from the source | Unprocessed, messy |
| **Silver** | Cleans and transforms the raw data | Structured, consistent |
| **Gold** | Provides analytics-ready data for reporting and dashboards | Optimized, aggregated |

---

### 📂 Dataset Structure

The dataset is divided into six folders:

| Table Type | Tables |
|------------|--------|
| **Fact Table** | order_items |
| **Dimension Tables** | brands, category, customers, date, products |

- **Fact Table (order_items):** Contains transactional data (e.g., purchases, quantities, amounts).  
- **Dimension Tables:** Provide descriptive context (e.g., product details, customer info, categories, brands, dates).

---

### 🔄 Data Flow

1. **Source Layer:** Raw data is kept in the source folders.  
2. **Bronze Layer:** Raw data ingested into Databricks.  
3. **Silver Layer:** Data cleaned, standardized, and transformed (handling duplicates, fixing formats, etc.).  
4. **Gold Layer:** Final curated data prepared for analytics and BI.  

---

### 📊 BI Dashboard

Using the **Gold Layer data**, I built a **Business Intelligence dashboard in Databricks**.  
- The dashboard visualizes ecommerce trends such as **sales by category, top products, customer behavior, and revenue growth**.  
- This makes it easier for stakeholders to make **data-driven decisions**.

---

👉 In simple terms:  
Think of the Bronze layer as the **raw ingredients**, the Silver layer as the **cooked meal**, and the Gold layer as the **beautifully plated dish ready to serve**. The BI dashboard is like the **menu card** that shows the final results in a way everyone can understand.

---

Would you like me to also sketch out a **sample dashboard layout** (like KPIs, charts, and filters you could include) so it feels more concrete and presentation-ready?
