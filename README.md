# Inventory-Management
A comprehensive inventory management analysis for multi-category e-commerce supply chain management, demonstrating ABC-XYZ classification, Economic Order Quantity (EOQ) modeling, safety stock calculations, and reorder point determination based on real-world operations across 118 unique SKUs.

![Excel](https://img.shields.io/badge/Excel-Advanced-green.svg)  ![PowerBI](https://img.shields.io/badge/PowerBI-green.svg)  ![Status](https://img.shields.io/badge/Status-Complete-success.svg)

## 🎯 Business Problem
In e-commerce and retail supply chain management, maintaining optimal inventory levels is critical for:
- **Preventing stockouts** that disrupt deliveries and damage customer sastification
- **Minimizing holding costs** from excess inventory consuming valuable warehouse space
- **Optimizing procurement decisions** through data-driven reorder points and order quantities
- **Reducing operational costs** from inefficient ordering patterns and excess safety stock
- **Improving cash flow** by identifying amount of stock value in potential inventory reduction

This project addresses these challenges by implementing industry-standard inventory optimization techniques on **118 SKUs across 45+ product categories** in an e-commerce environment, resulting in quantifiable recommendations for $1.48M cost savings (24.4% of current inventory value).

## 📊 Project Overview
### Dataset
- **Scope:** 12 months of daily inventory transactions
- **SKUs Analyzed:** 118 unique products across 45+ categories
- **Total Records:** 53,196 daily transaction records
- **Categories:** Electronics, Apparel, Sports Equipment, Health & Beauty, Books, Music, and more
### Current Portfolio Status
- **Total Current Inventory Value:** $6,075,152
- **Total SKUs:** 118
- **Average Lead Time:** 4 days
- **Service Level Achievement:** 91.5% items above Reorder Point (ROP)
- **Critical Items Below ROP:** 16 SKUs requiring immediate ordering
### Key Analyses Performed
1. **ABC Classification Analysis**
    - Categorizes inventory items by annual sales value contribution (Pareto principle)
    - Identifies high-value products requiring focused management attention
    - Results:
        - **Class A:** 9 SKUs (7.6% of total) generating 87.3% of value ($9.2M revenue)
        - **Class B:** 23 SKUs (19.5%) generating 18.8% of value ($1.99M revenue)
        - **Class C:** 86 SKUs (72.9%) generating 5.8% of value ($608K revenue)
2. **XYZ Demand Variability Analysis**
    - Analyzes demand predictability using Coefficient of Variation (CV)
    - Identifies demand patterns and forecasting requirements
    - Results:
        - **X-Class (Predictable):** 4 items (3.4%) - CV < 0.2
        - **Y-Class (Moderate):** 52 items (44.1%) - CV 0.2-0.5
        - **Z-Class (Unpredictable):** 62 items (52.5%) - CV > 0.5
    - **Key Finding:** 52.5% of items have high demand variability, requiring stronger demand forecasting
3. **Economic Order Quantity (EOQ) Optimization**
    - Calculates optimal order quantities to minimize total inventory costs
    - Balances ordering costs vs. holding costs
    - Results: Determines optimal number of orders per year for each product
4. **Safety Stock & Reorder Point Analysis**
    - Determines buffer inventory to maintain 95% service levels
    - Accounts for demand variability and lead time uncertainty
    - Identifies items requiring immediate reordering
    - Results:
        - **Items Below ROP (Critical):** 16 SKUs
        - **Items Above ROP (Healthy):** 108 SKUs (91.5%)
5. **Stock Level Classification**
    - Categorizes current inventory into three levels: High, Mid, Low
    - Results:
        - **High Stock Level:** 8 items (6.8%) - potential over-stocking risk
        - **Mid Stock Level:** 86 items (72.9%) - optimal range
        - **Low Stock Level:** 24 items (20.3%) - watch list for potential stockouts
6. **Cost Optimization & Savings Identification**
    - Identifies cost reduction opportunities across portfolio
    - Calculates potential annual savings
    - Results: 
	    - **Total Potential Savings Opportunity:** $1,482,335 (24.4% of current inventory value)
## 🛠️ Technologies Used
- **Microsoft Excel Advanced** - Data analysis (ETL) and Calculations using formulas
    - Power Query supports load, clean and transform raw data
    - Pivot tables supports metrics calculations for ABC classification, EOQ, ROP, Safety Stock 
    - Formulas: IF & Nested IFs, XLOOKUP
- **Microsoft PowerBI** - Data Visualization
    - Data modeling
    - Visualization: Charts, Cards, Slicers
    - DAX measures and Calculated columns
    - Conditional formating
## 📈 Key Results
### ABC Classification Results

| Class     | # of SKUs | % of SKUs | Annual Value    | % of Total Value |
| --------- | --------- | --------- | --------------- | ---------------- |
| **A**     | 9         | 7.6%      | $9,215,164      | 78.04%           |
| **B**     | 23        | 19.5%     | $1,985,555      | 16.81%           |
| **C**     | 86        | 72.9%     | $607,717        | 5.15%            |
| **TOTAL** | **118**   | **100%**  | **$11,808,436** | **100%**         |
### Demand Variability (XYZ Classification)
| Class | # of SKUs | % of SKUs | Demand Pattern      | Forecast Challenge |
| ----- | --------- | --------- | ------------------- | ------------------ |
| **X** | 4         | 3.4%      | Highly Predictable  | Low                |
| **Y** | 52        | 44.1%     | Moderately Variable | Moderate           |
| **Z** | 62        | 52.5%     | Highly Variable     | High               |
### Economic Order Quantity (EOQ) Analysis
| Metric                          | Value    |
| ------------------------------- | -------- |
| **Average EOQ**                 | 27 units |
| **Annual Ordering Cost**        | $34,377  |
| **Annual Holding Cost**         | $34,377  |
| **Total Annual Inventory Cost** | $68,754  |
### Safety Stock & Reorder Point Summary
| Metric                         | Value           |
| ------------------------------ | --------------- |
| **Average SS per Item**        | $39.18          |
| **Average ROP per Item**       | $85.15          |
| **Items Below ROP**            | 16 (13.6%)      |
| **Items in Safe Zone**         | 108 (91.5%)     |
| **Critical A-Class Below ROP** | 1 (Dell Laptop) |

**⚠️ Immediate Action Required:**
- **Dell Laptop (SKU 1351):** A-Class item, currently at exact ROP - requires immediate reordering
- **6 B-Class items:** Below ROP - need emergency procurement this week
- **Overstock items:** 8 SKUs
### Stock Level Distribution
| Stock Level | # of SKUs | % of SKUs | Assessment                      |
| ----------- | --------- | --------- | ------------------------------- |
| **High**    | 8         | 6.8%      | Over-stocked, obsolescence risk |
| **Mid**     | 86        | 72.9%     | Healthy, optimal range          |
| **Low**     | 24        | 20.3%     | Monitor for stockout risk       |

**Insight:** 72.9% of items are in healthy "Mid" range - suggests well-balanced overall inventory position.
## 💡 Business Impact
### Quantifiable Benefits
- **Inventory Cost Reduction:** Identified potential to free up $1.48M in tied-up capital, annual savings opportunity (24.4% of current inventory)
- **Stockout Prevention:** Calculated reorder points ensure continuous product availability for high-value items
- **Management Focus:** ABC-XYZ classification enables prioritized attention (9 A-items represent 78% of revenue)
### Strategic Recommendations
**Immediate Actions:**
1. **Order critical A-class items** below ROP (especially Dell Laptop at exact ROP)
2. **Emergency procurement** for 6 B-class items below reorder point
3. **Demand audit** on overstock 8 items to identify forecast errors
## 📂 Project Structure
```
inventory-management/
│
├── Dataset.csv                            # Project dataset
├── Inventory_Management.xlsx              # Main Excel workbook with analysis
│   ├── Sheet: Data                        # 53,196 transaction records
│   ├── Sheet: ABC_Analysis                # ABC classification
│   ├── Sheet: EOQ                         # EOQ calculations for all 118 SKUs
│   ├── Sheet: ROP                         # Safety stock & reorder point 
│   ├── Sheet: Pivot                       # Pivot table supporting calculations 
│   └── Sheet: Summary                     # Integrated key results
│
├── Inventory_Management.pbix              # PowerBI interactive dashboard
│
├── Inventory_Management_Dashboard.png     # Visualization dashboard
├── README.md                              # Project documentation
```
### Worksheets Explanation
| Sheet            | Purpose                                | Key Metrics                                                                        |
| ---------------- | -------------------------------------- | ---------------------------------------------------------------------------------- |
| **Summary**      | Integrated results and recommendations | ABC Class, XYZ Class, EOQ, ROP, Stock Level, Reorder Point, Stock & Reorder Status |
| **Data**         | Complete transaction history           | Daily demand, lead times, costs, inventory levels...                               |
| **ABC_Analysis** | Product value classification           | Annual sales value, cumulative percentage, ABC classification                      |
| **EOQ**          | Order quantity optimization            | Optimal order quantity, order & holding costs, annual costs                        |
| **ROP**          | Reorder point determination            | Safety stock, reorder point, demand/lead time variability                          |
| **Pivot**        | Support calculations using Pivot       |                                                                                    |

## 📊 Visualizations
The project includes dashboards and visualizations including:
- **Inventory Health Snapshot:** Current stock value, quantity, SKUs analyzed
- **Pareto Analysis Chart:** ABC classification showing value concentration (80/20 rule)
- **Stock Level Distribution:** High/Mid/Low classification pie chart
- **Products by Reorder Status:** Order Now, Plan To Order, ReOrder Not Required
- **Revenue and Stock Value by Demand Variability and Stock Quantity:** Scatter plot showing demand-inventory relationship
- **Summary table:** Including information about ABC Class, Revenue, Cummulative Revenue (%), Stock & Stock Value, EOQ, Safety Stock, ROP and Average Lead Time Days for each SKU
<img width="1909" height="994" alt="Inventory_Management_Dashboard" src="https://github.com/user-attachments/assets/79b12be2-891a-4047-8da2-a0252d605d02" />

## 📋 Calculations
### 1. Data Collection & Preparation
- Collected 53,196 daily transaction records over 12 months
- Organized data by product, category, date, demand quantity, and unit costs
- Calculated key metrics: Revenue and Percentage Cummulative Revenue for ABC Classification, EOQ, Safety Stock, ROP, lead times, demand variability, 

### 2. ABC Classification Analysis
**Objective:** Identify high-value items requiring focused management attention
**Process:**
1. Calculated annual sales value for each SKU = Annual demand × Unit price
2. Sorted SKUs by descending annual sales value
3. Calculated cumulative value and percentage of total
4. Classified based on cumulative percentage:
    - Class A: 0-80% of total value (9 SKUs)
    - Class B: 80-95% of total value (23 SKUs)
    - Class C: 95-100% of total value (86 SKUs)
**Formula:**
```
ABC Class = IF(Cumulative % ≤ 80%, "A", IF(Cumulative % ≤ 95%, "B", "C"))
```
**Result:** 78.04% of value concentrated in 7.6% number of SKUs
### 3. XYZ Demand Variability Analysis
**Objective:** Understand demand predictability for each product
**Process:**
1. Calculated daily demand mean and standard deviation for each SKU
2. Computed Coefficient of Variation (CV) = Standard Deviation / Mean
3. Classified based on CV values:
    - X-Class: CV < 0.30 (Predictable)
    - Y-Class: CV 0.30-0.70 (Moderately variable)
    - Z-Class: CV > 0.70 (Highly variable)
**Formula:**
```
CV = STDEV(Daily Demand) / AVERAGE(Daily Demand)
XYZ Class = IF(CV < 0.2, "X", IF(CV > 0.5, "Z", "Y"))
```
**Finding:** 52.5% of items have high demand variability (Z-Class), requiring enhanced forecasting
### 4. Economic Order Quantity (EOQ) Calculation
**Objective:** Determine optimal order quantity that minimizes total inventory costs
**Formula:**
```
EOQ = √[(2 × Annual Demand × Ordering Cost) / Holding Cost per Unit]
```
**Components:**
- **Annual Demand:** Sum of daily demand × 365 days
- **Ordering Cost:** $20 per order (includes procurement, shipping verification)
- **Holding Cost:** 20-25% of unit cost annually
### 5. Safety Stock Calculation
**Objective:** Determine buffer inventory to maintain 95%+ service level
**Formula:**
```
SS = z × √(L × σ_d² + D_avg² × σ_L²)
```
**Where:**
- **z-score:** 1.65 (95% service level)
- **σ_d:** Standard deviation of daily demand
- **σ_L:** Standard deviation of lead time in days
- **D_avg**: daily demand
### 6. Reorder Point (ROP) Determination
**Objective:** Identify when to trigger new purchase orders
**Formula:**
```
ROP = (Average Daily Demand × Lead Time Days) + Safety Stock
```
## 🎓 Skills Demonstrated
- **Inventory Management:** Inventory optimization, ABC classification analysis, Calculate EOQ, SS, ROP
- **Data Analytics:** Excel (Power Query, Pivot Table) to load, clean and transform raw data and Power BI (Data modeling, DAX measures, Calculated columns, Charts) to create executive dashboard
  **Business Intelligence:** Actionable recommendations, Business impact quantification ($1.48M savings opportunity)
- **Domain Knowledge:** e-commerce warehouse and inventory managements
## 📄 License
This project is open source and available under the [MIT License](https://github.com/h8ngquan-sca/Inventory-Management/blob/main/LICENSE).
