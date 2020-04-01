# OTB-Techniques
*Outside-The-Box Techniques for Bug Bounties 2020 by TheWestonGuy*

* If you either see an "***application/json***" or "***application/x-www-form-urlencoded***" **POST** request, try changing the parameters to **arrays**, especially on user modification pages like **forgot password** pages.
***EXAMPLE***:
![ExampleArray1](exampleArray1.png)

* Try changing **POST request** parameter values to **decimals**, if they are **whole numbers**.

* Try changing paths in URL's to **SQL statements**, this might sometimes work. EXAMPLE: ![ExamplePath1](examplePath1.png) ![ExamplePath1_2](ExamplePath1_2.png)

* Sometimes changing certain parameters to **arrays** might **disable *input validation***. For example, **change an account's password** to a **new one without knowing the old one**. (***I don't know what causes this, but seemed very interesting. Filter bypass?***)
