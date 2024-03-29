
# Monitoring tool for the Carpentries Incubator
 
 This Project done as CS5099 module at the University of St Andrews under Dr Olexandr Konovalov's  supervision.
  
  
1. Description :
   This project focuses on building a monitoring tool to help open-source projects. Carpentries Incubator is used as an exemplar, a platform for the 
   collaborative development of domain-specific lessons for coding and data science skills. Presently only some basic information is presented on the Carpentries 
   Incubator website. This project aims to automate this process and build a monitoring tool that may be helpful to the Carpentries community managers and other 
   similar projects.
    
   This project consists of a Monitoring tool to manage open-source projects in python, and jupyter notebook files in 
   the 'Notebook' folder.
   
2. Installation
    - requires python, preferably the latest version

 3. This installs all the python libraries needed.
    
    $ Use pip install -r requirements.txt to install required modules.

 4. Generate GitHub personal access token at https://github.com/settings/tokens

 5. Where to enter the access token to run the code.
  
    - The token should be stored in the file `~/.github_shell_token`
      in your home directory
      
    To view the jupyter projects, open jupyter notebook using the command line in the top directory with:
   
    $ jupyter notebook

    Select the .ipynb files in the 'Notebook' folder and run cells using the Jupyter notebook interface. 
    Run all cells at once or 'Shift+Enter' to run the individual cell.

 6. List of Notebook files to analyse the each stage of tool development.
     
    - Data_Retrieval.ipynb--- contain functions to retrieve consolidated data of parameters such as commit data , 
      open pull request data , open issues data , list of labels, life cycle stage of each repositories as an 
      individual file in json format.The commit_user_details() function used in this file for the commit user data       
      retrieval was provided by the project supervisor.
    
    - Repository_Indicators.ipynb---Contains individual functions to get an overview of an every parameter of the
      repsoistories with lesson such as "repo_name","open_PR","closed_PR","closed_issues","open_issues","stargazers_count" .
    
    - Lesson_Information_Dashboard.ipynb---Contain functions  to display the dashboard of Carpentries Incubator website 
      (Repository name , Lesson title, Last updated date ,List of topics ,life cycle stage , label count) and also has a
      function to get the total count of all categories (Issue_count, Pr_count,Stagazers_count).
    
    - Collaborative-Aspects.ipynb---Contains functions to get the commit count,issues count pull requests count and their 
      contributors and total contributors. It also contain a code to get average number of contributors for a lesson 
      (classifying by different stages: pre-alpha, alpha, beta, stable).Addionally, shows average of total contributors of a lesson 
      (classifying by different stages:pre-alpha, alpha, beta,stable).
    
    - Data_Visualisation.ipynb---Contain functions to plot a histogram and Collaboration graph.
  


## Documentation

 REST API Documnetation-- https://docs.github.com/en/rest

 PyGithub documentation - https://pygithub.readthedocs.io/en/latest/introduction.html
 
 The Carpentries website- https://carpentries.org/community-lessons/

 Carpentries Incubator - https://carpentries-incubator.org/

 Carpentries Incubator GitHub Account- https://github.com/carpentries-incubator/


