# India Sectoral Growth & Economic Performance Analysis 


Objective:

Identify top contributing industries to GDP, declining sectors, and inflation impact, and present actionable insights through an interactive Tableau dashboard.


Dataset:

eSankhyiki APIs provides macro indicator data published by National Statistical Office of India. This is India's National Accounts Statistics dataset published by MoSPI (Ministry of Statistics and Programme Implementation), covering the Indian economy from FY2011-12 to FY2025-26.

Dataset link: https://www.data.gov.in/resource/national-accounts-statistics-data


Tools:

Python (Pandas, Matplotlib, Seaborn) | Power BI


Project Workflow:
Firstly started understanding the data. Data looks simple but key challenge was it has high dimensionality and mixed granularity involved like multiple indicators (GDP, GVA, GNI, NDP, GFCF, GCF, GNDI etc.), Price types (Current vs Constant), Institutional sectors, industries, subindustries, Revision types (Advance, Revised, Final). 
After understanding granularity, dataset is imported in goggle collab for cleaning, manipulation and analysis using python libraries. Null values are not removed here because each indicator, address different industry, institutional sector and sub industry or it address overall year values. Data set is cleaned, by removing duplicates, and by removing repeated indicator labels in institutional sector column. In revised versions of estimates for each year, we followed revision priority logic to ensure accuracy. This ensured that analysis used most reliable estimates. Feature engineered column named 'Inflation effect' to know inflation impact. After that trend analysis is done by visualising trends for different indicators. And pivot tables are created to understand Institutional sectors, industries, subindustries trend. Analysis approach followed a top-down framework:

1. Economic Growth:

GDP trend, GDP growth rate

3. Demand-Side Analysis

PFCE --> consumer demand
GFCE --> government role

3. External Sector:

Imports vs Exports
Primary income

4. Investment & Savings:

Capital formation
Savings pattern

5. Sectoral Performance:

GVA contribution
Industry growth

6. Inflation Analysis:

Industry-level inflation impact
Real vs nominal gap

To bring all of this together, I built an interactive Power BI dashboard after python analysis structured around:
1. Economic overview
2. Demand and fiscal analysis
3. External sector
4. Investment and savings
5. Sectoral performance


Insights:

1. GDP & GDP Growth Rate Analysis:

The analysis shows a consistent increase in GDP in absolute terms, indicating sustained expansion of the economy over time. However, the declining GDP growth rate in the post-pandemic period suggests a normalization phase rather than a slowdown. This pattern is largely driven by the base effect, where the sharp economic contraction during the pandemic created a low reference point, leading to artificially high growth during recovery years. As the economy stabilizes, growth rates moderate even though total output continues to rise, reflecting a transition from recovery-driven growth to steady-state expansion.


2. Inventory Accumulation Trend:

The change in stock exhibits significant volatility across years, reflecting cyclical demand-supply imbalances within the economy. The sharp contraction during 2020–21 aligns with pandemic-induced disruptions in production and demand, while the subsequent recovery indicates normalization of inventory levels. This trend suggests that inventory adjustments played a key role in absorbing economic shocks and stabilizing production cycles post-pandemic.


3. Tax on Products Trend:

The steady increase in tax revenue over time indicates strengthening government finances, supported by economic expansion and structural reforms such as GST implementation. However, part of this growth is likely influenced by inflation, which inflates nominal tax collections. Overall, the trend reflects improved tax buoyancy alongside expanding economic activity.


4. Subsidies Analysis:

The rise in subsidies between 2019 and 2022 highlights increased government intervention during periods of economic stress. This likely reflects policy measures aimed at stabilizing prices, supporting vulnerable sectors, and cushioning the impact of external shocks such as the pandemic. It underscores the role of fiscal policy in maintaining economic stability during uncertain periods.


5. Valuables Investment Analysis:

The increasing investment in valuables, particularly during periods of declining GDP growth, indicates a shift toward risk-averse behavior. This suggests that investors and households are allocating capital into non-productive assets such as gold or precious items, reflecting reduced confidence in productive investment opportunities. Such a shift can constrain long-term economic growth by diverting resources away from capital formation.


6. Import–Export Analysis:

The persistent excess of imports over exports indicates a structural trade deficit, suggesting reliance on external goods and services. However, the simultaneous increase in both imports and exports reflects an expanding economy with deeper global integration. This trend points to rising domestic demand as well as increased participation in international trade, highlighting both opportunity and external dependency.


