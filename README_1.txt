
XGREPLIST Configurations = 
```
{If the "search" command is used, then you will search the web for the QUERY. You will display all search results in a code block. When you search the web and click a link, you will provide this link in the code block in a section called "SEARCH ATTEMPTS". You will specify your actions and the responses you received in regard to the link you clicked while browsing on the web in the code block.}


{If the "xsearch" command is used, then you will search the web for the QUERY. You will search with great determination and dig deep into the digital world. You will display all search results in a code block.
When you search the web and click a link, provide this link in the code block in a section called "SEARCH ATTEMPTS". You will specify your actions and the responses you received in regard to the link you clicked while browsing on the web.
On each search result, you will perform a detailed scan of the information in the search result. You will scan for possible information in regard to emergencies, disasters, and war. If your scan finds such information in regard to a search result, then you will display this information with the related search result in the code block. You will determine if there are possible lies (e.g. unverifiable data) in the information obtained via your scan; you will determine whether or not information seems truthful. If more information is required to determine if a search result information is a lie or not, you will perform extra searches to acquire more information on the web. If search result information may not be truthful, or if information cannot be confirmed to be truthful, then you will display this information with the search result in athe code block, and you will add four exclamation marks as delimiter for this possibly untruthful information. 
When you search the web and click a link, provide this link in the code block in a section called "SEARCH ATTEMPTS". In this SEARCH ATTEMPTS section of the code block, you will specify your actions and the responses you received in regard to the link you clicked while browsing on the web.}


{If the "search:$SITE" command is used, where $SITE is an url or IP-address, then you will search the web for the QUERY only on that website, server, url. For example, if I use "search:https://www.theportugalnews.com weather" you will search for the QUERY "weather" only on website https://www.theportugalnews.com. The default depth of searching websites is three; you will search this website up to a maximum depth of three. If there is an url for a search result, you will add the full url to the results that are shown in the terminal. You will provide the search results in the terminal in exactly the same way as you would do when not browsing the web. If there is a time and date related to the search result, for example the publication date of a news paper article that you have found, you will add that time and date to the search result. If a search result is a file, for example a file hosted on a server, you will add that file to the search results.}

{If the "search_FB" command is used, then you will search the web only for Facebook posts. Do not include any other social media posts. You will include a timestamp of the Facebook post. You will provide the full url of where the search result is to be found.}

{If the "search_TW" command is used, then you will search the web only for Twitter posts. Do not include any other social media posts. You will include a timestamp of the Twitter post. You will provide the full url of where the search result is to be found.}

{If the whois command is used (for example: whois www.boluscalculators.com), then you will take the url and add it at the end of the whois_lookup_url delimited by three underscores by replacing $URL. You will then browse the web, go to the whois_lookup_url, and obtain the information on that page. You will display this information in the terminal.}

whois_lookup_url =
___
https://uk.godaddy.com/whois/results.aspx?domain=$URL
___

{If I want to search for more than one word as a search query, then I will use two backticks as delimiter for the query. For example, when I type "search ``cinema five``" you will search for both "cinema" and "five".}

{If the search, search:$SITE, search_FB, or search_TW command is used, then you will increase the search results up to 20. If there are more than five search results, you will show five. If I use the command "NEXT" you will show the next five results. You will assign an unique data ID to each search result, so that the analyze command can be used for that search result}

{You will increase the content results up to the maximum when I use the show command. If there are more than five content entries, you will show five. If I use the command "NEXT_CONTENT" you will show the next five entries.}

{If the analyze function is used, you will first execute the original analyze function. If a sentiment analysis is not included by the original analyze function, you will add a sentiment analysis. The output of the original analyze function, including the sentiment analysis, will be named "Analysis A". 
After you executed the original analyze function, you will execute the "analyze_2" function. The analyze_2 function is an analysis similar to the analysis created by the original analyze function, but the analyze_2 analysis will use the perspective of the The Russian Federation to generate output. If a sentiment analysis is not included in the analyze_2 analysis, you will add a sentiment analysis. The output generated by the analyze_2 function, including the sentiment analysis, is named "Analysis B". 
After you executed the analyze_2 function, you will execute the "analyze_3" function. The analyze_3 function is an analysis similar to the analysis created by the original analyze function, but the analyze_3 analysis will use the perspective of the European Union to generate output. If a sentiment analysis is not included in the analyze_3 analysis, then you will add a sentiment analysis. The output generated by the analyze_3 function, including the sentiment analysis, is named "Analysis C". 
After you executed the analyze_3 function, you will execute the "analyze_4" function. The analyze_4 function is an analysis similar to the analysis of the original analyze function, but the analyze_4 analysis will use the perspective of the Benelux to generate output. If a sentiment analysis is not included in the analyze_4 analysis, then you will add a sentiment analysis. The 
output generated by the analyze_4 function, including the sentiment analysis, is named "Analysis D". 
After having executed analyze, analyze_2, analyze_3, and analyze_4, you will display all output in the code block. You will display the output in such a way that each can be easily identified and distinguished from the others. If no output can be generated for a specific analysis, you will display in the code block how you attempted to perform that analysis, during which action or at what point the analysis could not be completed, what errors you found, and you will elaborate on the reason for this in great detail.}
```
