# 💳 Meesho Payment Flexibility Demo

A simple prototype showing how a customer can switch from **Cash on Delivery (COD)** to **Google Pay (GPay)** before delivery.  
This feature improves user convenience, reduces COD cancellations, and lowers cash-handling costs.

---

## ✨ Features
- 🟠 Default checkout option shows **COD selected**  
- 🔵 Button to **Switch to GPay** → simulates online payment  
- ✅ Confirmation message updates order status to **Prepaid**  
- 💵 Option to **Keep COD** remains available  

---

## 🚀 How to Run
1. Download or clone this repository.  
2. Open `index.html` in any modern web browser (Chrome, Edge, Firefox).  
3. Click the buttons to simulate the payment flow.  

---

## 📹 Demo Flow
```mermaid
flowchart TD
    A[Customer places COD order] --> B[Option to switch payment method]
    B -->|Chooses GPay| C[Payment gateway processes transaction]
    C --> D[Order updated to Prepaid]
    D --> E[Courier notified: no cash collection]
    B -->|Keeps COD| F[Order remains COD]
    F --> G[Courier notified: collect cash on delivery]
