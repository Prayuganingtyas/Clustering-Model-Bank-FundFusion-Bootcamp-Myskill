# **Clustering-Model-Bank-FundFusion-Bootcamp-Myskill**  
This project was developed as part of my learning experience in the Data Analyst Bootcamp at Myskill, where I focused on applying Python code for Clustering Model analysis.

### **PROBLEM STATEMENT**  
There is no effective strategy for offering the appropriate products to the segments of potential customers to be recruited.

### **OBJECTIVE**  
To create a clustering model that can identify product ownership based on the demographics of customers who are currently using FundFusion services, with a Silhouette Score >0.7.

### **AVAILABLE VARIABLES**  
The dataset contains several data points:

---
**1. GCIF**: Unique Customer Identifier  
**2. Area**: Customer's location (Jakarta, Bogor, Bandung, Surabaya, Jogja, Solo)  
**3. Jalur_Pembukaan**: Customer's touchpoint for product registration → Branch, Telemarketing, Digital Application, Internet Banking  
**4. Vintage**: Duration as a customer (since account opening)  
**5. Usia**: Customer's age  
**6. Jenis_Kelamin**: Gender (Male: 1, Female: 0)  
**7. Status_Perkawinan**: Marital status (Single: 0, Married: 1, Divorced: 2, Widowed: 3)  
**8. Jumlah_Anak**: Number of children (numeric)  
**9. Pendidikan**: Last level of education (No formal education: 0, Elementary: 1, Middle School: 2, High School: 3, Bachelor: 4, Master: 5, Doctorate: 6)  
**10. Produk_Tabungan**: Product ownership status (Yes/1, No/0)  
**11. Produk_Deposito**: Product ownership status (Yes/1, No/0)  
**12. Produk_Kartu_Kredit**: Product ownership status (Yes/1, No/0)  
**13. Produk_Kredit_Rumah**: Product ownership status (Yes/1, No/0)  
**14. Produk_Kredit_Kendaraan**: Product ownership status (Yes/1, No/0)  
**15. Produk_Kredit_Dana_Tunai**: Product ownership status (Yes/1, No/0)  
**16. Total_Kepemilikan_Produk**: Total number of products owned (sum of all products)  
**17. Pendapatan_Tahunan**: Average annual income  
**18. Total_Relationship_Balance**: Total customer assets at the observation cutoff month  

# **EXPERIMENT**

**Point of View:**  
1. Clustered based on demographics to find patterns in product ownership.  
2. Clustered based on product ownership to find patterns in demographics.

# **RECOMMENDATIONS AND CONCLUSIONS**

## Recommendations

### **1. Cluster 0:**  
   - **Profile:** Very high total balance (around 400 million) and relatively few children. Customers in this cluster already own many savings and deposit products.  
   - **Product Offering Strategy:**
     - **Premium Deposits:** Increase offering of deposits with competitive interest rates, considering their high balance.
     - **Credit Cards with High Limits:** Offer premium credit cards with higher limits and exclusive rewards programs to encourage usage.
     - **Luxury Home or Vehicle Loans:** With a high balance, these customers may be interested in home or luxury vehicle loans.

### **2. Cluster 1:**  
   - **Profile:** Medium total balance (around 172 million) and a similar average number of children as other clusters. They primarily have savings and deposit products, but credit card and home loan usage is still low.  
   - **Product Offering Strategy:**
     - **Home Loans:** Encourage home loan ownership by offering affordable financing options.
     - **Credit Cards with Attractive Promotions:** Offer credit cards with cashback or reward points to increase appeal.
     - **Term Deposits:** Offer term deposits with competitive interest rates for customers seeking safe investments.

### **3. Cluster 2:**  
   - **Profile:** Medium-high total balance (around 284 million), with a slightly higher average number of children than other clusters. Their main products are savings and home loans.  
   - **Product Offering Strategy:**
     - **Savings and Deposit Bundles:** Offer bundles of savings and deposits to encourage ownership of safe investment products.
     - **Vehicle Loans:** This cluster is likely to be interested in vehicle loans, especially for those who already own a home.
     - **Medium Limit Credit Cards:** Offer credit cards with medium limits and rewards programs focused on everyday needs.

### **4. Cluster 3:**  
   - **Profile:** Relatively low total balance (around 59 million) and a slightly higher number of children than average. Their main products are savings and home loans, while credit cards are less popular.  
   - **Product Offering Strategy:**
     - **Vehicle Loans or Cash Loans:** Offer vehicle loans or cash loans with low interest rates, as this cluster may need financial support for everyday needs.
     - **Sustained Savings Programs:** Provide automatic savings programs with routine deposits to help accumulate balance.
     - **Basic Credit Cards:** Offer credit cards with low limits and minimal annual fees, especially for customers without credit cards.

### **5. Cluster 4:**  
   - **Profile:** Very high total balance (around 607 million) with a higher number of children. This cluster is highly interested in all products, including savings, deposits, credit cards, and home loans.  
   - **Product Offering Strategy:**
     - **Exclusive Home Loans:** Offer home loan products with special interest rates and additional services, considering their high interest in home loans.
     - **Premium Credit Cards with Exclusive Benefits:** Offer premium credit cards providing access to exclusive programs like airport lounges or special cashback.
     - **Vehicle Loans or Cash Loans with Competitive Interest Rates:** Customers with high balances may be interested in vehicle loans or cash loans that provide flexible financing options.

### **Conclusion:**  
By implementing tailored strategies like the ones above, clients can offer more relevant products to each customer cluster:

1. **Cluster 0** – Focus on investment products, home loans, and premium credit cards.
2. **Cluster 1** – Focus on home loans, term deposits, and credit cards with attractive promotions.
3. **Cluster 2** – Encourage vehicle loans and product bundling for savings and deposits.
4. **Cluster 3** – Prioritize vehicle loans or cash loans, as well as basic credit cards with low limits.
5. **Cluster 4** – Target exclusive home loan products, premium credit cards, and competitive vehicle or cash loans.

From the clustering results, the key differentiator is the Total Relationship Balance. However, segmenting customers solely based on this variable does not provide a clear enough segmentation (as seen from the silhouette score not reaching 0.7). Future improvements could involve adding more variables and running additional iterations.
