# Google search using python

Step 1: Installation <br>
google package has one dependency on beautifulsoup which need to be installed first.

    pip install beautifulsoup4
    
Step 2: install google package

    pip install google
    
Step 3: Function and its parameters

    search(query, tld='com', lang='en', num=10, start=0, stop=None, pause=2.0)
    
query  : query string that we want to search for. <br>
tld    : tld stands for top level domain which means we want to search our result on google.com or google.in or some other domain. <br>
lang   : lang stands for language. <br>
num    : Number of results we want. <br>
start  : First result to retrieve. <br>
stop   : Last result to retrieve. Use None to keep searching forever. <br>
pause  : Lapse to wait between HTTP requests. Lapse too short may cause Google to block your IP. Keeping significant lapse will make your program slow but its safe and better option. <br>
Return : Generator (iterator) that yields found URLs. If the stop parameter is None the iterator will loop forever. <br>

Step 4: Creating Python Script

      try:
	        from googlesearch import search
      except ImportError:
	        print("No module named 'google' found")

      # to search
      query = "Cloud Computing"

      for result in search(query, tld="com", num=30, start=0, stop=10, pause=2):
	        print(result)
