1 - Using a proxy always look at Response Status code (3XX) and investigate it Request.

2 - Keep your eye always on parametres like `redirect=` or `red=` and so on.

3 - Try to test an open redirection on your path for example `https://www.example.com//%2Fhttps://www.redirectsite.com/`.

4 - Always look at `=/` or `=/directorie/` or `=/file.extention` this may indicate that the application you are testing may be redirected you to the root path or to a directorie or to a file.

5 - parametre brute forcing is a good way to discover this type of issue. ***Focus on login functionality***.

6 - use an archive.org to discover redirect parametres that are hidden on the live application. :) Give a try

7 - Don't give up.
