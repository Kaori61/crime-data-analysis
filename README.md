# London Business Crime analysis

**London Business Crime Analysis** is is a personal capstone project focused on the ETL (Extract, Transform, Load) pipeline in Jupyter Notebook and visualisations. 

The project examines business-related crimes (any criminal offence that is committed against a person or property which is associated by the connection of that person or property to a business.) across London boroughs, using publicly available police data. The goal of this analysis is to uncover trends in types crimes, identify crime rates in different boroughs and generte insights to inform better resource allocation.

# ![CI logo](https://codeinstitute.s3.amazonaws.com/fullstack/ci_logo_small.png)


## Dataset Content
* London Business Crime dataset is publically available data that can be downloaded from here [London Datastore](https://data.london.gov.uk/dataset/mps-business-crime-dashboard-data/). The data contains a range of records of crimes such as date, borough, type of crime and more.


## Business Requirements
* Monitor borough performance.
* Identify crime types that need attention.
* Improve case closure rate.

## Hypothesis and how to validate?
* List here your project hypothesis(es) and how you envision validating it (them) 

## Project Plan
* Outline the high-level steps taken for the analysis.
* How was the data managed throughout the collection, processing, analysis and interpretation steps?
* Why did you choose the research methodologies you used?

## The rationale to map the business requirements to the Data Visualisations
* List your business requirements and a rationale to map them to the Data Visualisations

## Analysis techniques used
* List the data analysis methods used and explain limitations or alternative approaches.
* How did you structure the data analysis techniques. Justify your response.
* Did the data limit you, and did you use an alternative approach to meet these challenges?
* How did you use generative AI tools to help with ideation, design thinking and code optimisation?

## Ethical considerations
* This project uses anonymised, publicly available data with no personally identifiable information. Ethical considerations regarding privacy and confidentiality have been fully observed.


## Dashboard Design
* List all dashboard pages and their content, either blocks of information or widgets, like buttons, checkboxes, images, or any other item that your dashboard library supports.
* Later, during the project development, you may revisit your dashboard plan to update a given feature (for example, at the beginning of the project you were confident you would use a given plot to display an insight but subsequently you used another plot type).
* How were data insights communicated to technical and non-technical audiences?
* Explain how the dashboard was designed to communicate complex data insights to different audiences. 

## Unfixed Bugs
* Please mention unfixed bugs and why they were not fixed. This section should include shortcomings of the frameworks or technologies used. Although time can be a significant variable to consider, paucity of time and difficulty understanding implementation are not valid reasons to leave bugs unfixed.
* Did you recognise gaps in your knowledge, and how did you address them?
* If applicable, include evidence of feedback received (from peers or instructors) and how it improved your approach or understanding.

## Development Roadmap
* What challenges did you face, and what strategies were used to overcome these challenges?
* What new skills or tools do you plan to learn next based on your project experience? 
* I had issues activating my Python virtual environment (`.venv`) in Git Bash while using the default MINGW64 shell — VS Code wasn't detecting the environment, and key packages like `pandas` weren't working. After some changes to `.bashrc`, Git Bash began launching in the MSYS shell, which added confusion by showing duplicate prompts like (`.venv`) (`.venv`).
With help from ChatGPT, I diagnosed the issue, fixed my .bashrc configuration, selected the correct interpreter in VS Code, and installed missing packages like ipykernel.
* Plotly wasn't working properly on Jupyter Notebook. It kept showing me the error message "nbformat >=4.2.0 isn't installed" even though I had correct version installed. Thanks to two of my fellow students Celia and Jane, who helped me fix this issue. I was able to create Plotly graphs. 

## Deployment
### Heroku

* The App live link is: https://YOUR_APP_NAME.herokuapp.com/ 
* Set the runtime.txt Python version to a [Heroku-20](https://devcenter.heroku.com/articles/python-support#supported-runtimes) stack currently supported version.
* The project was deployed to Heroku using the following steps.

1. Log in to Heroku and create an App
2. From the Deploy tab, select GitHub as the deployment method.
3. Select your repository name and click Search. Once it is found, click Connect.
4. Select the branch you want to deploy, then click Deploy Branch.
5. The deployment process should happen smoothly if all deployment files are fully functional. Click now the button Open App on the top of the page to access your App.
6. If the slug size is too large then add large files not required for the app to the .slugignore file.

## Conclusion
* Write conclusion of the analysis

## Main Data Analysis Libraries
* Here you should list the libraries you used in the project and provide an example(s) of how you used these libraries.


## Credits 

* In this section, you need to reference where you got your content, media and extra help from. It is common practice to use code from other repositories and tutorials, however, it is important to be very specific about these sources to avoid plagiarism. 
* You can break the credits section up into Content and Media, depending on what you have included in your project. 
* [GeekforGeeks](https://www.geeksforgeeks.org/) - used to aid in code generation.



### Content 

- The text for the Home page was taken from Wikipedia Article A
- Instructions on how to implement form validation on the Sign-Up page was taken from [Specific YouTube Tutorial](https://www.youtube.com/)
- The icons in the footer were taken from [Font Awesome](https://fontawesome.com/)

### Media

- The photos used on the home and sign-up page are from This Open-Source site
- The images used for the gallery page were taken from this other open-source site



## Acknowledgements (optional)
* Thank the people who provided support through this project.
