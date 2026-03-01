Data Dictionary

Dataset: Superstore Sales Dataset



Source: Superstore sample retail dataset (commonly used retail analytics dataset)

Downloaded: January 2026

File: data/raw/Sample - Superstore.csv

Rows: 9,994

Columns: 21





| Column Name     | Data Type | Description                                       | Example Value                     | Notes                                  |

| --------------- | --------- | ------------------------------------------------- | --------------------------------- | -------------------------------------- |

| `Row ID`        | integer   | Unique identifier for each row/transaction record | 1                                 | Sequential ID                          |

| `Order ID`      | string    | Unique identifier for each order                  | CA-2016-152156                    | Multiple rows can share same Order ID   |

| `Order Date`    | date      | Date the order was placed                         | 2016-11-08                        | Format: YYYY-MM-DD                     |

| `Ship Date`     | date      | Date the order was shipped                        | 2016-11-11                        | Used to calculate shipping duration    | 
| `Ship Mode`     | string    | Shipping method selected                          | Second Class                      | Standard Class, First Class, Same Day  |

| `Customer ID`   | string    | Unique identifier for each customer               | CG-12520                          | Repeat customers share ID              |

| `Customer Name` | string    | Name of the customer                              | Claire Gate                       |                                        |

| `Segment`       | string    | Customer segment classification                   | Consumer                          | Consumer, Corporate, Home Office       |

| `Country`       | string    | Country of the customer                           | United States                     | Dataset limited to U.S.                |

| `City`          | string    | Customer city                                     | Henderson                         |                                        |

| `State`         | string    | Customer state                                    | Kentucky                          |                                        |

| `Postal Code`   | integer   | Customer ZIP/postal code                          | 42420                             | U.S. postal codes                      |

| `Region`        | string    | Geographic region                                 | South                             | West, East, Central, South	       |

| `Product ID`    | string    | Unique identifier for each product                | FUR-BO-10001798                   |                                        |

| `Category`      | string    | High-level product category                       | Furniture                         | Furniture, Technology, Office Supplies |

| `Sub-Category`  | string    | More specific product grouping                    | Bookcases                         |                                        |

| `Product Name`  | string    | Full product name                                 | Bush Somerset Collection Bookcase |                                        |

| `Sales`         | float     | Revenue generated from the order line             | 261.96                            | Currency in USD                        |

| `Quantity`      | integer   | Number of units sold                              | 2                                 |                                        |

| `Discount`      | float     | Discount applied to the order line                | 0.20                              | Represented as decimal (0–1)	       |

| `Profit`        | float     | Net profit earned on the order line               | 41.91                             | Can be negative (loss)       	       |





Data Quality Notes



Missing values: No missing values detected across all 21 columns.



Duplicates: No exact duplicate rows found. Multiple rows may share the same Order ID due to multi-item orders.



Assumptions: Sales and Profit are recorded in USD. Discount is applied per order line, not per entire order.



Limitations: Dataset does not include cost breakdown, marketing spend, inventory levels, or customer lifetime value metrics.



Changes Made During Cleaning



Verified and formatted Order Date and Ship Date as proper date fields.



Confirmed Discount, Sales, and Profit data types as numeric for accurate calculations.



Removed no rows as there were no missing or duplicate records.



Cleaned file saved to: data/cleaned/Superstore\_clean.csv



