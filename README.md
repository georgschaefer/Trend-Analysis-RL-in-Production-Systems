# Quantitative Trend Analysis of Reinforcement Learning Algorithms in Production Systems

This repository contains the code for the extended abstract "Quantitative Trend Analysis of Reinforcement Learning Algorithms in 
Production Systems" submitted to the 19th Internation Conference on Computer Aided System Theory ([EUROCAST 2024](https://eurocast2024.fulp.ulpgc.es/)).

## Installation
To install the required packages, run `pip install -r requirements.txt`.

### Limitations
To substitute the keywords for Springer publications, the Springer API is used.
Make sure to set the API key in the notebook to be able to access the Springer API.


## Data

The data was collected from the following platforms:
 - [IEEE Xplore](https://ieeexplore.ieee.org/)
 - [Science Direct](https://www.sciencedirect.com/)
 - [ACM Digital Library](https://dl.acm.org/)
 - [Springer Link](https://link.springer.com/)

### Search Query

The used search query is inspired by [Panzer and Bender](http://dx.doi.org/10.1080/00207543.2021.1973138) and consists of an algorithmic keyword and general keywords.

 - Algorithmic Keyword: Reinforcement Learning
 - General Keywords: Assembly OR Automation OR Industry OR Industrie OR Manufacturing OR Production

Additionally, the keyword "Industrie" is added to the general keywords used by [Panzer and Bender](http://dx.doi.org/10.1080/00207543.2021.1973138) of the search query to detect all papers in the domain of Industrie 4.0.

The search query was structured such that the algorithmic keywords must be present in the title of the paper, while the general keywords must be present in its metadata.
### Results

The data was downloaded and placed into folder [data](./data) on the 22nd of October 2023. The queries and the amount of papers is shown in the following list:

 - [IEEE Xplore](https://ieeexplore.ieee.org/search/searchresult.jsp?action=search&newsearch=true&matchBoolean=true&queryText=(%22Document%20Title%22:Reinforcement%20Learning)%20AND%20(%22All%20Metadata%22:Assembly%20OR%20%22All%20Metadata%22:Automation%20OR%20%22All%20Metadata%22:Industry%20OR%20%22All%20Metadata%22:Manufacturing%20OR%20%22All%20Metadata%22:Production%20OR%20%22All%20Metadata%22:Industrie)%20NOT%20(%22Document%20Title%22:Survey%20OR%20%22Document%20Title%22:Review)&highlight=true&returnFacets=ALL&returnType=SEARCH&matchPubs=true&rowsPerPage=100&pageNumber=1): 3743 results
 - [ACM Digital Library](https://dl.acm.org/action/doSearch?fillQuickSearch=false&target=advanced&expand=dl&field1=Title&text1=%22reinforcement+learning%22&field2=AllField&text2=Assembly+OR+Automation+OR+Industry+OR+Industrie+OR+Manufacturing+OR+Production&field3=Title&text3=NOT+%28Survey+OR+Review%29): 1279 results
 - [Science Direct](https://www.sciencedirect.com/search?title=%22Reinforcement%20Learning%22&qs=Assembly%20OR%20Automation%20OR%20Industry%20OR%20Industrie%20OR%20Manufacturing%20OR%20Production): 2015 results
 - [Springer Link](https://link.springer.com/search?dc.title=%22Reinforcement+learning%22&query=%28Assembly+OR+Automation+OR+Industrie+OR+Industry+OR+Manufacturing+OR+Production%29&facet-start-year=2023&showAll=true&facet-end-year=2020): 2254 results


## Evaluation

The evaluation can be found by running the notebook [evaluation.ipynb](evaluation.ipynb).
