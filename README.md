# 📦 AI-Driven Supply Chain Data Analysis Project

This project demonstrates how to automate and analyze supply chain data using modern AI tools like [n8n](https://n8n.io/) for workflow automation and [Quadratic](https://www.quadratichq.com/) for intelligent spreadsheet-based analytics. I created the full pipeline with real-world use cases.


## 🔧 Tools & Technologies

-  **n8n** – for automated email monitoring and CSV extraction  
-  **PostgreSQL** – as the primary data store  
-  **Quadratic** – AI-powered spreadsheet for data analysis  
-  **CSV** – input format for sales data  
- 📊 **KPIs** – line fill rate, volume fill rate, on-time delivery  


##  Use Case: Atlique Mart (Organic Foods)

**Problem:** Inefficient order and inventory management  
**Solution:** Automated data ingestion + AI-driven analysis to track and improve fulfillment metrics



##  Data Flow & Architecture

1. Sales data received as email attachments (India & USA)
2. `n8n`:
   - Monitors Gmail inbox
   - Extracts CSVs
   - Converts them to JSON
   - Pushes to PostgreSQL
3. `Quadratic`:
   - Connects to Postgres
   - Uses prompts + functions to generate KPIs & charts


##  Key Learnings

- Automating daily ingestion & cleaning improves efficiency
- Using AI tools like Quadratic accelerates insight generation
- Date formatting & dimensional modeling are key to accuracy



##  Getting Started

1. Clone the repo
2. Configure your n8n workflow using provided JSON
3. Set up PostgreSQL tables (`sales`, `order_lines`)
4. Connect Quadratic to your DB
5. Start analyzing!

## N8N and Dashboards

<img width="1086" alt="image" src="https://github.com/user-attachments/assets/5537613a-1b40-40dc-a85e-af321e30dc89" />

<img width="787" alt="image" src="https://github.com/user-attachments/assets/07ec5620-d9d3-4115-bede-c1c16fa8e39a" />



##  Reference

Inspired by: [Supply Chain Analytics](https://www.youtube.com/watch?v=PglKAYgRdJ4&t=710s)

---
