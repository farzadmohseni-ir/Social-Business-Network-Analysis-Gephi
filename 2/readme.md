## 💳 Question 2 - Variation in Payment Methods by Time of Day

**Question:**  
آیا روش پرداخت مشتریان در ساعات مختلف روز تغییر می‌کند؟

**Dataset:**  
`a0-ECDSa16-ResturantSales`

**Use Case:**  
👨‍💼 مدیر رستوران یا تیم مالی برای بررسی نیاز به دستگاه‌های پرداخت بیشتر در ساعات اوج و بهینه‌سازی تجربه پرداخت.

---

### 🧠 Insights

- بررسی ارتباط بین نوع پرداخت (`transaction_type`) و زمان انجام آن (`time_of_sale`)
- شناسایی الگوهایی مثل اینکه پرداخت نقدی در شب رایج‌تر است یا کارت در ساعات ظهر
- قابلیت استفاده برای زمان‌بندی نیروی انسانی یا دستگاه‌های POS

---

### 🧾 Network Design

**🔵 Nodes:**  
- `transaction_type`: نوع پرداخت (نقدی، کارت، آنلاین و ...)
- `time_of_sale`: زمان روز (صبح، ظهر، عصر، شب)

**🔗 Edges:**  
- اتصال بین نوع پرداخت و ساعت، بر اساس تعداد تراکنش
- وزن یال‌ها: تعداد تراکنش‌هایی که در یک ساعت مشخص با یک روش خاص انجام شده

**🎨 Visual Encoding:**  
- گره‌های `transaction_type`: آبی  
- گره‌های `time_of_sale`: قرمز  
- ضخامت لبه: بر اساس تعداد تراکنش  
- رنگ یکنواخت برای یال‌ها

---

### 📊 کاربرد تحلیل

- تشخیص ساعات اوج برای روش‌های پرداخت خاص
- تصمیم‌گیری در مورد تعداد یا نوع دستگاه‌های پرداخت در شیفت‌های مختلف
- ارتقاء تجربه مشتری و جلوگیری از صف‌های طولانی

---

### 🖼️ Network Graph Preview

![Payment Method Network](./2.png)

---

### 📁 Included Files

| File Name     | Description                                        |
|---------------|----------------------------------------------------|
| `2.gephi`     | Gephi project file with visual and metric results  |
| `nodes.csv`   | Nodes: time slots and payment types                |
| `edges.csv`   | Edges weighted by transaction count                |
| `2.png`       | Final graph preview image                          |

---

> 📌 *این تحلیل به مدیر رستوران کمک می‌کند تا در زمان مناسب، تجهیزات مناسب پرداخت را در دسترس داشته باشد و صف‌های پرداخت را کاهش دهد.*


