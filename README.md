# Project: Analyzing the Relationship between Sustainable Development Goals (SDGs) and Country-Level Performance

## Project Overview
This project examines the quantitative relationship between global Sustainable Development Goals (SDGs) and each country’s performance on individual SDG scores. The study leverages statistical and machine learning methods to assess how the 17 individual SDGs collectively contribute to the overall SDG Index for various countries. The results provide actionable insights to policymakers for resource allocation and prioritization, helping to enhance global efforts toward sustainable development.

## Tools and Techniques Used
- **RStudio**
  - Data cleaning to inspect null values
  - Summary statistics
  - Multiple linear regression
  - Decision tree modeling
  - Data visualizations

## Exploratory Data Analysis
Through Exploratory Data Analysis (EDA), patterns and correlations between each SDG score and the SDG Index were uncovered, providing answers to key research questions on sustainable development. The analysis identified the SDGs that most significantly impact the overall index, highlighting areas that require further attention.

## Modeling and Analysis
- **Multiple Linear Regression**: Quantified the relationship between individual SDG scores (independent variables) and the SDG Index (dependent variable), identifying the goals with the greatest positive impact on the SDG Index.
- **Decision Tree**: Implemented to identify key drivers among the SDGs, offering a visual and interpretable understanding of how each goal influences the SDG Index, and providing targeted policy insights.

## Results and Findings of Decision Tree

### Goal 1 - No Poverty
- If the score falls below 47 for Goal 1, these countries are further categorized under a new internal node.
- This group, consisting of 55 observations (18% of the dataset), represents countries facing poverty-related challenges and striving to reduce poverty levels.
- Within this subset, 53 observations (10% of the dataset) have a goal score lower than 47, indicating a significant portion of the population may experience poverty or economic hardship.
- The remaining observations, with scores exceeding 47, are classified into the right terminal node, indicating a smaller proportion of the population experiencing extreme poverty.
- Countries in this subset under Goal 6 with scores less than 78 likely face challenges related to poverty and clean water access.

### Goal 3 - Good Health and Well-being
- Countries scoring below 58 on Goal 3 account for 34% of the dataset, indicating challenges in health and well-being, such as inadequate healthcare infrastructure, access to services, and disease prevention.
- Countries whose Goal 3 score exceeds 58 are further subset into Goal 6, which focuses on ensuring clean water and sanitation.

### Goal 4 - Quality Education
- For countries with an SDG 4 score below 42, the decision tree examines Goal 11 (Sustainable Cities and Communities).
- Countries with low education scores may also struggle with urban sustainability, indicating potential issues with access to quality education or educational infrastructure in urban areas.
- Countries where the Goal 4 score exceeds 42 represent those with relatively stronger indicators for quality education and are further classified under Goal 1 (No Poverty).

### Goal 6 - Clean Water and Sanitation
- For countries where Goal 6 scores fall below 78, observations are grouped under Goal 1, which addresses poverty reduction.
- This grouping includes 67 observations (46% of the dataset), indicating that many countries focus on poverty reduction despite facing water and sanitation challenges.
- Countries with Goal 6 scores above 78 represent 20% of the dataset and generally have better access to clean water and sanitation.

### Goal 8 - Development and Transfer of Technology
- Countries with high Goal 8 scores often focus on global partnerships and knowledge sharing, supporting sustainable economic growth.

### Goal 11 - Sustainable Cities and Communities
- Countries with Goal 11 scores below 33 (4% of the dataset) may face urban development challenges such as inadequate infrastructure, urban planning, or environmental sustainability issues.

### Goal 17 - Partnerships for the Goals
- Countries focusing on Goals 1, 17, or 18 emphasize partnerships and global cooperation for sustainable development, which is essential for achieving multi-sectoral impacts.

## Insights and Recommendations

### Goal 1 - No Poverty
- **Insight**: Countries scoring below 47 face significant poverty challenges, with many also struggling with clean water and sanitation.
- **Recommendation**: Prioritize integrated poverty reduction and water sanitation programs, and allocate resources to countries with low Goal 1 scores, exploring partnerships focused on poverty alleviation and water sanitation.

### Goal 3 - Good Health and Well-being
- **Insight**: About 34% of countries score below 58, showing substantial gaps in healthcare access and infrastructure, often requiring improvements in clean water and sanitation.
- **Recommendation**: Strengthen healthcare infrastructure, focusing on preventive care and community health. Recognize the synergy between health and water access, implementing initiatives to improve both healthcare and sanitation.

### Goal 4 - Quality Education
- **Insight**: Low scores in education often correlate with urban development challenges.
- **Recommendation**: Improve access to quality education, especially in urban and underdeveloped areas. Support community-specific educational programs and partnerships with urban planning organizations.

### Goal 6 - Clean Water and Sanitation
- **Insight**: A significant portion of countries struggle with water and sanitation, impacting poverty levels.
- **Recommendation**: Invest in water infrastructure and promote educational programs on water management to encourage sustainable practices.

### Goal 8 - Development and Transfer of Technology
- **Insight**: High scores on Goal 8 reflect a strong focus on global partnerships and knowledge sharing.
- **Recommendation**: Strengthen international partnerships supporting economic development and technology transfer, encouraging sustainable growth strategies aligned with broader SDG priorities.

### Goal 11 - Sustainable Cities and Communities
- **Insight**: Countries with low Goal 11 scores face urban development challenges.
- **Recommendation**: Invest in sustainable urban planning, focusing on infrastructure and community engagement to address sustainability needs.

### Goal 17 - Partnerships for the Goals
- **Insight**: A commitment to partnerships and global cooperation is critical for achieving multi-sectoral impacts.
- **Recommendation**: Facilitate cross-border collaborations that enhance resource sharing and align with SDG priorities, focusing on impactful projects across these goals.

### Overall Strategic Recommendations
- **Cross-Goal Synergies**: Recognize interdependencies between goals, such as poverty and water, or education and urban development, to catalyze improvements.
- **Customized Country Programs**: Tailor programs to individual countries based on their greatest needs and gaps.
- **Policy Prioritization**: Develop policies that leverage international partnerships, amplifying resources and expertise for achieving SDGs.

## Limitations
- **Model Limitations**: The current model does not account for weighted variables or the exact calculation of the SDG Index, limiting the analysis of nuanced relationships.
- **Stakeholder Perspectives**: Varying perspectives on the effectiveness of the SDGs may challenge stakeholder buy-in for recommendations based on this study.
- **Lack of Temporal Analysis**: The research is cross-sectional and does not capture temporal changes, potentially missing trends over time.
