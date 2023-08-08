# XGREPLIST
XGREPLIST is a non-invasive non-surveiling XKEYSCORE simulator that runs in chatGPT (and probably others) by prompting the AI to alter behaviour and become a search and analytical tool in the form of a terminal. 

When the AI catches up, XGREPLIST will dig into the digital world with great determination. Additional modules to further increase search, analysis, and reporting are in testing phase. Stats/algorithm/visualization options to be included after initial testing. Free to use and edit by all.

Current status:  
![Model](https://raw.githubusercontent.com/bveldhuyzen/XGREPLIST/main/Screenshot_2023-08-08-05-20-11-565_com.chrome.beta.jpg)  
  
  
# Functions:

#Search tools (testing/online):  

- search: normal web search  
> [b]use[/b]: type `search QUERY` to search for QUERY  
> example: `search Amsterdam events August 2022`  
> requires: at least one web browsing plugin enabled

- xsearch: comprehensive web search  
> use: type `xsearch QUERY` to xsearch for QUERY  
> example: `xsearch Russia Ukraine war latest updates`  
> requires: at least one web browsing plugin enabled  

- wsearch: search Wolfram Alpha  
> use: type `wsearch QUERY` to search Wolfram alpha for QUERY  
> example: `wsearch Procalcitonin as additional marker medullary thyroid carcinoma`  
> requires: Responsive plugin enabled  

- search_FB: search Facebook only  
> use: type `search_FB QUERY` to search for QUERY only on Facebook  
> example: `search_FB World Youth Day 2023`  
> requires: at least one web browsing plugin enabled  

- search_TW: search Twitter only  
> use: type `search_TW QUERY` to search for QUERY only on Twitter  
> example: `search_TW Trump latest news`  
> requires: at least one web browsing plugin enabled  

#Web tools (testing/online):  

- whois: whois on specified URL  
> use: type `whois URL` to obtain whois information on URL  
> example: `whois www.openai.com`  
> requires: at least one web browsing plugin enabled  

- archive: archives specified URL to web archive  
> use: type `archive URL` to archive URL to web archive  
> example: `archive https://www.google.com`  
> requires: at least one web browsing plugin enabled  

#Analysis tools:  

- analyze: performs specified analysis on specified [Data ID]  
> use: type `analyze DATA_ID` to perform analysis on DATA_ID  
> example: `analyze 4`    
> requires: [Data ID] of search result(s)  
> NOTE: This analyze function is just a test to test some analysis capabilities, e.g. sentiment analysis; later analyze functions will be more specific  

- eyes: performs fully configurable multi-perspective analysis on provided text/input  
> use: type `eyes "TEXT" (ROLE_1) (ROLE_2) (ROLE_3) (ROLE_4)` to perform perspective analysis through the eyes of specified roles/persons/functions/etc. on TEXT.  
Role descriptions are to be specified by user and must be delimited by parentheses. Role description is to be minimum 1 character and maximum 4000 words.  
> example: `eyes "due to the war in Ukraine, all consumable prices are up, but oddly enough the beer price has remained the same all the time" (professor in economics specialized in super markets) (head of Dutch food and consumable regulatory authority) (random medium-wage earning individual in France; likes beer a lot) (CEO of the largest beer brewer in Europe)`  
requires: at least one web browsing plugin enabled to load eyes module (if not loaded yet; if eyes module is loaded then no plugin's required)

#Pending / in testing phase

- Scientific/medical calculator integration
- Execute formula
- Execute bash code/script on input text/code/url/file (testing; possibly limited functionality))
- Statistical analysis
- Output visualization 
- Search result validation (lie detector)
- Data upload / outbound messenger (testing/offline)
- MDR compliance scanner
...
  
  
For prototype use/testing, enable web browsing on the AI, and copy-paste the prompt from XGREPLIST_prototype.
  
  
glhf

