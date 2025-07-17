# Laptop-Price-Analysis
# About Dataset

The original dataset was pretty compact with a lot of details in each column. The columns mostly consisted of long strings of data, which was pretty human-readable and concise but for Machine Learning algorithms to work more efficiently it's better to separate the different details into their own columns. After doing so, 28 duplicate rows were exposed and removed with this dataset being the final result.
Formatting Issues The file was saved in standard encoding so there shouldn't be any problems reading it in pandas. Though if it gives you any trouble you could try reading it with the encoding='ISO-8859-1' parameter, as this was the original dataset's formatting. 

# Columns:

 ● Company: Laptop Manufacturer.
 ● Product: Brand and Model.
 ● TypeName: Laptop Type (Notebook, Ultrabook, Gaming, …etc).
 ● Inches: Screen Size.
 ● Ram: Total amount of RAM in laptop (GBs).
 ● OS: Operating System installed.
 ● Weight: Laptop Weight in kilograms.
 ● Price_euros: Price of Laptop in Euros. (Target)
 ● Screen: screen definition (Standard, Full HD, 4K Ultra HD, Quad HD+).
 ● ScreenW: screen width (pixels).
 ● ScreenH: screen height (pixels).
 ● Touchscreen: whether or not the laptop has a touchscreen.
 ● IPSpanel: whether or not the laptop has an IPSpanel.
 ● RetinaDisplay: whether or not the laptop has retina display.
 ● CPU_company
 ● CPU_freq: frequency of laptop CPU (Hz).
 ● CPU_model
 ● PrimaryStorage: primary storage space (GB).
 ● PrimaryStorageType: primary storage type (HDD, SSD, Flash Storage,
 Hybrid).
 ● SecondaryStorage: secondary storage space if any (GB).
 ● SecondaryStorageType: secondary storage type (HDD, SSD, Hybrid, None).
 ● GPU_company
 ● GPU_model

 # Project Summary

After analyzing the laptop dataset, I explored how various specifications — like company, processor type, RAM, storage, GPU, and OS — influence the overall pricing.

Through visualizations, I discovered patterns such as:
- Premium brands (e.g., Apple, MSI) command higher prices.
- Higher RAM and SSD storage clearly push prices up.
- Touchscreen laptops and newer OS versions also increase the cost.

I cleaned the dataset, encoded necessary features, and built three machine learning models — Linear Regression, Random Forest, and XGBoost — to predict prices.

XGBoost performed the best, showing that pricing can be predicted accurately based on specifications, which is valuable for strategic pricing and inventory decisions.

# Future Enhancements & Business Opportunities:

1.  Focus on High-Margin Features:
   From the model's feature importance, RAM, SSD, and GPU are top contributors to higher prices. 
   We should prioritize stocking laptops with these specs, as they offer better profitability and customer value.

2.  Introduce Tier-Based Product Bundles:
   Based on the pricing segmentation observed in visuals, we can bundle high-performing laptops into Bronze, Silver, and Gold tiers — making it easier for customers to choose based on need and budget, increasing     sales conversions.

3.  Data-Driven Dynamic Pricing:
   Implement a dynamic pricing tool using the XGBoost model, which updates prices based on configuration trends, market benchmarks, and stock levels — helping us stay competitive without undervaluing premium         models.

4.  Expand Premium Offerings for Business Clients:
   Since business-oriented specs (higher RAM, SSD, discrete GPUs) show a clear pricing jump, targeting enterprise segments with premium bundles can drive revenue growth.

5.  Build an Internal Sales Recommender:
   Equip our sales or e-commerce team with a tool that uses this model to suggest alternative configurations — helping upsell better laptops and reduce deadstock.

By integrating these insights into operations, we can improve pricing strategies, attract the right customer segments, and boost profitability.

 # Business Recommendations:

- Laptops with more SSD storage and better CPUs tend to be priced higher. The company should consider marketing configurations that focus on performance-based upselling.
- Windows-based laptops have greater pricing variability. Adding premium Windows models can increase margin diversity.
- Touchscreen availability doesn’t significantly raise average price — consider bundling features for perceived value without cost escalation.
