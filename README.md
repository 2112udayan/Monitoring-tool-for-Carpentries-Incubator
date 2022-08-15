
  CS5099 Monitoring-tool-for-managing-open-source-projects



1. Description : This project focuses on building a monitoring tool to help open-source projects. Carpentries Incubator is used as an exemplar, a platform for the 
   collaborative development of domain-specific lessons for coding and data science skills. Presently only some basic information is presented on the Carpentries 
   Incubator website. This project aims to automate this process and build a monitoring tool that may be helpful to the Carpentries community managers and other 
   similar projects.
    
   This project has only been tested on Windows 11; it consists of a Monitoring tool to manage open-source projects in python, and jupyter notebook files in 
   the 'Notebook' folder.
   
2. Installation
   - requires python, preferably the latest version.
   - Only tested on Windows 11

 3. This installs all the python libraries needed.
    
   $ Use pip install -r requirements.txt to install required modules.

 4. Generate Access token
   - Verify your email address.
   - In the upper-right corner of any page, click your profile photo, then click Settings.
   - In the left sidebar, click Developer settings.
   - In the left sidebar, click Personal access tokens
   - Click Generate new token.

  5 Where to enter the access token to run the code.
   - Refer to the notebook file -named -Setup_API.ipynb
   - Enter the Personal access token in  "INSERT CODE HERE".

   To view the jupyter projects, open jupyter notebook using the command line in the top directory with:
   
   $ jupyter notebook

   Select the .ipynb files in the 'Notebook' folder and run cells using the Jupyter notebook interface. Run all cells at once or 'Shift+Enter' to run the individual      cell.

  6 List of Notebook files to analyse the each stage of tool development.
   - Setup_API.ipynb ---is an indicator to insert the personal token to each notebook file to authenticate before excecuting the further code .
   - Data_Extraction.ipynb--- contains a function to retrieve consolidated data such as commit data , open pull request data , open issues data , list of labels, life      cycle stage of each repsoitories as an individual file in json format.
   - Indicators_of_each_repositories.ipynb---Contains individual functions to get an overview of an each parameter of the repsoistories such as "repo_name","open_PR",      "closed_PR","closed_issues","open_issues","stargazers_count of 111 repsoitories .
   - Monitoring-tool-for-Carpentries-Incubator---contains a function to get the total count of ( allcategories (Issue_count, Pr_count, Stagazers_count &                    contributors_count).
   - Carpentries_dashboard.ipynb---Contains a function to display the dashboard of Carpentries Incubator website ( Repository name , Lesson title, Last updated date ,      List of topics ,life cycle stage , label count)
   - Collaborative-aspect.ipynb---Contains functions to get the commit count and contributors , issues count and contributors , pulls count and contributors.
   - Analysis.ipynb--- Contains functions to plot a histogram and Collaboration graph.
   
   Credits:

  Special thanks to Dr Olexandr Konovalov:)

## Appendix

Any additional information goes here


## Documentation

Link to get the API url for available resource in the REST API-- https://docs.github.com/en/rest

Link to PyGithub documentation - https://pygithub.readthedocs.io/en/latest/introduction.html

Link to The Carpentries website- https://carpentries.org/community-lessons/

Link to the Carpentries Incubator - https://carpentries-incubator.org/

Link to Carpentries Incubator GitHub Account- https://github.com/carpentries-incubator/

## Acknowledgements

 - [Awesome Readme Templates](https://awesomeopensource.com/project/elangosundar/awesome-README-templates)
 - [Awesome README](https://github.com/matiassingers/awesome-readme)
 - [How to write a Good readme](https://bulldogjob.com/news/449-how-to-write-a-good-readme-for-your-github-project)


## API Reference

#### Get all items

```http
  GET /api/items
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `api_key` | `string` | **Required**. Your API key |

#### Get item

```http
  GET /api/items/${id}
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `id`      | `string` | **Required**. Id of item to fetch |

#### add(num1, num2)

Takes two numbers and returns the sum.

