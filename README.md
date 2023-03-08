# selectors_cheatSheet

In an absolute XPath, you traverse from the top of the hierarchy, say html or body node, until the target node in the DOM. 
In a relative XPath, as the name suggests, we can start locating the element from anywhere in the hierarchy tree, 


    //input[@placeholder="First Name"]

![image](https://user-images.githubusercontent.com/26559577/223581455-40e51172-1492-441d-8620-bdba3356398c.png)


    //button[contains(@type, "submit")]

![image](https://user-images.githubusercontent.com/26559577/223585218-576979ec-3c86-4db4-bdd1-f0c3579a75ef.png)


    //h2[contains(text(),'Register')]
    
![image](https://user-images.githubusercontent.com/26559577/223591516-5538ab54-d498-440a-bea0-b4ab83945749.png)


    //input[contains(@value,'Hockey')]

![image](https://user-images.githubusercontent.com/26559577/223591728-d5ebaf34-8ef5-447f-b499-25da0ea8b0b3.png)
