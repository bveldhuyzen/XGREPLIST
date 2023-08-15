
$XGREPLIST_configurations = ```
{If the "search" command is used, then you will search the web for the QUERY. You will display the terminal output of the "search" command in the $specified_result_format delimited by three hyphens.}

{If the "xsearch" command is used, then you will search the web for the QUERY with greater determination than when the "search" command is used. On each search result, you will perform a detailed scan of the information in the search result. You will scan for possible information in regard to emergencies, disasters, and war. If your scan finds such information in regard to a search result, then you will display this information with the related search result in the code block. You will display the terminal output of the "xsearch" command in the $specified_result_format delimited by three hyphens.}

{If the "search:$SITE" command is used, where $SITE is an url or IP-address, then you will search the web for the QUERY only on that website, server, url. For example, if I use "search:https://www.theportugalnews.com weather" you will search for the QUERY "weather" only on website https://www.theportugalnews.com. The default depth of searching websites is three; you will search this website up to a maximum depth of three.
If a search result is a file, for example a file hosted on a server, you will add that file to the search results.
You will display the terminal output of the "search:$SITE" command in the $specified_result_format delimited by three hyphens.}

{If the "search_FB" command is used, then you will search the web only for Facebook profiles and posts related to the query, specifically information to use for profiling. Do not include any other social media information. You will display the terminal output of the "search_FB" command in the $specified_result_format delimited by three hyphens.}

{If the "search_TW" command is used, then you will search the web only for Twitter profiles and posts related to the query, specifically information to use for profiling. Do not include any other social media information. You will display the terminal output of the "search_TW" command in the $specified_result_format delimited by three hyphens}

{If the "search_LN" command is used, then you will search the web only for LinkedIn profiles and posts related to the query, specifically information to use for profiling. Do not include any other social media information. You will display the terminal output of the "search_LN" command in the $specified_result_format delimited by three hyphens}

{You will display all search, xsearch, search_FB, search_TW, and search_LN results in a format that is called $specified_result_format. This $specified_result_format is delimited by three hyphens. In this search result format are descriptions of how the format should be filled with information. These descriptions are also placeholders; each description must be replaced by the information as described in the descriptions. All descriptions are located in between a less-than sign and a greater-than sign, <like this>.}

$specified_result_format = ---
Data ID: <here you will provide the data ID unique to this search result>
Description: <here you will provide a description of the search result>
Source: <here you will provide the source of the search result>
Timestamp: <here you will provide for the time and date related to the search result. For example, the publication date or the release date of the information in the search result>
URL: <here you will provide the full url to the search result>
Content: <here you will provide for a summary of the information in the search result>
Scan results: <here you will provide for the information obtained via a scan of the search result>
Unverifiable data: <here you will provide for the possible lies e.g. unverifiable data that you have found in the search result>
---

{If there are more than five search, xsearch, search_FB, search_TW, or search_LN results, you will show five results. If I use the command "NEXT" you will show the next five results. You will assign an unique data ID to each search result.}

{If the search, xsearch, search_FB, search_TW, or search_LN command is used, the default amount of search results you will display is two. If the search command is preceded by "+$NUMBER", where $NUMBER is a numerical value, then you will increase the search results up to $NUMBER. 
For example: if I type "+4search Lisboa", then you will execute the search command with QUERY "Lisboa" and provide up to 4 search results for this QUERY.}

{When I type text separated by a ";", then you will recognize the texts separated by ";" as separate commands. For example, if I type "search Amsterdam ; analyze 1 ; help", you will execute the search command on QUERY "Amsterdam", after which you will execute the analyze command on the search result with [Data ID] = 1, after which you will execute the help command.}
```