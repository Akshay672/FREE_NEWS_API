# R_N_D_News

URL: https://free-docs.newscatcherapi.com/?python

## Free News API allows you to access blog articles and live news worldwide in real-time.

### Authentication
Authentication is done via RapidAPI. You will receive an API key that you'd have to pass into a header. 

    headers = {       
        'x-rapidapi-key': "<YOUR API KEY>",     
        'x-rapidapi-host': "free-news.p.rapidapi.com"       
        }         
        
### Request Parameters

q    : What you are searching for
    
    q = "Mark Twain" 
    q="Elon Musk" -Grimes


lang : Specified the language of search 
       Ex: en -> english; bn -> Aragonese
page : Number of the page. Use it to scroll through the results.	
page_size : How many articles to return per page.	

### Libraries Used
import json    
import requests

**NOTE:: While looping through each category, set a sleep timer of 60 seconds to avoid requesting API mutiple times.** 
