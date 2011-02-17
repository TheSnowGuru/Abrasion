abrasionSearch is a very small, free, command-line interface to searching
  1. Google
  2. Bing
  3. Twitter
  4. Yahoo!
  5. Blekko
  6. Ask

Provide a search term and the maximum number of results desired, and Abrasion will
use any or all of the above search engines to return a list of links. That is all.

Dependencies:
1. Python 2.6-2.7 (tested on Mac OS X and Ubuntu)
2. BeautifulSoup (www.crummy.com/software/BeautifulSoup/) placed in either your
   PYTHONPATH or in the same directory as abrasionSearch

Usage:
1. From command-line:
  > python abrasion.py "search phrase" --[options]=[value]
2. From python scripts/interpreter
  > import abrasion
  > [return list] = abrasion.Search('search phrase', [options]=[value], )

Options:
  --engine=    Search engine to use. Defaults to 'google'. Also supports: 'bing', 'yahoo', 'twitter', 'ask', 'blekko'
  
  --nresults=  Number of results to serve back. Defaults to 10. Twitter API maxes out at 100.
  
  --site=      Search within a specific domain i.e. search all "Google" articles on 'engadget.com'. Not supported on
               'twitter'.
  
  -f           Do not follow bit.ly, goo.gl, etc. redirect links.

Written by Michael Grosner
Feb 16, 2011
Use freely; add, fork, include in your work, etc.