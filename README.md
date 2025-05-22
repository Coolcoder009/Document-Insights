# 📊 Document Insights Generator

A powerful web app that lets users upload documents (PDFs, CSVs, Excels) and automatically extract actionable insights based on **custom KPIs** using **Claude AI**.

---

## 🚀 Features

- ✅ Upload multiple documents (`.pdf`, `.csv`, `.xls`, `.xlsx`)
- ✅ Add unlimited custom KPIs (Key Performance Indicators)
- ✅ Automatically extract content from:
  - PDFs using `PyPDF2`
  - CSV/Excel using `pandas`
- ✅ Claude AI-powered insight generation per KPI
- ✅ User-friendly frontend to view document-wise insights
- ✅ FastAPI backend with Claude integration

---

## 🧠 How It Works

1. **User uploads documents** via the frontend.
2. **User enters KPIs** like "Revenue", "Profit", "Expenses", etc.
3. **Backend processes** each document:
   - PDFs → text extracted using `PyPDF2`
   - Excel/CSV → relevant data filtered using `pandas`
4. **Claude AI** analyzes the extracted content and generates a short insight per KPI.
5. Results are returned and **rendered in a dynamic table** on the frontend.

---

## 🖥 Tech Stack

| Layer       | Tech                  |
|-------------|-----------------------|
| Frontend    | HTML, JavaScript      |
| Backend     | FastAPI (Python)      |
| AI Engine   | Claude AI (`anthropic`) |
| Parsing     | `PyPDF2`, `pandas`    |
| Hosting     | Hetzner               |

---

## 🔧 Setup Instructions

### 1. Clone the Repo

```bash
git clone https://github.com/Coolcoder009/Document-Insights-backend.git
cd Document-Insights-backend
```
### 2. Starting the app
```bash
uvicorn main:app --reload
```
