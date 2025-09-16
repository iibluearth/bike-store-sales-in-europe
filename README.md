# 🚴‍♂️ Bike Store Sales in Europe – Excel Project

🔗 **[View Live Excel](https://1drv.ms/x/c/6f959456e43a0e33/EY3Ud21db-FBl3Wd5gwjEbIBuShOOMHO94UoKUxi8X8KUQ?e=rD80gc)

## Resources

- Dataset: [Kaggle: Bike Store Sales in Europe](https://www.kaggle.com/code/sadiqshah/bike-store-sales-in-europe)

- Tools: Microsoft Excel

## 📌 Project Overview

This project analyzes **bike purchase behavior in Europe** using the Bike_Buyers dataset. The dataset contains customer demographics, financial details, and lifestyle factors to identify patterns in bike purchases.

The project involves:

- Data cleaning and transformation of raw data

- Creating a structured **working sheet** for analysis

- Building **pivot tables** to summarize insights

- Designing a **Bike Sales Dashboard** for visualization

## 📂 Dataset

```
Raw Data Fields:

- ID

- Marital Status

- Gender

- Income

- Children

- Education

- Occupation

- Home Owner

- Cars

- Commute Distance

- Region

- Age

- Purchase Bike
```

<img src=https://i.imgur.com/jnVDPNS.png/>
</p>

## 🛠️ Data Cleaning Process (Working Sheet)

Steps applied to raw data before analysis:

### 1. Apply Filters

- `Ctrl + A`→ `Filter`

<img src=https://i.imgur.com/H5861hL.png/>
</p>

### 2. Remove Duplicates

-  `Data` → `Remove Duplicates` → Select All

<img src=https://i.imgur.com/l69jZYE.png/>
</p>

### 3. Find & Replace Values

- `Ctrl + H` → Replace codes with readable labels

  - Marital Status:

    - `"M"` → `Married`

    - `"S"` → `Single`

  - Gender:

    - `"F"` → `Female`

    - `"M"` → `Male`

<img src=https://i.imgur.com/wAHvFL7.png/>
</p>

### 4. Format Currency

- Standardized **Income** field → `Decrease Decimal`

<img src=https://i.imgur.com/JkhuV95.png/>
</p>

### 5. Age Brackets (Categorization)

Created a new **Age Group** column:

```
=IF(L2>54,"Old",IF(L2>=31,"Middle Age",IF(L2<31,"Adolescent","Invalid")))
```
- Adolescent → < 31

- Middle Age → 31–54

- Old → > 54

<i>(Note: Avoid nested IF duplication errors – use only the final version above.)</i>

<img src=https://i.imgur.com/bqSSPer.png/>
</p>

## 📊 Pivot Tables

Created multiple pivot tables to explore relationships in the data:

### 1. Average Income by Gender (Per Purchase)

- Shows whether male or female customers have higher average incomes when purchasing bikes.

<img src=https://i.imgur.com/0Psemh1.png/>
</p>

### 2. Count of Purchased Bikes by Commute Distance (Per Customer)

- Highlights how commuting habits influence bike purchases.

<img src=https://i.imgur.com/lNR0oks.png/>
</p>

### 3. Count of Purchased Bikes by Age Brackets

- Compares purchase rates between **Adolescent, Middle Age, and Old** groups.

<img src=https://i.imgur.com/qSPBRBu.png/>
</p>

## 📊 Bike Sales Dashboard

Designed an interactive dashboard with:

- **Visualizations** for:

  - Average income by gender per purchase

  - Bike purchases by commute distance

  - Bike purchases by age bracket

- **Slicers** for filtering by:

  - Marital Status

  - Region

  - Education

This allows users to segment data dynamically and see how different factors affect bike purchases.

<img src=https://i.imgur.com/2d7iDZc.png/>
</p>

## 🎯 Key Learnings

- **Data Cleaning Matters** → Removing duplicates, replacing coded values (M/F, S/M), and formatting income made the dataset easier to interpret and analyze.

- **Age Grouping Added Insights** → Creating age brackets helped reveal purchasing trends across life stages (Adolescent, Middle Age, Old).

- **Pivot Tables Simplify Analysis** → Using pivot tables made it easy to compare average income by gender, purchases by commute distance, and purchases by age groups.

- **Dashboards Improve Communication** → Combining charts with slicers (Marital Status, Region, Education) turned raw data into an interactive, user-friendly tool for decision-making.

- **Excel as an Analytics Tool** → Beyond simple spreadsheets, Excel can replicate some BI capabilities (like filtering and segmenting customer behavior).