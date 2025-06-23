# 📦 Tableau Prep Flow - Regional Orders & Returns Integration

This project demonstrates the use of **Tableau Prep Builder** to clean, combine, and enrich sales data from multiple regions (Central, East, West, and South), and join it with return information for analysis.

## 🗂️ Project Overview

The Tableau Prep flow consolidates regional order files, applies cleaning and data transformations, and merges them with return data to produce a unified dataset. The final output is exported as a `.csv` file and can be used for reporting or visualizations in Tableau Desktop.

---

## 🔁 Workflow Steps

### 1. **Input Files**
- `Orders_Central.csv`
- `Orders_West.csv`
- `orders_south_2015.csv`
- `Orders_East.xlsx`
- `return reasons_new.xlsx`

### 2. **Data Cleaning**
- Renamed and standardized column names
- Fixed data types and formatting (e.g., date and discount fields)
- Removed null or redundant entries

### 3. **Union Step**
- All cleaned regional datasets were merged into a single table using the **Union** tool.

### 4. **Join Step**
- The unified order dataset was **joined** with the cleaned return dataset on relevant keys (e.g., `Order ID` or `Product ID`) to enrich the data with return information.

### 5. **Output**
- The final dataset is saved as:  
  `Output.csv`  
  **Location:**  
  `C:\Users\kunal\Documents\My Tableau Prep Repository\Datasources\Output.csv`

---

## 🔍 Output Preview

| Date to Ship | Category        | Customer Name | Country       | Discount | Order ID         |
|--------------|------------------|----------------|----------------|----------|------------------|
| 19/11/2015   | Technology        | Robert Marley  | United States  | 0        | CA-2015-158274   |
| 13/09/2015   | Office Supplies   | Erin Ashbrook  | United States  | 0.6999   | US-2015-156216   |
| 24/12/2015   | Office Supplies   | Luke Foster    | United States  | 0.2      | CA-2015-113166   |

---

## 💼 Tools Used

- **Tableau Prep Builder**
- **Excel & CSV files**
- **Tableau Desktop (for visualization, optional)**

---

## 🚀 How to Use

1. Open `Flow1.tfl` in Tableau Prep Builder.
2. Ensure source files are located correctly or relink them.
3. Click `Run Flow` to generate the output.
4. Use the generated `Output.csv` in Tableau Desktop or other tools for analysis.

---

## 📅 License

This project is for educational and analytical purposes. Feel free to fork or contribute.

---
![Screenshot](https://github.com/kunal1300/Tableau/blob/main/Tableau%20Prep%20Builder/Screenshot%202025-06-23%20085520.png)
![Screenshot](https://github.com/kunal1300/Tableau/blob/main/Tableau%20Prep%20Builder/Screenshot%202025-06-23%20090531.png)
## 🙋‍♂️ Author

**Kunal Solanki**  
_Data Analyst | Tableau Enthusiast_
