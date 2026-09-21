# Funnel and Retention Analysis for MercadoLibre
**Skills and technology used:** ![Static Badge](https://img.shields.io/badge/SQL-blue?style=plastic&logo=postgresql&logoColor=white&logoSize=auto&label=%20%20%20&labelColor=black)
![Static Badge](https://img.shields.io/badge/Funnel%20Analysis-blue?style=plastic)
![Static Badge](https://img.shields.io/badge/Cohort%20Analysis-blue?style=plastic)
![Static Badge](https://img.shields.io/badge/Data%20Storytelling-blue?style=plastic)
![Static Badge](https://img.shields.io/badge/Excel%2FGoogle%20Sheets-green?style=plastic&logo=googlesheets&logoColor=white&logoSize=amg&labelColor=black)

## 📋 Context
Analyzed 8 months of MercadoLibre user data in 10 countries of LATAM to identify desertion patterns in the purchase funnel and the customer retention.

Objective: understand where customers drop off and why retention declines to implement strategies to improve retention in the purchase funnel.

**Data sources:** mercadolibre_funnel + mercadolibre_retention

**Analysis period:** 01/01/2025 - 08/31/2025

## 🔍 Findings

### Funnel Analysis
- **Conversion flow:** 76.90% (select_item) → 11.01% (add_to_cart) → 4.00% 
  (begin_checkout) → 2.42% (add_shipping) → 2.09% (add_payment) → 1.25% (purchase)
- **Critical drop-off:** -65.89 pp between select_item → add_to_cart
- **Possible cause:** Issues with product page optimization, pricing presentation and customer trust signals.

### Retention Analysis by Country
- **Uruguay:** Best retention with 4.55% final conversion
- **Bolivia:** 3.23% final conversion
- **Mexico:** 2.48% final conversion
- **Paraguay, Ecuador, Colombia:** Worst retention with 0% final conversion

**Country specific issues identified:**
- Paraguay collapses at begin_checkout.
- Ecuador and Colombia stagnate at add_payment_info.

### Retention Over Time (Days)
The averages were approximately:
- D7 → 86.6%
- D14 → 55.4%
- D21 → 25.0%
- D28 → 2.6%

The greatest drop off occurs between D7 and D14 with approximately -31 pp. The March cohort had the best retention (D7 → 87.7%; D28 → 3.0%), while August presents an atypical behavior (D7 → 70.8%; D28 → 0.2%), being the lowest retention of the time period analyzed.

## 💡 Implications
### What This Means for Business
1. **Fix Product Page Experience (Highest Priority)**
   - Optimize product presentation, pricing clarity and customer trust signals
   - This single improvement could recover a significant portion of conversions
2. **Audit Country-Specific Technical Issues**
   - Investigate begin_checkout failures in Paraguay
   - Debug payment gateway integration in Ecuador & Colombia
3. **Increase Retention Through Targeted Interventions**
   - Focus on D7-D14 window (when 31% of users abandon)
   - Implement: rewards, personalized notifications and price drop alerts for returning customers
   - Analyze device type and traffic source to identify highest-converting channels
4. **Validate All Improvements**
   - A/B test product page redesign
   - Test retention strategies by country and device type
   - Monitor via ongoing funnel tracking
