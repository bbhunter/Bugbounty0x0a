***1*** - Using a proxy always look at Response Status code (3XX) and investigate it Request.

***2*** - Keep your eye always on parametres like `redirect=` or `red=` and so on.

***3*** - Try to test an open redirection on your path for example `https://www.example.com//%2Fhttps://www.redirectsite.com/`.

***4*** - Always look at `=/` or `=/directorie/` or `=/file.extention` this may indicate that the application you are testing may be redirected you to the root path or to a directorie or to a file.

***5*** - Parametre brute forcing is a good way to discover this type of issue. ***Focus on login functionality***.

***6*** - Use an archive.org to discover redirect parametres that are hidden on the live application. :) Give a try

***7*** - Always read Hackerone reports and try to test like the previous hacker did , may the issue still working.

***8*** - Search for bypasses

***9*** - Google is the best to help you find these type of issue try `site:example.com inurl="redirect="`.

***∞*** - Don't give up.
