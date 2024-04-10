# Webscraping_with_R_-Jupiter_Notebook

#Currently I am working on a project for my first ever R class and I am having some difficulty.  

 # Our target COVID-19 wiki page URL is: https://en.wikipedia.org/w/index.php?title=Template:COVID-19_testing_by_country  
  # Which has two parts: 
    # 1) base URL `https://en.wikipedia.org/w/index.php  
    # 2) URL parameter: `title=Template:COVID-19_testing_by_country`, seperated by question mark ?
    
  # Wiki page base
 
  # You will need to create a List which has an element called `title` to specify which page you want to get from Wiki
  # in our case, it will be `Template:COVID-19_testing_by_country`
 
  # - Use the `GET` function in httr library with a `url` argument and a `query` arugment to get a HTTP response
    
  # Use the `return` function to return the response
    
get_wiki_covid19_page <- function() {
     base_url <- "https://en.wikipedia.org/w/index.php"
     query_param <-list(title = 'Template:Covid-19_testing_by_country')
     response <-GET(base_url,query=query_param)
     return(response)
    }
    
 #This is what I have so far, I was wondering if anyone could help correct this and explain why that correction is needed.
    
        
