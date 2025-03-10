# Data Visualization

## Assignment 3: Final Project

### Requirements:
- We will finish this class by giving you the chance to use what you have learned in a practical context, by creating data visualizations from raw data. 
- Choose a dataset of interest from the [City of Toronto’s Open Data Portal](https://www.toronto.ca/city-government/data-research-maps/open-data/) or [Ontario’s Open Data Catalogue](https://data.ontario.ca/). 
- Using Python and one other data visualization software (Excel or free alternative, Tableau Public, any other tool you prefer), create two distinct visualizations from your dataset of choice.  

https://data.ontario.ca/dataset/5472ffc1-88e2-48ca-bc9f-4aa249c1298d/resource/d5d8f478-765c-4246-b8a7-c3b13a4a1a41/download/outbreak_cases.csv

Code and the outputs: please see file "Assignment-3-code.ipynb" 

- For each visualization, describe and justify: 
    > What software did you use to create your data visualization?
      My answer: Jupter Notebook

    > Who is your intended audience? 
      My answer:
      1. Public Health Officials & Epidemiologists
      2. General Public & At-Risk Communities 
      3. Healthcare Workers & Hospitals
      4. Researchers & Data Scientists
      5. Policymakers & Government Agencies 
      6. Media & Journalists

    
    > What information or message are you trying to convey with your visualization? 
    My answer:
      I'm trying to visualize the:
      1. Summary of cases associated with outbreaks, by outbreak setting and date
      2. the trend over time periods

    
    > What design principles (substantive, perceptual, aesthetic) did you consider when making your visualization? How did you apply these principles? With what elements of your plots? 
    My answer:
    1. Substantive Principles (What Information to Show?)
       These principles focus on the clarity and accuracy of the data representation.
     - How I Applied It:
          Grouped data by time periods (monthly and quarterly) to summarize the dataset without overwhelming the viewer.
          Used different plot types (Bar, Scatter, Line) to represent:
          Aggregated cases
          Distribution of cases
          Temporal trends
          Split the data by category_grouped to help identify patterns across different outbreak categories.
    2. Perceptual Principles (How Information is Shown?)
       These principles ensure the visualization is easy to read and understand by the human eye.
     - How I Applied It:
          Used consistent color palettes (sns.color_palette() automatically assigns unique hues to each category).
          Chose different chart types:
          Bar plot for comparison of categories.
          Scatter plot to emphasize distribution and variation across quarters.
          Line plot to highlight trends over time.
          Made grid lines smaller with adjusted font sizes to avoid visual clutter while still guiding the eye.
          Applied legends with smaller sizes to avoid distracting from the main data.
    3. Aesthetic Principles (How the Plot Looks?)
       These principles improve the visual appeal of the plot while keeping it functional.
     - How I Applied It:
          Used a mosaic layout to arrange multiple visualizations without crowding.
          Balanced white space with plt.tight_layout() to make the layout clear and not cramped.
          Applied color consistency across all three plots, so the same categories always have the same color.
          Added titles for each plot to guide the reader at a glance.
          Rotated axis labels (45 degrees for better readability).
    
    > How did you ensure that your data visualizations are reproducible? If the tool you used to make your data visualization is not reproducible, how will this impact your data visualization? 
    My answer:
       Ensuring reproducibility in data visualizations is crucial for maintaining trust and reliability in the results. Here's how I ensured that the visualizations are reproducible:
    1. Use of Open-Source Libraries. The tools I used, such as Pandas, Seaborn, and Matplotlib, are open-source Python libraries widely used in the data science community.
       These libraries are well-documented and widely supported, ensuring that others can easily reproduce the visualizations when using the same tools and techniques.They allow others to run the same code on their machines (given the same dataset) to reproduce identical results.
    2. Clear code structure and well-defined plotting parameters contribute to consistency. I used specific plot parameters like:
         --Fixed color palettes (sns.color_palette())
         --Specified font sizes and layout using plt.tight_layout()
    3. Consistent Randomization (If Any): For this particular case, no randomization is used, which means results are deterministic. Re-running the same code with the same input data will produce identical plots each time.


    > How did you ensure that your data visualization is accessible?  
    My answer:
    1. Color Choices for Better Accessibility 
       -- To avoidi Color Ambiguity, I used Seaborn’s color palettes, specifically sns.color_palette("tab10"), which is designed for distinguishable colors. This ensures that people with color blindness can differentiate categories.
    2. I used multiple visual Cues for clarity. On the scatter Plot, I used shapes instead of just colors.
    3. To improve text readability and layout, i adjusted font size for readability. I set font sizes explicitly for:
        --Titles (fontsize=14) – Large enough for clarity.
        --Tick Labels (fontsize=10) – Clear but not overwhelming.
        --Annotations (fontsize=8) – Small but still legible.
        --Used fontsize=10 for legends to keep them readable but not overpowering.

    > Who are the individuals and communities who might be impacted by your visualization? 
    My answer:
    The individuals and communities impacted by my visualization depend on the context of the outbreak data being analyzed. Below are the key stakeholders who may be affected and how they might use or interpret the visualization.
    1. Public Health Officials & Epidemiologists: 
          use data-driven insights to track the spread of diseases, allocate resources, plan interventions, and develope policies.
    2. General Public & At-Risk Communities: 
          This data visualization could bring community awareness, vulunerable group can take precautionary measures based on trends in the data. Individuals may use the visualization to assess risk levels and adjust their behaviorIndividuals may use the visualization to assess risk levels and adjust their behavior 
    3. Healthcare Workers & Hospitals
          If cases spike in specific months or categories, hospitals can prepare for an increase in admissions (e.g., allocating more ICU beds), and manage workload.
    4. Researchers & Data Scientists
          Researchers can analyze patterns over time to predict future outbreaks.The dataset can be used to train predictive models for forecasting future cases.
    5. Policymakers & Government Agencies 
          If certain categories show persistent high case counts, governments may allocate more resources such as funding to affected groups.
          Officials may introduce new policies (e.g., mandatory vaccinations, mask mandates) based on visualized trends.
    6. Media & Journalists
          Journalists rely on clear and accurate data to report outbreak trends to the public.
          News organizations may use visualized data to advocate for healthcare reforms.


    > How did you choose which features of your chosen dataset to include or exclude from your visualization? 
     My answer:
    When choosing which features (columns) of the dataset to include or exclude in the visualization, I followed a systematic approach based on relevance, clarity, and interpretability. Here’s how I made these decisions:
    1. Features Included & Why: I selected 'date', 'category_grouped' and 'Total_cases' for visualization.These features allow us to:
        --Track case trends over time (by month/quarter).
        --Compare different categories .
        --Aggregate data for meaningful insights without excessive granularity.
    2. Features Excluded & Why : 'outbreak_subgroup' was not included beacuse it had too many subgroups,which would make the plots hard to read.
    3. Aggregation Choices & Why:
        --Monthly & Quarterly Aggregation:Instead of daily data (which can be noisy), I aggregated cases by month & quarter to show clear trends. The quarterly trend seemed lost some details, so I kept monthly trend which smoothed out random fluctuations while keeping meaningful patterns.
        --Line plots were used for monthly trends (better for showing progression over time).
        --Stacked Bar & scatter Plots:Bar plots were chosen for quarterly cases (better for comparing categories).

    > What ‘underwater labour’ contributed to your  final data visualization product?
     My answer:
     Here’s what went into making the final visualization:
     1. Getting the data: I tried using Python grabing data from the URL. Unfortunately it seems get the meta data but not the real dataset.The I downloaded the dateset to local then read it to VS.
     2. Data Cleaning & Preparation:Before even creating the plots, I had to preprocess the dataset to ensure accuracy.
     3. Choosing the Right Plot Types & Layout: I tested multiple visualization styles before finalizing the best ones
     4. Fine-Tuning Aesthetics & Readability: color choices,legend optimization,ddjusted font size & color to match bar/dot colors for subtle readability.

- This assignment is intentionally open-ended - you are free to create static or dynamic data visualizations, maps, or whatever form of data visualization you think best communicates your information to your audience of choice! 
- Total word count should not exceed **(as a maximum) 1000 words** 
 
### Why am I doing this assignment?:  
- This ongoing assignment ensures active participation in the course, and assesses the learning outcomes: 
* Create and customize data visualizations from start to finish in Python
* Apply general design principles to create accessible and equitable data visualizations
* Use data visualization to tell a story  
- This would be a great project to include in your GitHub Portfolio – put in the effort to make it something worthy of showing prospective employers!

### Rubric:

| Component         | Scoring  | Requirement                                                                 |
|-------------------|----------|-----------------------------------------------------------------------------|
| Data Visualizations | Complete/Incomplete | - Data visualizations are distinct from each other<br>- Data visualizations are clearly identified<br>- Different sources/rationales (text with two images of data, if visualizations are labeled)<br>- High-quality visuals (high resolution and clear data)<br>- Data visualizations follow best practices of accessibility |
| Written Explanations | Complete/Incomplete | - All questions from assignment description are answered for each visualization<br>- Explanations are supported by course content or scholarly sources, where needed |
| Code              | Complete/Incomplete | - All code is included as an appendix with your final submissions<br>- Code is clearly commented and reproducible |

## Submission Information

🚨 **Please review our [Assignment Submission Guide](https://github.com/UofT-DSI/onboarding/blob/main/onboarding_documents/submissions.md)** 🚨 for detailed instructions on how to format, branch, and submit your work. Following these guidelines is crucial for your submissions to be evaluated correctly.

### Submission Parameters:
* Submission Due Date: `23:59 - 09/03/2025`
* The branch name for your repo should be: `assignment-4`
* What to submit for this assignment:
    * A folder/directory containing:
        * This file (assignment_3.md)
        * Two data visualizations 
        * Two markdown files for each both visualizations with their written descriptions.
        * Link to your dataset of choice.
        * Complete and commented code as an appendix (for your visualization made with Python, and for the other, if relevant) 
* What the pull request link should look like for this assignment: `https://github.com/<your_github_username>/visualization/pull/<pr_id>`
    * Open a private window in your browser. Copy and paste the link to your pull request into the address bar. Make sure you can see your pull request properly. This helps the technical facilitator and learning support staff review your submission easily.

Checklist:
- [ ] Create a branch called `assignment-3`.
- [ ] Ensure that the repository is public.
- [ ] Review [the PR description guidelines](https://github.com/UofT-DSI/onboarding/blob/main/onboarding_documents/submissions.md#guidelines-for-pull-request-descriptions) and adhere to them.
- [ ] Verify that the link is accessible in a private browser window.

If you encounter any difficulties or have questions, please don't hesitate to reach out to our team via our Slack. Our Technical Facilitators and Learning Support staff are here to help you navigate any challenges.
