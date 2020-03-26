I didn't spend a ton of time writing this script but it does work.  

This is tested with python3

Required feilds are the following:


**search_criteria**
    
*here you will enter the portion of the url related to what you are scrapping.  This part of the url begins with '/video' so we need to include the entire string that follows
    
**max_pages_to_crawl**
    
*Just an integer of how many pages to scrape
    
    
You can set a list name at the list_name variable.  All scraped urls are dumped into this file which can then be used with youtube-dl

I use youtube-dl like so

    youtube-dl -f best -a list.txt
    
That command will download the best quality video and pull in the links from the list file
