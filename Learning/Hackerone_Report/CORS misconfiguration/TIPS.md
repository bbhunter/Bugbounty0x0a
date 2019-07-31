***1*** - Use CURL command to verify that your target is vulunerable to CORS :) fast .

***2*** - Always look at the ``Oringin:`` in the request headers try to change it to value from your choice if it's reflected into the response then the application you're testing is vulunerable to CORS . 

***3*** - Since The ``Origin`` header does not reflect your input try some bypasses like ``https://www.target.attacker.com/`` or ``https://www.targetattacker.com`` and so on , it may works for you to hunt these types of issue .


