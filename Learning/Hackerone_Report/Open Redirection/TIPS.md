***1*** - Using a proxy always , look at Response Status code (3XX) and investigate it Request.

***2*** - Keep your eye always on parametres like `redirect=` or `red=` and so on.

***3*** - Try to test an open redirection on your path for example `https://www.example.com//%2Fhttps://www.redirectsite.com/`.

***4*** - Always look at `=/` or `=/directorie/` or `=/file.extention` this may indicate that the application you are testing may be redirected you to the root path or to a directorie or to a file.

***5*** - Parametre brute forcing is a good way to discover this type of issue. ***Focus on login functionality***.

***6*** - Use an archive.org to discover redirect parametres that are hidden on the live application. :) Give a try

***7*** - Always read Hackerone reports and try to test like the previous hacker did , may the issue still working.

***8*** - Search for bypasses

***9*** - Google is the best to help you find these type of issue try `site:example.com inurl="redirect="`.

***10*** - Sometimes you must encode your payload to work.

***11*** - Open redirection issue may exist into HTTP POST Request , Try it !.

***12*** - If the application implement an open redirection protection on `?next=https://something` try `Http` or `HTTP` or `httP`, it may be bypassed. 

***13*** - If the application implement an open redirection protection on `?next=https://www.ewample.com/` then try an ip adress `?next=127.0.0.1` or `?next=127.1` or `?next=Http:362773246` , it may work to bypass protection.

***14*** - Always keep your eye on the web server it's configuration may be vulunerable to open redirection.

***15*** - If you are faced with a long url that is encoded send it to Decoder into burp suite and decode it to see if there is a parametre that is used to redirection because it's difficult to observe it when it's encoded.

***16*** - Try to encode your payload multiple time to see if you can bypass the open redirection.

***17*** - Some application use a hashing schema to the redirected path try to crack all hashes, if yes try to hash your own payload, send it and see if there is an open redirection.

***18*** - Always request `index.php` file this may redirect you to `http://www.example.com` so try `http://www.example.com/index.php/google.com` or `http://www.example.com/index.php/index.php//google.com` or `http://www.example.com/index.php/index.php.google.com` and so on , try all .

***19*** - Try to add more slashes into your payload this may bypass open redirection protection .

***∞*** - Don't give up.
