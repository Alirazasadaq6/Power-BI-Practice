# Adidas USA – Data Cleaning & Transformation Using Power Query

## 📊 Project Overview

I performed data cleaning and transformation on an Adidas USA product dataset using Microsoft Power BI and Power Query Editor.

The objective was to improve data quality, standardize product information, and prepare a structured dataset for accurate reporting and analysis.


## 🛠️ Tools & Technologies

- **Microsoft Power BI Desktop** – Data preparation, validation, and reporting
- **Power Query Editor** – Data cleaning and transformation
- **Power Query M Language** – Understanding and reviewing transformation expressions
- **Microsoft Excel** – Source dataset

## 📁 Dataset Information

The dataset contains 845 Adidas USA product records across three main categories:

- Shoes
- Clothing
- Accessories

Key columns used during data cleaning include:

- `sku`
- `category`
- `breadcrumbs`
- `selling_price`
- `average_rating`
- `reviews_count`

Additional columns created during transformation:

- `Merged_Category` – Combined product category information
- `SKU_Prefix` – First three characters extracted from the SKU


**Dataset Source:** This project uses the same `adidas_usa.xlsx` dataset as Day 1. The original dataset is available in the [Day 1 project folder](https://github.com/Alirazasadaq6/Power-BI-Practice/tree/main/Day-01-Adidas-Product-Analysis).


## 🧹 Data Cleaning & Transformation

**1. Data Type Validation**

Reviewed and validated column data types to ensure that text, numeric, and other values were correctly classified.

**2. Column Quality & Data Profiling**

Used Power Query's data profiling features to inspect:

- Valid values
- Missing or empty values
- Errors
- Distinct values
- Unique values
- Column distribution

**3. Removing Duplicates & Blank Rows**

Practised identifying and removing duplicate records and unnecessary blank rows to improve data quality.

**4. Splitting Columns**

Used the Split Column by Delimiter transformation to separate product breadcrumb information.

Example:

`Women/Clothing` → `Women` and `Clothing`

**5. Merging Columns**

Combined the split breadcrumb values into a new column named `Merged_Category`.

Example:

`Women` + `Clothing` → `Women - Clothing`

**6. Replacing Values**

Standardized selected category names using the Replace Values transformation.

Example:

`Women - Clothing` → `Women's Clothing`

**7. Trim & Clean Text**

Applied text cleaning transformations:

- **Trim** – Removed unnecessary leading and trailing spaces
- **Clean** – Removed non-printable characters

**8. Text Formatting**

Practised converting text into different formats:

- UPPERCASE
- lowercase
- Capitalize Each Word

**9. Extracting Text**

Extracted the first three characters from the `sku` column to create `SKU_Prefix`.

**10. Removing Temporary Columns**

Removed unnecessary practice columns while retaining the relevant cleaned and transformed fields.

## ⚙️ Power Query M Language

Explored the Power Query Formula Bar and Advanced Editor to understand how data transformations are represented using M expressions.

Key functions studied:

| **M Function** | **Purpose** |
|---|---|
| `Text.Trim()` | Remove leading and trailing whitespace |
| `Text.Clean()` | Remove non-printable characters |
| `Text.Upper()` | Convert text to uppercase |
| `Text.Lower()` | Convert text to lowercase |
| `Text.Proper()` | Capitalize each word |
| `Text.Start()` | Extract characters from the beginning |
| `Text.End()` | Extract characters from the end |
| `Text.Middle()` | Extract characters from a specific position |
| `Table.ReplaceValue()` | Replace values in a table |

## 🔍 Data Validation

After applying transformations, I reviewed the cleaned dataset to check:

- Column data types
- Missing and invalid values
- Column quality and distribution
- Transformation errors
- Applied Steps dependencies
- Required columns for reporting

The cleaned data was then loaded into Power BI for report validation.

## 🎯 Skills Demonstrated

- Power Query Data Cleaning
- Data Type Validation
- Data Profiling
- Duplicate and Null Value Handling
- Split and Merge Columns
- Replace Values
- Text Cleaning and Formatting
- Text Extraction
- Applied Steps Management
- Power Query M Language Basics
- Advanced Editor Exploration
- Data Quality Validation
- Preparing Data for Power BI Reporting

## 🖼️ Dashboard Preview

This project builds on the Adidas USA Product Analysis Dashboard created on Day 1.

[View Day 1 Adidas USA Dashboard](https://github.com/Alirazasadaq6/Power-BI-Practice/blob/main/Day-01-Adidas-Product-Analysis/dashboard.png)

The Day 2 Power BI file contains the additional data cleaning and transformation work.

🖼️ Power Query Preview

This project focuses on data cleaning and transformation using Power Query Editor rather than dashboard development.

The screenshot shows the Power Query Editor with the cleaned Adidas dataset, transformed columns, and Applied Steps.

Power Query Screenshot: power_query_screenshot.png

## 📂 Project Files

| **File** | **Description** |
|---|---|
| `Day_02_Adidas_Data_Cleaning.pbix` | Power BI file containing data cleaning and Power Query transformations |
| `power_query_screenshot.png` | Screenshot of Power Query Editor showing the transformed dataset and Applied Steps |
| `README.md` | Data cleaning project documentation |

**Dataset:** The Adidas USA Excel dataset is available in the Day 1 project folder.

## 📚 Learning Outcome

This project helped me develop practical skills in preparing, cleaning, validating, and transforming real-world product data using Power Query.

I learned how to manage transformation steps, work with text functions, inspect data quality, and understand the fundamentals of Power Query M Language.
