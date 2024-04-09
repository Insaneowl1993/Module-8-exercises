[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-718a45dd9cf7e7f842a935f5ebbe5719a5e09af4491e668f4dbf3b35d5cca122.svg)](https://classroom.github.com/online_ide?assignment_repo_id=13541396&assignment_repo_type=AssignmentRepo)
<br/>
<br/>

[![alt text](https://x4w8f4y8.rocketcdn.me/wp-content/uploads/2020/05/iod_h_tp_white_c.png)](#)

<!-- _class: lead -->

![](./images/iod.png)

>### Module 8 | Exercises

# Databases

<br/>

This assignment includes an in-class directive.

In case you missed any of the instructions in the class, please refer to the recording:

[![Maintainer](https://custom-icon-badges.demolab.com/badge/-ZOOM%20CLASS%20RECORDING-gold?style=for-the-badge&logo=google-logo&logoColor=black)](https://docs.google.com/spreadsheets/d/1ToABwZF6np66kwIxg-qORVwkW-G__6FBbsPHdmH6rOA/edit#gid=0{:target="_blank})

<br/>
<br/>

<h1> Logical Diagram</h1>

<!-- checked, completion receipt for exercise 2, i fixed the diagram 1, please fix the diagram 2. -->


```mermaid
classDiagram

    User : username
    User : profile_picture
    
    User --|> Post 
    Post : Title
    Post : description
    Post : image

    User --|> Comments
    Comments : username
    Comments : count
    Comments : post_title

    User --|>  Likes 
    Likes : username
    Likes : username
    Likes : count
    
```

<br>
<br>
<h1>Physical Diagram</h1>


```mermaid

classDiagram

    User : User id (string)
    User : Profile Image(png)

    User --|> Post
    Post : Bio(string)
    Post : User Image(Image)
    Post : Post IMG(FK)

    
    User --|> Comments 
    Comments : User ID(string)
    Comments : Post ID(string)
    Comments : Count(var)


    User --|>  Likes 
    Likes : User ID(String)
    Likes : Post ID(String)
    Likes : Count(Var)

    Redis 
    Redis : comments (hash list)
    Redis : ####Date, date
    Redis : comment####Message, the Message 


```
<html>
  <div align='center'>
    <h4>Please don't forget to add "<b>COMPLETED</b>" into your commit description when your assignment is ready for checking.</h4>
  </div>
</html>

<br/>
<br/>
<br/>
