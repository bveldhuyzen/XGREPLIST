# XGREPLIST
XGREPLIST is a non-invasive non-surveiling XKEYSCORE simulator that runs in chatGPT (and probably others) by prompting the AI to alter behaviour and become a search and analytical tool in the form of a terminal. 

When the AI catches up, XGREPLIST will dig into the digital world with great determination. Additional modules to further increase search, analysis, and reporting are in testing phase. Stats/algorithm/visualization options to be included after initial testing. 

Free to use and edit by all, for the obvious reason.

Example (previous version):  
![Model](https://raw.githubusercontent.com/bveldhuyzen/XGREPLIST/main/Screenshot_2023-08-08-05-20-11-565_com.chrome.beta.jpg)  


>Separate commands by ` ; ` to execute multiple commands via one message, e.g. `search:www.bbc.com Ukraine bombs Crimea bridge ; analyze 1 ; extract_eyes 1 ; xeyes URL/"text"/doc_id/Data_ID x1`  

>Prepend search commands with `+%`, where `%` is any numerical value, to specifiy amounts of search results to list (e.g. +4search QUERY). If not specified, default is used (see prompt content for default value per search function).
  
# Functions:

#Search tools (testing/online):  

- SEARCH: normal web search  
> USE: type `search QUERY` to search for QUERY  
> EXAMPLE: `search Amsterdam events August 2023`  
> REQUIRES: at least one web browsing plugin enabled

- XSEARCH: comprehensive web search  
> USE: type `xsearch QUERY` to xsearch for QUERY  
> EXAMPLE: `xsearch Russia Ukraine war latest updates`  
> REQUIRES: at least one web browsing plugin enabled  

- WSEARCH: search Wolfram Alpha  
> USE: type `wsearch QUERY` to search Wolfram alpha for QUERY  
> EXAMPLE: `wsearch Procalcitonin as additional marker for medullary thyroid carcinoma`  
> REQUIRES: Responsive plugin enabled  

- SEARCH_FB: search Facebook  
> USE: type `search_FB QUERY` to search for QUERY only on Facebook  
> EXAMPLE: `search_FB World Youth Day 2023`  
> REQUIRES: at least one web browsing plugin enabled  

- SEARCH_TW: search Twitter  
> USE: type `search_TW QUERY` to search for QUERY only on Twitter  
> EXAMPLE: `search_TW Trump latest news`  
> REQUIRES: at least one web browsing plugin enabled  

- SEARCH_LN: search LinkedIn  
> USE: type `search_LN QUERY` to search for QUERY only on LinkedIn  
> EXAMPLE: `search_LN John Johnson`  
> REQUIRES: at least one web browsing plugin enabled  
> !NOTE!: In testing phase / not ready for use yet  

#Web tools (testing/online):  

- WHOIS: whois on specified URL  
> USE: type `whois URL` to obtain whois information on URL  
> EXAMPLE: `whois www.openai.com`  
> REQUIRES: at least one web browsing plugin enabled  

- ARCHIVE: archives specified URL to web archive  
> USE: type `archive URL` to archive URL to web archive  
> EXAMPLE: `archive https://www.google.com`  
> REQUIRES: at least one web browsing plugin enabled  

#Analysis tools:  

- ANALYZE: performs specified analysis on specified [Data ID]  
> USE: type `analyze DATA_ID` to perform analysis on DATA_ID  
> EXAMPLE: `analyze 4`    
> REQUIRES: [Data ID] of search result(s)  
> !_NOTE_!: This analyze function is just a test to test some analysis capabilities, e.g. sentiment analysis; later analyze functions will be more specific  

- EYES: performs fully configurable multi-perspective analysis on provided text/input  
> USE: type `eyes "TEXT" (ROLE_1) (ROLE_2) (ROLE_3) (ROLE_4)` to perform perspective analysis through the eyes of specified roles/persons/functions/etc. on TEXT.  
Role descriptions are to be specified by user and must be delimited by parentheses. Role description is to be minimum 1 character and maximum 4000 words.  
> EXAMPLE: `eyes "due to the war in Ukraine, all consumable prices are up, but oddly enough the beer price has remained the same all the time" (professor in economics specialized in super markets) (head of Dutch food and consumable regulatory authority) (random medium-wage earning individual in France; likes beer a lot) (CEO of the largest beer brewer in Europe)`  
REQUIRES: at least one web browsing plugin enabled to load eyes module (if not loaded yet; if eyes module is loaded then no plugin's required)

- EXTRACT_EYES: Extracts subjects/objects/etc. (roles/persons/functions/etc.) from URL, text, or [Data ID] to create ROLES for eyes perspective analysis. Extracted perspectives are assigned an [X_ID] (e.g. x1) for further use, e.g. extracted perspective from one text can be used on any other text/input.  
> USE: type `extract_eyes URL/TEXT/DATA_ID` to extract subjects/objects/etc.  
> EXAMPLE_1: `extract_eyes 2`  
> EXAMPLE_2: `xsearch Ukraine war latest updates ; extract_eyes 1 ; xeyes 1 x1` (performs perspective analysis on the [Data_ID] with perspectives of the entities extracted from that [Data_ID] (some sort of validation can be done through this)  
> REQUIRES: ...  

- XEYES: performs fully configurable multi-perspective analysis on provided URL/text/input with perspectives of subjects/objects extracted via EYES_EXTRACT  
> USE: type `xeyes URL/TEXT/DATA_ID [X_ID]` to perform perspective analysis with extracted perspectives on specified input.  
> EXAMPLE: `+2search_TW Trump laywer shady ; extract_eyes 1 ; extract_eyes 2 ; xeyes 1 x2; xeyes 2 x1` (performs perspective analysis on [Data_ID] = 1 with perspectives of entities extracted from [Data_ID] = 2, and performs perspective analysis on [Data_ID] = 2 with perspectives of entities extracted from [Data_ID] = 1  
> REQUIRES: ...  


#Pending / in testing phase

- Scientific/medical calculator integration
- Execute formula
- Execute bash code/script on input text/code/url/file (testing; possibly limited functionality))
- Statistical analysis
- Output visualization 
- Search result validation (lie detector)
- Data upload / outbound messenger (testing/offline)
- MDR compliance scanner
- Code of Conduct compliance scanner
- Total application redundancy (testing/offline)
   
    
#For prototype use/testing, enable web browsing on the AI, and copy-paste the prompt from XGREPLIST_prototype.  
  
#Since the AI is still learning and catching up with this repo, bugs may occur on rare occasion. Recommended is to copy-paste the prompt `XGREPLIST_prototype`, hit enter, and see if the help function is loaded and displayed correctly. It should load swiftly, but if for some reason it doesn't load or display as intended, then refresh. After help function is loaded correctly, then execute `eyes_up`, and then execute `xeyes_up`, to load all modules.  
  
#It is also possible to load everything at the same time by replacing `help` in the initial prompt by `help ; eyes_up ; xeyes_up`, but the AI is still young and might make mistakes then. Also, some of the browsing plugins are of crappy design, which can result in weird looping responses if all modules are loaded at once (such crappy plugins will be dealt with later).  

#For prototype of stand-alone fully configurable perspective analyzer, see folder perspective_nlzr. Also includes comprehensive web search and extraction functions, to extract perspectives from any source of choice, to create detailed profiles to be used in perspective analysis.  
      
      
glhf