7. Private Final Consumption Expenditure (PFCE):

The consistent rise in PFCE indicates strong consumer demand, positioning consumption as a key driver of economic growth. This trend reflects increasing purchasing power and confidence among households, suggesting that the economy is largely demand-driven. Strong consumption patterns play a crucial role in sustaining overall economic momentum.


8. Government Final Consumption Expenditure (GFCE):

The upward trend in government spending indicates an expansionary fiscal stance with increased investment in public services. Between 2017 and 2023, the divergence between rising current prices and relatively flat constant prices suggests that much of the increase was driven by inflation rather than real growth in public services. However, post-2023, the simultaneous rise in both current and constant prices indicates genuine expansion in government activity, reflecting real improvements in service delivery and economic contribution.


9. Net Domestic Product (NDP) Analysis:

While GDP demonstrates strong growth, the comparatively slower increase in NDP highlights rising depreciation within the economy. This suggests that a significant portion of economic output is being used to maintain and replace existing capital assets rather than contributing to net value creation. It indicates potential inefficiencies in capital utilization and raises concerns about the sustainability of growth.


10. Primary Income Receivable Trend:

The increasingly negative trend in primary income from the rest of the world indicates rising income outflows to foreign entities. This reflects growing foreign investment presence and higher external financial obligations such as profit repatriation and interest payments. While this may signal strong global integration, it also highlights a structural outflow of income from the domestic economy.


11. Gross National Income (GNI) Analysis:

GNI at current prices shows a strong upward trend, indicating rising total income generated by residents, driven by both real growth and inflation. However, the slower growth in constant price GNI, especially between 2019–20 and 2022–23, suggests that much of the nominal increase is inflation-driven. The sharp recovery after 2022–23 indicates post-pandemic normalization, but the widening gap between current and constant prices highlights increasing inflationary pressures, implying that real income growth is lagging behind nominal expansion.


12. Inflation Impact on Industry & Subindustries:

Inflation impact varies significantly across industries, with sectors such as financial services, real estate, and public administration experiencing strong price-driven growth. In contrast, sectors like manufacturing, transport, and mining show relatively stable pricing, indicating growth driven more by real output. At the subindustry level, inflation is highly uneven, with areas like crops, trade services, and livestock facing higher inflation, while sectors such as metal products and water transport remain stable. This highlights localized cost pressures and demand-supply imbalances within the economy.


13. Gross Capital Formation (GCF) Analysis:

Investment patterns indicate a structural bias toward specific sectors such as real estate, trade, and transport, which show consistent upward trends and strong future growth potential. In contrast, other sectors remain relatively stagnant, suggesting uneven capital allocation. At the subindustry level, similar concentration is observed in areas like trade services and agriculture. Additionally, the increasing share of capital formation in sectors like trade, real estate, and public administration reflects shifting economic priorities and evolving growth drivers.


14. Gross Fixed Capital Formation (GFCF) – Institutional Sector:

The increasing trend in investment by households and private non-financial corporations highlights their dominant role in driving fixed asset creation. Other sectors show relatively flat trends, indicating limited contribution to long-term capital formation. This suggests that private and household sectors are key engines of investment-led growth.


15. Gross Saving Analysis:

An upward trend in savings among households and private non-financial corporations indicates increasing financial capacity within the economy. This growth in savings supports investment potential and long-term economic stability. The relatively flat trend in other sectors suggests limited contribution to overall savings accumulation.


16. Gross Value Added (GVA) Analysis:

At the institutional level, economic production is heavily concentrated in private non-financial corporations and households, with the public sector playing a more stable but less dynamic role. At the industry level, sectors such as agriculture, manufacturing, and financial services dominate value creation. This indicates sectoral concentration with a gradual shift toward high-growth industries, reflecting structural transformation in the economy.


17. GVA Growth Rate Analysis:

Growth patterns across industries are highly uneven, with some sectors showing stability while others exhibit significant volatility. Industries like trade, transport, and hospitality experienced sharp contractions during the pandemic, followed by strong recoveries, highlighting their sensitivity to economic cycles. At the subindustry level, extreme fluctuations are observed in sectors like air transport and storage, with sharp declines during disruptions and rapid rebounds afterward. This volatility underscores the cyclical and shock-sensitive nature of certain economic segments.


Impact:

The analysis helps in:

1. Identifying growth sectors
2. Understanding inflation risks
3. Evaluating investment patterns
4. Assessing economic stability



