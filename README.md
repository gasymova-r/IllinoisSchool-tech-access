# Illinois-School-tech-access
The project uses data from the [Illinois State Board of Education](https://www.isbe.net/Pages/Data-Analysis-Reports.aspx) in an attempt to define which school districts in Illinois experience the most technology accessibility issues and potentially need more funding. We then attempt to identify the underlying reasons for disproportions using machine learning models.

The "code" R Markdown file outputs an HTML file thoroughly describing the analysis (data wrangling, feature engineering, assessment of NAs, variable distributions, etc.).

The final conclusions were made based on two main visualizations:
1. Cleveland Dot Plot demonstrating schools with the highest gap between Internet access demand and supply
2. bar chart showcasing the schools with the lowest number of devices available per student


The "model" R Markdown file completes the analysis by providing both regression and classification approaches to identifying feature importance. This represents a rather unusual application of machine learning: we did not create a machine learning pipeline for the sake of prediction alone, rather - **use it for the purposes of analysis and proof of underlying trends**. By looking at what a machine can predict from the given data it seems possible to reveal the flaws in human judgment. Both classification and regression models mostly base **their predictions on the percentage of Asian and White populations in schools**. This, furthermore, demonstrates how biases can be engraved into data. If we were to ask an algorithm to assign Illinois School Districts with devices for next year based on previous history, it would most likely disproportionately favor the schools with higher percentages of Asian and White populations. Thus, hopefully, this project is able to demonstrate how crucial it is to consider the flaws of existing data and the limits of ML applications.
