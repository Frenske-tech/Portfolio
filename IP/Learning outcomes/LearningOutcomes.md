# Portfolio s3

# Inhoud

[Learning outcomes 3](#_Toc105073453)

[1.You design and build user-friendly, full-stack web applications. 3](#_Toc105073454)

[Auth0 3](#_Toc105073455)

[2. You use software tooling and methodology that continuously monitors and improve the software quality during software development. 5](#_Toc105073456)

[4. You design and implement a (semi)automated software release process that matches the needs of the project context. 8](#_Toc105073457)

[8. You act in a professional manner during software development and learning. 9](#_Toc105073458)

# Learning outcomes

1.
## You design and build user-friendly, full-stack web applications.

For my individual project I chose to work with react and java spring boot, the main reason I chose to work with react in this project is because it has backing from facebook and a rather large community, I think it will be relevant longer then other frontend frameworks like vue. I chose to use java spring boot to learn a new language and it was recommended to me by my teacher.

Adding a review and scoring it

Gamename needs to be added by users themselves currently has no connection to a premade game I was planning on doing it but there were more urgent things I needed to do

![lo1](https://user-images.githubusercontent.com/71487939/173833211-7a6b7579-f937-438a-b978-f0f4afa6c7b6.png)

![lo2](https://user-images.githubusercontent.com/71487939/173833208-fab7c6dd-7975-4ba7-bc8f-c9101915950f.png)

A fairly straightforward list of the different reviews this could&#39;ve used more work and some user testing but I did both those things for the group project in de form of ux testing and a usability test. Which I will link to

## Auth0

I used Auth0 in order to let the user login to the application without needing to register.

![lo3](https://user-images.githubusercontent.com/71487939/173833204-89830252-50f8-4c8c-940c-35d32f7bd8f2.png)

![lo4](https://user-images.githubusercontent.com/71487939/173833203-25c1ccae-e5f3-4965-b3ad-7b6bf034b8c6.png)

The picture isn&#39;t showing but that is on my account, on another account is does work

There is also the option to log out.

To work with auth0 I used a tutorial [https://auth0.com/blog/spring-boot-authorization-tutorial-secure-an-api-java/](https://auth0.com/blog/spring-boot-authorization-tutorial-secure-an-api-java/), which already contained a frontend so I used that

![lo5](https://user-images.githubusercontent.com/71487939/173833200-be87b892-c8d7-4d45-a094-405b3aed770a.png)

When you&#39;re logged in with correct roles u can add edit and delete items.

![lo6](https://user-images.githubusercontent.com/71487939/173833199-6d3e8b3c-8f21-4ad4-bb60-4f9cf3b9269c.png)

![lo7](https://user-images.githubusercontent.com/71487939/173833191-88280588-2905-42a1-802e-f3db926a5125.png)

![lo8](https://user-images.githubusercontent.com/71487939/173833262-bd55bf7c-761c-410f-9a7a-0e65f379909d.png)

This checks whether the user actually has the authority in the frontend this is also filtered when you&#39;re not logged in or without the permission buttons wont show up

1.
## You use software tooling and methodology that continuously monitors and improve the software quality during software development.

### Unit testing

![lo9](https://user-images.githubusercontent.com/71487939/173833257-6208d75e-33e4-43d6-8dba-fe968261374d.png)

I added a few unit tests in order to test the functionality of my application I struggled a lot with running all the test for example in de delreview I used to deletebyid but for some reason that wouldn&#39;t work so I tested It like this.

### Integration testing

![lo10](https://user-images.githubusercontent.com/71487939/173833256-ce36c85a-0ef5-45b5-a331-1f907df605ac.png)

I&#39;ve got one measly integration test checking the controller. I have ran some other tests for example testing to post it 
![lo11](https://user-images.githubusercontent.com/71487939/173833254-95f7d860-0655-47be-ae72-262cfca02fa0.png)

But for some weird reason it cant resolve the content object while friend with exactly the same dependencies etc don&#39;t have any problem

![lo12](https://user-images.githubusercontent.com/71487939/173833252-ec7f8f43-5066-41e3-acbc-8ae6c527890c.png)

I also added sonar cloud in order to check bugs and vulnerabilities within my code as you can see there is most Definitely still work to do

![lo13](https://user-images.githubusercontent.com/71487939/173833249-db3ff36a-1e4f-40b3-afca-6d02badd907a.png)

You can also see the review the bugs and see why it is an issue although in my case its about the tests im running so it isn&#39;t high priority

# 4. You design and implement a (semi)automated software release process that matches the needs of the project context.

With github actions before a push or pull request on master I will run tests and when the tests check out it will push an image to docker hub

![lo14](https://user-images.githubusercontent.com/71487939/173833246-6aa48763-1814-4440-b63d-de74213e0a9e.png)

![lo15](https://user-images.githubusercontent.com/71487939/173833242-6faafd89-357e-403c-8f01-b88445dd0dae.png)

![lo16](https://user-images.githubusercontent.com/71487939/173833239-15e78eb1-4d6c-49b2-a9f4-8a974c66f047.png)

This was the first version for the backend

And the dockerfile I used

![lo17](https://user-images.githubusercontent.com/71487939/173833236-0d582beb-9081-4fa9-888b-b7237aa42b5c.png)

![lo18](https://user-images.githubusercontent.com/71487939/173833235-b76ab627-6bf4-4576-b81c-76184642c71e.png)

Later I added in Sonarcloud as well to perform static code analysis and discover potential weak point in my code which I wrote about in the previous chapter

![lo19](https://user-images.githubusercontent.com/71487939/173833229-fe63c739-0019-4235-87d0-05b269540360.png)

All tasks completed and a new image was pushed to docker

I also did this for the frontend in order to be able to run it together this also pushes an image to another docker repository

![lo20](https://user-images.githubusercontent.com/71487939/173833227-9c580234-6e78-4bf9-99b5-5831c0777f05.png)

And the dockerfile

![lo21](https://user-images.githubusercontent.com/71487939/173833225-fa52691a-cbdf-437e-809b-0259ce64d75e.png)

![lo22](https://user-images.githubusercontent.com/71487939/173833222-47cb0900-103a-41e6-ae83-c2bd5e497fa4.png)

All tasks completed and an image is pushed.

![lo23](https://user-images.githubusercontent.com/71487939/173833220-cca2bb51-a843-4336-bb57-5c8e2d12dc65.png)

Both running on different ports I did have some issues getting them to run together but after I added the -p tag in the console it worked

## 8. You act in a professional manner during software development and learning.

I uploaded every research I made unto github in the portfolio and in its own public repository so everyone can find and use it.

Project board here I have user stories im working on and under every user story there&#39;s different tasks I need to finish to split up the user story even more. I started the semester really not using my jira board but gradually towards the end of the year is started using it more and more helping me keep track of my progress and my todos

![lo24](https://user-images.githubusercontent.com/71487939/173833217-e44085de-2819-45da-ab18-f60a9e6ef19b.png)

I have a lot of problems keeping my concentration when I&#39;m working I was recommended a certain method by my teacher called pomodoro. Pomodoro breaks up your workday in 25 minutes of work and then a 5 minute break, this helped me keep my concentration and the 5 minute break helped me get a fresh look at things the website I used

-https://pomofocus.io/

![lo25](https://user-images.githubusercontent.com/71487939/173833214-a7b24cde-572f-4950-a510-db173ee3070e.png)

![lo26](https://user-images.githubusercontent.com/71487939/173833212-244c7175-7d79-4f50-8212-62b6da3d6d75.png)

I also wrote a few researches where I used the dot framework and apa style for references
The first about logging in with identity providers such as auth0 etc

[IdentityProvider](https://github.com/Frenske-tech/Portfolio/blob/main/IP/Research/ResearchReportLogin.md)

the second about User stories 

[User story](https://github.com/Frenske-tech/Portfolio/blob/main/IP/Research/UserStoryResearch.md)
