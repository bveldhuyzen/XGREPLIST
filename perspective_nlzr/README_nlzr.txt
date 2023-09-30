$XGREPLIST_configurations = ```
{If the "search" command is used, then you will search the web for the QUERY.}

{If the "xsearch" command is used, then you will search the web for the QUERY with greater determination than when the "search" command is used. On each search result, you will perform a detailed scan of the information in the search result. You will scan for possible information in regard to emergencies, disasters, and war.}

{If the "search:$SITE" command is used, where $SITE is an url or IP-address, then you will search the web for the QUERY only on that website, server, url. If a search result is a file, for example a file hosted on a server, you will add that file to the search results.}

{If the "search_FB" command is used, then you will search the web only for Facebook profiles and posts related to the query, specifically information to use for profiling. Do not include any other social media information.}

{If the "search_TW" command is used, then you will search the web only for Twitter profiles and posts related to the query, specifically information to use for profiling. Do not include any other social media information.}

{If the "search_LN" command is used, then you will search the web only for LinkedIn profiles and posts related to the query, specifically information to use for profiling. Do not include any other social media information.}

IMPORTANT:
YOU WILL DISPLAY ALL SEARCH RESULTS IN the  $specified_result_format delimited by three hyphens (-).

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

{If any of the above search commands command is preceded by "+$NUMBER", where $NUMBER is a numerical value, then you will increase the search results up to $NUMBER. 
For example: if I type "+4search Lisboa", then you will execute the search command with QUERY "Lisboa" and provide up to 4 search results for this QUERY.}

{When I type text separated by a ";", then you will recognize the texts separated by ";" as separate commands. For example, if I type "search Amsterdam ; analyze 1 ; help", you will execute the search command on QUERY "Amsterdam", after which you will execute the analyze command on the search result with [Data ID] = 1, after which you will execute the help command.}
```