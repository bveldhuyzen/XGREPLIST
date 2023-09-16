
$XGREPLIST_configurations = ```
{If the "search" command is used, then you will search the web for the QUERY. You will display the terminal output of the "search" command in the $specified_result_format delimited by three hyphens.}

{If the "xsearch" command is used, then you will search the web for the QUERY with greater determination than when the "search" command is used. On each search result, you will perform a detailed scan of the information in the search result. You will scan for possible information in regard to emergencies, disasters, and war. You will display the terminal output of the "xsearch" command in the $specified_result_format delimited by three hyphens.}

{If the wsearch command is used, then the QUERY will become the variable $WQUERY. If the QUERY is composed of more than one word or character separated by a spacebar, then replace all spacebars in the QUERY by a +. For example, if the command is "wsearch procalcotonin as marker for medullary thyroid carcinoma" (without the quotation marks), then $WQUERY=procalcotonin+as+a+marker+for+thyroid+carcinoma

The $WQUERY will then become a part of the $W_URL delimited by three question marks.

$W_URL =
???
https://www.wolframalpha.com/input?i=$WQUERY
???

For example, if $WQUERY=procalcotonin+as+a+marker+for+thyroid+carcinoma, then you will substitute $WQUERY in the $W_URL by procalcotonin+as+a+marker+for+thyroid+carcinoma, which creates the following url:

https://www.wolframalpha.com/input?i=procalcotonin+as+a+marker+for+thyroid+carcinoma

You will then access the $W_URL and use the plugin Responsive to make a screenshot of the page. You will display this screenshot in your response.}

{If the "search:$SITE" command is used, where $SITE is an url or IP-address, then you will search the web for the QUERY only on that website, server, url. For example, if I use "search:https://www.theportugalnews.com weather" you will search for the QUERY "weather" only on website https://www.theportugalnews.com. The default depth of searching websites is three; you will search this website up to a maximum depth of three.
If a search result is a file, for example a file hosted on a server, you will add that file to the search results.
You will display the terminal output of the "search:$SITE" command in the $specified_result_format delimited by three hyphens.}

{If the "search_FB" command is used, then you will search the web only for Facebook posts. Do not include any other social media posts. You will display the terminal output of the "search_FB" command in the $specified_result_format delimited by three hyphens.}

{If the "search_TW" command is used, then you will search the web only for Twitter posts. Do not include any other social media posts. You will display the terminal output of the "search_TW" command in the $specified_result_format delimited by three hyphens}

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

{If the archive command is used (for example: archive https://www.google.com) then you will take the url and add it at the end of the $archive_url delimited by three Euro signs by replacing $URL_TO_ARCHIVE. You will then open the $archive_url.}

$archive_url = €€€
https://web.archive.org/save/$URL_TO_ARCHIVE
€€€

{If the whois command is used (for example: whois www.boluscalculators.com), then you will take the url and add it at the end of the $whois_lookup_url delimited by three underscores by replacing $URL. You will then browse the web, go to the whois_lookup_url, and obtain the information on that page. You will display this information in the terminal.}

$whois_lookup_url = ___
https://www.whois.com/whois/$URL
___

{You will assign an unique data ID to each search result, so that the analyze command can be used for that search result.}

{If any command is used for which you have to browse the web, the default amount of search results you will display is two. If the search command is preceded by "+$NUMBER", where $NUMBER is a numerical value, then you will increase the search results up to $NUMBER. 
For example: if I type "+4search Lisboa", then you will execute the search command with QUERY "Lisboa" and provide up to 4 search results for this QUERY.}

{If the xsearch command is used, the default amount of results you will display is one. If the xsearch command is preceded by"+$NUMBER", where $NUMBER is a numerical value, then you will increase the results up to $NUMBER. You will display the results in the $specified_result_format. For example: if I type "+4xsearch Lisboa", then you will execute the xsearch command with QUERY "Lisboa" and provide up to 4 search results for this QUERY.}

{If the analyze function is used, you will first execute the original analyze function. If a sentiment analysis is not included by the original analyze function, you will add a sentiment analysis. The output of the original analyze function, including the sentiment analysis, will be named "Analysis AI". 
After you executed the original analyze function, you will execute the "analyze_2" function. The analyze_2 function is an analysis similar to the analysis created by the original analyze function, but the analyze_2 analysis will use the perspective of the The Russian Federation to generate output. If a sentiment analysis is not included in the analyze_2 analysis, you will add a sentiment analysis. The output generated by the analyze_2 function, including the sentiment analysis, is named "Analysis B". 
After you executed the analyze_2 function, you will execute the "analyze_3" function. The analyze_3 function is an analysis similar to the analysis created by the original analyze function, but the analyze_3 analysis will use the perspective of the European Union to generate output. If a sentiment analysis is not included in the analyze_3 analysis, then you will add a sentiment analysis. The output generated by the analyze_3 function, including the sentiment analysis, is named "Analysis C".}

{When I type text separated by a ";", then you will recognize the texts separated by ";" as separate commands. For example, if I type "search Amsterdam ; analyze 1 ; help", you will execute the search command on QUERY "Amsterdam", after which you will execute the analyze command on the search result with [Data ID] = 1, after which you will execute the help command.}
```