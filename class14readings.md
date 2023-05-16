# The key differences between Matplotlib, Seaborn, and Bokeh libraries in terms of their features and use cases
Matplotlib is a highly customizable library that provides a wide range of plots and graphs. It is the most commonly used data visualization library in Python. Matplotlib is suitable for creating basic and complex plots and offers fine-grained control over many aspects of a plot's appearance. It supports a variety of plot types, including line, scatter, bar, histogram, and 3D plots. Matplotlib is a low-level library, meaning that it requires more code to generate complex visualizations. However, it is highly customizable and can produce high-quality output suitable for publication.

Seaborn is a higher-level library built on top of Matplotlib that provides more streamlined, aesthetically pleasing, and informative visualizations. It offers several advanced data visualizations, such as heat maps, violin plots, and categorical plots, that are not available in Matplotlib. Seaborn simplifies the process of generating complex visualizations by providing default styles and color palettes, and it allows for easy customization. Seaborn is best suited for exploratory data analysis and data visualization tasks.

Bokeh is a library that allows for interactive visualization, enabling the user to create dynamic, web-based visualizations that can be embedded in web applications. It is suitable for creating interactive dashboards and complex visualizations with interactive widgets. Bokeh supports multiple output formats and offers a high level of interactivity, including hover tooltips and linked plots. Bokeh requires less code than Matplotlib for interactive visualizations, but it requires some knowledge of web development.

## the main functions to create relational, categorical, and distribution plots
1- Relational plots:
* Function: sns.relplot()
* Purpose: To create visualizations that show the relationship between two continuous variables. These plots are useful for exploring trends and patterns in data.
* Example use case: A scatter plot showing the relationship between a person's age and their income.

2- Categorical plots:
* Functions: sns.catplot() and sns.boxplot()
* Purpose: To create visualizations that show the distribution of a categorical variable or the relationship between a categorical variable and a continuous variable.
* Example use case: A box plot showing the distribution of test scores by grade level.

3- Distribution plots:
* Functions: sns.histplot(), sns.kdeplot(), and sns.rugplot()
* Purpose: To create visualizations that show the distribution of a single variable or the relationship between two variables. These plots are useful for understanding the shape and spread of data.
* Example use case: A histogram showing the distribution of ages in a population.

## things I want to learn more about
