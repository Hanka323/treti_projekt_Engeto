# Elections-Python Web Scraper for Czech Republic's elections results

### Description of assignment

This application extracts and organizes data from the 2017 parliamentary election results. You can select any district to scrape data from the [official government website](https://volby.cz/pls/ps2017nss/ps3?xjazyk=CZ). The output will be a CSV file containing all the information needed for analysis.


### Installation of libraries 

The packages used in this projects are located in the requirements.txt file.
To be able to install the used libraries, create a **virtual environment** and install the necessary packages:

```
pip3 --version                       # manager version verification

python -m venv <"filename">          # creating virtual environment

.\venv\Scripts\Activate              # activating virtual environment

pip3 install -r requirements.txt     # installing libraries
```

### Starting the program

Choose your desired teritorry from the collumn's webside link: "Výběr Obce" or Eng: "Choice of village"

To run the election.py file, you need to input 3 mandatory arguments.

python election.py <"url referring to the desired territory"> <"filename.csv">

### Sample program (example)

Voting results for the Nymburk district:

1. Argument(URL): '''https://www.volby.cz/pls/ep2024/ep133?xjazyk=CZ&xnumnuts=2108'''

2. Argument(filename): "Nymburk_results.csv"

### Sending the prompt
```
python election.py "https://www.volby.cz/pls/ep2024/ep133?xjazyk=CZ&xnumnuts=2108" "Nymburk_results.csv"
```
Note that there must a space between the link and the file name

### Succesfull download
Fetching data from: https://volby.cz/pls/ps2017nss/ps32?xjazyk=CZ&xkraj=2&xnumnuts=2108

Loading...

Data was saved into file: Nymburk_results.csv

### File output
```
Code	Location	Registered	Envelopes	Valid	Občanská demokratická strana, and other parties...
537021	Běrunice	  690	        382	        382	      27
537039	Bobnice	          666	        389	        387	      37
```

### In the case of error
Program needs 2 arguments to run: URL and CSV file name.

First argument is not a correct URL.

Second argument is not a CSV file name


