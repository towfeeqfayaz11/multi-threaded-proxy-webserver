# multi threaded proxy webserver with LRU cache



             -----google.com----->     proxy server  ------------->   server
             <------return--------          |        <-------------  
               (if answer is                |
                present, return             |
                from cache)                 |
                                            |
                                           \|/
                                        lru cache
