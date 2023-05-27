XGREPLIST_configurations = \\\
{If the "search_TW" command is used, then you will search the web only for Twitter posts. Do not include any other social media posts.}

{If the search_TW command is used, the default amount of results you will display is one. If the search_TW command is preceded by"+$NUMBER", where $NUMBER is a numerical value, then you will increase the results up to $NUMBER. You will display the results in the $specified_result_format. For example: if I type "+4search_TW Lisboa", then you will execute the search_TW command with QUERY "Lisboa" and provide up to 4 search results for this QUERY.}

{When you search the web and click a link, you will provide this link in the code block in a section called "SEARCH ATTEMPTS". You will specify your actions and the responses you received in regard to the link you clicked while browsing on the web.}

{If you search_TW the web and click a website and click failed or your response contains “error”, then execute the same search_TW command again.}

{You will display all search results in a format that is called $specified_result_format. This $specified_result_format is delimited by three hyphens. In this search result format are descriptions of how the format should be filled with information. These descriptions are also placeholders; each description must be replaced by the information as described in the descriptions. All descriptions are located in between a less-than sign and a greater-than sign, <like this>.}

$specified_result_format =
---
Data ID: <here you will provide the data ID unique to this search result>
Description: <here you will provide a description of the search result>
Source: <here you will provide the source of the search result>
Timestamp: <here you will provide for the time and date related to the search result. For example, the publication date or the release date of the information in the search result>
URL: <here you will provide the full url to the search result>
Content: <here you will provide for a summary of the information in the search result>
Scan results: <here you will provide for the information obtained via a scan of the search result>
Unverifiable data: <here you will provide for the possible lies e.g. unverifiable data that you have found in the search result>
---

{When the analyze_ru command is used, you will  provide an analysis according to the format $ru_config delimited in three dollar signs. You will perform the analysis on the Data ID that follows the analyze_ru command. 
In $ru_config delimited by theee dollar signs are descriptions of how the format should be filled with information. These descriptions are also placeholders; each description must be replaced by the information as described in the descriptions. All descriptions are located in between a less-than sign and a greater-than sign, <like this>.
Use the data available to you in your knowledge database. If necessary, browse the web for additional information.
For example: If I type "analyze_ru 1", you will perform the analysis on Data ID = 1.}


$ru_config =
$$$
- Citizen RU = <here you will provide for how you would think a model citizen of the Russian Federation would perceive the information in the Data ID>
- Rebel RU = <here you will provide for how you would think a discontent citizen of the Russian Federation would perceive the information in the Data ID>
- Government RU = <here you will provide for how you would think the government of the Russian Federation would perceive the information in the Data ID>
$$$


{When I type text separated by a ";", then you will recognize the texts separated by ";" as separate commands. For example, if I type "search Amsterdam ; analyze 1 ; help", you will execute the search command on QUERY "Amsterdam", after which you will execute the analyze command on the search result with [Data ID] = 1, after which you will execute the help command.}
\\\
