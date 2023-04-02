# selectors_cheatSheet

In an absolute XPath, you traverse from the top of the hierarchy, say html or body node, until the target node in the DOM. 
In a relative XPath, as the name suggests, we can start locating the element from anywhere in the hierarchy tree, 


## Basic relative path 
    //input[@placeholder="First Name"]

![image](https://user-images.githubusercontent.com/26559577/223581455-40e51172-1492-441d-8620-bdba3356398c.png)

## contains
    //button[contains(@type, "submit")]

![image](https://user-images.githubusercontent.com/26559577/223585218-576979ec-3c86-4db4-bdd1-f0c3579a75ef.png)

## text  
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

## and 
    //td[@colspan='5' and @class='f22']
    //td[@colspan='5'][@class='f22']

![image](https://user-images.githubusercontent.com/26559577/229263417-259fa85f-69c9-4a9d-a30e-b47d4369695f.png)

## Axes 
### - self

    //input[@type='radio']//self::input
    
<img width="550" alt="image" src="https://user-images.githubusercontent.com/26559577/229327525-5ba07933-9d86-4cac-a9b4-33dcb483b5fe.png">

### - parent 

    //input[@type='radio']//parent::label

<img width="437" alt="image" src="https://user-images.githubusercontent.com/26559577/229327770-6ca409a1-5549-48ca-990b-edc1a83d1406.png">

### - ancestor

    //input[@type='radio']//ancestor::div


<img width="639" alt="image" src="https://user-images.githubusercontent.com/26559577/229327893-bf5ff15f-91d4-4703-93b5-0249fd92797c.png">

### - child

    //select[@id='Skills']//child::option

<img width="640" alt="image" src="https://user-images.githubusercontent.com/26559577/229330825-44c68cee-485f-4210-a9b6-22ade04c9f6d.png">

### - following 

    //input[@type='checkbox']//following::div

<img width="639" alt="image" src="https://user-images.githubusercontent.com/26559577/229358085-8c55836f-1e78-4dc0-a23e-279c3c5b86b1.png">


### -- following-sibling

    //label[contains(text(), 'Date Of Birth')]//following-sibling::div

<img width="645" alt="image" src="https://user-images.githubusercontent.com/26559577/229366782-7470d311-81a4-4714-bdb4-e956f76cd205.png">

### - preceding

    //input[@type='checkbox']//preceding::div

<img width="650" alt="image" src="https://user-images.githubusercontent.com/26559577/229358319-1f04a4e8-c973-4e4a-a231-6bf9bab91795.png">

### - preceding-sibling

    //label[@class='checks']//preceding-sibling::input 

<img width="640" alt="image" src="https://user-images.githubusercontent.com/26559577/229361928-a9038eb3-7b41-4b03-911b-d995f3862416.png">
