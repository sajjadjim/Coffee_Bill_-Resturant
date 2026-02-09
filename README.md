# ☕ Coffee Shop Bill Management System

A professional desktop-based billing application built using **Java Swing**. This system automates the ordering process for a coffee shop, allowing for quick item selection, automated tax calculation, and clean bill generation.

---

## 🚀 Features

* **Smart Selection:** * **Drinks:** Uses Radio Buttons for exclusive selection (Coffee, Tea, Milkshakes, etc.).
    * **Food:** Uses Checkboxes for multiple item selection (Pizza, Burger, Pasta, etc.).
* **Automatic Calculations:** * Instantly calculates **Sub-total**.
    * Calculates **15% VAT/Tax** automatically.
    * Generates the **Final Total Bill**.
* **Precision Formatting:** All currency values are displayed with two decimal places (e.g., `150.00`) using `DecimalFormat`.
* **User Controls:** * `Enter`: Process the bill.
    * `Clear`: Reset all fields and selections.
    * `Exit`: Close the application safely.

---

## 🛠️ Tech Stack

* **Language:** Java
* **GUI Library:** Java Swing & AWT
* **IDE:** NetBeans (Designed with GUI Form Builder)

---

## 📋 Menu & Pricing

| Category | Item | Price (Taka) |
| :--- | :--- | :--- |
| **Drinks** | Coffee | 50 |
| | Tea | 30 |
| | Milk Shake | 100 |
| | Chocolate Shake | 110 |
| | Water | 20 |
| **Food** | Pizza | 150 |
| | Burger | 80 |
| | Pasta | 130 |
| | Noodles | 90 |
| | Set Menu | 220 |

---

## ⚙️ Installation & Usage

1.  **Clone the Repository:**
    ```bash
    git clone [https://github.com/sajjadjim/Coffee-Shop-Bill-System.git](https://github.com/sajjadjim/Coffee-Shop-Bill-System.git)
    ```
2.  **Open in IDE:** Open the project folder in **NetBeans**, **IntelliJ**, or **Eclipse**.
3.  **Run Application:** Run the `ShopBill.java` file.
4.  **How to use:**
    * Select one drink and any number of food items.
    * Click **Enter** to see the subtotal, tax, and total.
    * Click **Clear** to start a new order.

---

## 💻 Logic Overview

The core calculation logic handles both the item price summation and the tax percentage:

```java
double subtotal = 0;
final double TAXRATE = 0.15; // 15% Tax

// Example Drink Selection
if (redCoffee.isSelected()) {
    subtotal += 50;
}

// Total Calculation
double tax = subtotal * TAXRATE;
double total = subtotal + tax;
```

👤 Author
Sajjad Hossain Jim

GitHub: @sajjadjim

Location: Dhaka, Bangladesh

Generated for the Coffee Shop Management Project.
