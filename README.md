   
get_wiki_covid19_page <- function() {
     base_url <- "https://en.wikipedia.org/w/index.php"
     query_param <-list(title = 'Template:Covid-19_testing_by_country')
     response <-GET(base_url,query=query_param)
     return(response)
    }
    
Response [https://en.wikipedia.org/w/index.php?title=Template%3ACovid-19_testing_by_country]
  Date: 2024-08-23 23:39
  Status: 404
  Content-Type: text/html; charset=UTF-8
  Size: 35.8 kB
<!DOCTYPE html>
<html class="client-nojs vector-feature-language-in-header-enabled vector-fea...
<head>
<meta charset="UTF-8">
<title>Template:Covid-19 testing by country - Wikipedia</title>
<script>(function(){var className="client-js vector-feature-language-in-heade...
"wgDigitTransformTable":["",""],"wgDefaultDateFormat":"dmy","wgMonthNames":["...
"wgMediaViewerOnClick":true,"wgMediaViewerEnabledByDefault":true,"wgPopupsFla...
"user.styles":"ready","ext.globalCssJs.user":"ready","user":"ready","user.opt...
<script>(RLQ=window.RLQ||[]).push(function(){mw.loader.impl(function(){return...
    
        
#The problem is that the colon is coming through as a hex code %3A instead of a colon.

#I am not sure how to get this to come through.
