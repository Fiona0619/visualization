# Data Visualization

## Assignment 2: Good and Bad Data Visualization

### Requirements:

- Data visualizations are important tools for communication and convincing; we need to be able to evaluate the ways that data are presented in visual form to be critical consumers of information 
- To test your evaluation skills, locate two public data visualizations online, one good and one bad  
    - You can find data visualizations at https://public.tableau.com/app/discover or https://datavizproject.com/, or anywhere else you like! 
- For each visualization (good and bad):  
    - Explain (with reference to material covered up to date, along with readings and other scholarly sources, as needed) why you classified that visualization the way you did.
      ```
      Your answer...

Certainly! Here are two public data visualizations from the provided sources—one exemplary and one suboptimal—along with explanations for their classifications:

### Good Visualization: Visualization: Global CO2 Emissions by Country 
https://public.tableau.com/app/profile/daniel.stone6313/viz/GlobalCO2byCountryandYear/Dashboard1

This visualization, available on Tableau Public, serves as a comprehensive guide to selecting appropriate chart types based on the data relationship one aims to convey. Inspired by the Financial Times' Visual Vocabulary, it categorizes various chart types and provides interactive examples for each.

*Why it's good one*

1. Interactive Map: The visualization features an interactive world map where users can hover over countries to view specific CO2 emission data, enhancing user engagement and understanding.

2. Temporal Analysis: It includes a timeline slider, allowing users to observe how emissions have changed over the years, facilitating temporal comparisons.

3. Clear Legends and Labels: The use of intuitive color gradients and clear labeling ensures that the information is accessible and easy to interpret.

4. Data Source Transparency: The visualization provides information about data sources, ensuring credibility and allowing users to delve deeper if desired.


### Bad Visualization:"3D Pie Chart of Sales Distribution"
https://public.tableau.com/app/profile/balaram3041/viz/3DPieChart/3DPie

*Why it's bad one*

1. Use of 3D Effects: Implementing 3D elements in pie charts can distort the perception of data, making it challenging to accurately compare segments.

2. Overcomplication: The addition of a third dimension does not provide additional insight but rather complicates the visualization unnecessarily.

3. Color Choices: Utilizing similar hues for adjacent segments can make differentiation difficult, leading to potential misinterpretation.


      ```
    - How could this data visualization have been improved?  
      ```
      Your answer...
### The good visulization:  though "Global CO2 Emissions by Country" is a well-designed visualization, there are still ways to improve it for better clarity and usability. Here are some potential enhancements:

1. Improve Color Scale for Readability
Issue: Some world map visualizations use color gradients that make it hard to differentiate between similar values (e.g., light shades of the same color).
Fix: Use a diverging color scheme where low emissions are clearly distinct from high emissions (e.g., light blue for low emissions, dark red for high emissions).
2. Provide a Normalized Metric
Issue: The visualization likely shows total CO2 emissions by country, which favors large economies/populations (e.g., China, the US) and can be misleading.
Fix: Include per capita CO2 emissions or CO2 emissions per GDP unit to provide a fair comparison between countries of different sizes.
3. Add a Comparison Feature
Issue: While users can hover over countries, there may be no easy way to compare emissions between selected countries.
Fix: Allow users to select multiple countries and display side-by-side comparisons or trend lines over time.
4. Enhance Time-Series Analysis
Issue: If the timeline slider is the only way to track changes, users might struggle to see overall trends.
Fix: Add line charts or bar charts below the map to show how emissions have changed for selected countries over time.
5. Show Data Sources and Uncertainty
Issue: Some countries may have unreliable or missing data, which can affect accuracy.
Fix: Provide data source details and indicate uncertainty levels (e.g., shaded areas or confidence intervals).

This visualization is already strong, but adding per capita metrics, better interactivity, and enhanced comparisons would make it even more insightful and user-friendly.

### To improve the "3D Pie Chart of Sales Distribution" visualization, consider the following changes:

1. Remove the 3D Effect
Why? The 3D perspective distorts the size of pie slices, making comparisons difficult.
Fix: Use a 2D pie chart instead for better readability and accuracy.
2. Consider a Bar Chart Instead
Why? A pie chart is only effective when comparing a small number of categories (ideally 2-5). If there are many segments, reading precise proportions becomes difficult.
Fix: A bar chart (horizontal or vertical) provides a clearer comparison of sales distribution, especially if categories have similar values.
3. Improve Color Choices
Why? If adjacent slices have similar colors, they become difficult to differentiate.
Fix: Use a well-contrasted color palette, ensuring each segment is distinct.
4. Add Data Labels or Percentages
Why? Without labels, users must estimate segment sizes, which can lead to misinterpretation.
Fix: Display percentages or absolute values on each segment to clarify the distribution.
5. Use Sorting for Better Comparisons
Why? Randomly placed slices make it harder to compare.
Fix: Order slices from largest to smallest for a more intuitive visual flow.

Afterall, if the dataset has many categories, replacing the pie chart with a bar chart would make comparisons much easier. However, if keeping a pie chart, ensuring it is 2D, well-labeled, and color-distinct would significantly improve its effectiveness.

      ```
- Word count should not exceed (as a maximum) 500 words for each visualization (i.e. 
300 words for your good example and 500 for your bad example)

### Why am I doing this assignment?:

- This assignment ensures active participation in the course, and assesses the learning outcomes
* Apply general design principles to create accessible and equitable data visualizations
* Use data visualization to tell a story

### Rubric:

| Component               | Scoring   | Requirement                                                 |
|-------------------------|-----------|-------------------------------------------------------------|
| Data viz classification and justification | Complete/Incomplete | - Data viz are clearly classified as good or bad<br />- At least three reasons for each classification are provided<br />- Reasoning is supported by course content or scholarly sources |
| Suggested improvements  | Complete/Incomplete | - At least two suggestions for improvement<br />- Suggestions are supported by course content or scholarly sources |

## Submission Information

🚨 **Please review our [Assignment Submission Guide](https://github.com/UofT-DSI/onboarding/blob/main/onboarding_documents/submissions.md)** 🚨 for detailed instructions on how to format, branch, and submit your work. Following these guidelines is crucial for your submissions to be evaluated correctly.

### Submission Parameters:
* Submission Due Date: `23:59 - 02/03/2025`
* The branch name for your repo should be: `assignment-2`
* What to submit for this assignment:
    * This markdown file (assignment_2.md) should be populated and should be the only change in your pull request.
* What the pull request link should look like for this assignment: `https://github.com/<your_github_username>/visualization/pull/<pr_id>`
    * Open a private window in your browser. Copy and paste the link to your pull request into the address bar. Make sure you can see your pull request properly. This helps the technical facilitator and learning support staff review your submission easily.

Checklist:
- [done ] Create a branch called `assignment-2`.
- [done] Ensure that the repository is public.
- [done ] Review [the PR description guidelines](https://github.com/UofT-DSI/onboarding/blob/main/onboarding_documents/submissions.md#guidelines-for-pull-request-descriptions) and adhere to them.
- [done ] Verify that the link is accessible in a private browser window.

If you encounter any difficulties or have questions, please don't hesitate to reach out to our team via our Slack. Our Technical Facilitators and Learning Support staff are here to help you navigate any challenges.
