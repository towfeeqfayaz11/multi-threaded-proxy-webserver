# multi threaded proxy webserver with LRU cache



             -----google.com----->     proxy server  ------------->   server
             <------return--------          |        <-------------  
               (if answer is                |
                present, return             |
                from cache)                 |
                                            |
                                           \|/
                                        lru cache



lsof -i tcp:8080
kill -9 <pid>

./proxy 8080
http://localhost:8080/https://www.cs.princeton.edu/
