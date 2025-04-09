## 🚘 Question 9 - Brand Popularity in Car Purchase Network

### ❓ Question:
کدام برندهای خودرو در شبکه توزیع خرید و پیشنهادات مشتریان بیشترین حضور را دارند؟  
**Which car brands are most central and frequently involved in customer purchase and recommendation networks?**

---

### 📦 Dataset:
`a2-ECDS4-CarSales (Car_Sales_Report)`

📌 تحلیل تراکنش‌ها برای شناسایی برندهای پرفروش و ساخت شبکه‌ای از ارتباط بین خودروها و برندها

---

### 💡 Use Case:
برای نمایندگی‌های فروش، نمایشگاه‌های خودرو و سرمایه‌گذاران جهت:
- تمرکز روی برندهای محبوب بازار
- پیش‌بینی روند فروش آینده
- طراحی پیشنهادات هدفمند بر اساس شبکه‌ی خرید واقعی مشتریان

---

### 🧠 Network Design

**🔵 Nodes:**
- `Car_id`: شناسه تراکنش هر خودرو (طیف رنگی بنفش)
- `Company`: برند تولیدکننده خودرو (رنگ سبز)

**🔗 Edges:**
- اتصال بین تراکنش (خودرو) و برند
- وزن یال = تعداد تراکنش‌های برند
- اندازه گره‌ها = درجه مرکزی بودن (Degree Centrality)

---

### 📷 Network Visualizations

<div align="center">
  <img src="./9-1.png" width="420" title="Brand Centrality in Network">
  <img src="./9-2.png" width="420" title="Brand Clustering View">
</div>

---

### 📁 Included Files

| File Name     | Description                                               |
|---------------|-----------------------------------------------------------|
| `9.gephi`     | Gephi project file for interactive network visualization |
| `nodes.csv`   | Node data (brands and transactions)                       |
| `edges.csv`   | Edge list between brands and sold vehicles                |
| `9-1.png`     | Graph view highlighting brand centrality (degree-based)   |
| `9-2.png`     | Clustered view of brands and network structure            |

---

### ✅ Key Insights:
- برندهایی با Degree بالا در مرکز شبکه فروش قرار دارند
- شناسایی برندهای پرتراکنش برای طراحی تبلیغات مؤثر
- ساختار گراف به تفکیک برندهای محبوب، ناحیه‌ای یا تخصصی کمک می‌کند

> 📌 *این تحلیل راهی داده‌محور برای اولویت‌بندی برندها و بهینه‌سازی تصمیمات فروش در صنعت خودرو فراهم می‌سازد.*
