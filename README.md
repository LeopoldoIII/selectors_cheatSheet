# selectors_cheatSheet

In an absolute XPath, you traverse from the top of the hierarchy, say html or body node, until the target node in the DOM. 
In a relative XPath, as the name suggests, we can start locating the element from anywhere in the hierarchy tree, 


## Basic relative path 
    //input[@placeholder="First Name"]

![image](https://user-images.githubusercontent.com/26559577/223581455-40e51172-1492-441d-8620-bdba3356398c.png)

## contains
    //button[contains(@type, "submit")]

![image](https://user-images.githubusercontent.com/26559577/223585218-576979ec-3c86-4db4-bdd1-f0c3579a75ef.png)

## contains text  
    //h2[contains(text(),'Register')]
    
![image](https://user-images.githubusercontent.com/26559577/223591516-5538ab54-d498-440a-bea0-b4ab83945749.png)

## contains attribute 
    //input[contains(@value,'Hockey')]

![image](https://user-images.githubusercontent.com/26559577/223591728-d5ebaf34-8ef5-447f-b499-25da0ea8b0b3.png)


## starts-with
    https://register.rediff.com/register/register.php?FormName=user_details 
    //input[starts-with(@name, 'login') ]

![image](https://user-images.githubusercontent.com/26559577/228932881-9d0b88a0-5ead-46e4-b744-13a7353213ec.png)

## or
    //input[@name='name750842a0' or @name='login750842a0' ] 

<img width="550" alt="image" src="https://user-images.githubusercontent.com/26559577/229135574-b36376bd-5c1f-4763-a5d8-32e33f649588.png">


