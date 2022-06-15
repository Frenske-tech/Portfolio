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

![](RackMultipart20220615-1-avd5ar_html_ba09f39628d6b120.png)

![](RackMultipart20220615-1-avd5ar_html_49f0a8b4e3c225e9.png)

A fairly straightforward list of the different reviews this could&#39;ve used more work and some user testing but I did both those things for the group project in de form of ux testing and a usability test. Which I will link to

## Auth0

I used Auth0 in order to let the user login to the application without needing to register.

![](RackMultipart20220615-1-avd5ar_html_a7c9f71e30eb1b26.png)

![](RackMultipart20220615-1-avd5ar_html_41a83c678c047d76.png)

The picture isn&#39;t showing but that is on my account, on another account is does work

There is also the option to log out.

To work with auth0 I used a tutorial [https://auth0.com/blog/spring-boot-authorization-tutorial-secure-an-api-java/](https://auth0.com/blog/spring-boot-authorization-tutorial-secure-an-api-java/), which already contained a frontend so I used that

![](RackMultipart20220615-1-avd5ar_html_4c976c9b1b4299ba.png)

When you&#39;re logged in with correct roles u can add edit and delete items.

![](RackMultipart20220615-1-avd5ar_html_fb707da75cf299d1.png)

![](RackMultipart20220615-1-avd5ar_html_1369c77f3796446b.png)

![](RackMultipart20220615-1-avd5ar_html_d6fcc32acf8b1388.png)

This checks whether the user actually has the authority in the frontend this is also filtered when you&#39;re not logged in or without the permission buttons wont show up

1.
## You use software tooling and methodology that continuously monitors and improve the software quality during software development.

### Unit testing

![](RackMultipart20220615-1-avd5ar_html_65a99e11f170d685.png)

I added a few unit tests in order to test the functionality of my application I struggled a lot with running all the test for example in de delreview I used to deletebyid but for some reason that wouldn&#39;t work so I tested It like this.

### Integration testing

![](RackMultipart20220615-1-avd5ar_html_d34c5cff1421adf5.png)

I&#39;ve got one measly integration test checking the controller. I have ran some other tests for example testing to post it ![](RackMultipart20220615-1-avd5ar_html_614a1ba926d52f78.png)

But for some weird reason it cant resolve the content object while friend with exactly the same dependencies etc don&#39;t have any problem

![](RackMultipart20220615-1-avd5ar_html_2e8802eaa810d5ad.png)

I also added sonar cloud in order to check bugs and vulnerabilities within my code as you can see there is most Definitely still work to do

![](RackMultipart20220615-1-avd5ar_html_6f5b4ac8ff9e783b.png)

You can also see the review the bugs and see why it is an issue although in my case its about the tests im running so it isn&#39;t high priority

# 4. You design and implement a (semi)automated software release process that matches the needs of the project context.

With github actions before a push or pull request on master I will run tests and when the tests check out it will push an image to docker hub

![](RackMultipart20220615-1-avd5ar_html_c29f829da690630f.png)

![](RackMultipart20220615-1-avd5ar_html_272ef6acb4db0455.png)

![](RackMultipart20220615-1-avd5ar_html_befd6de11832de8d.png)

This was the first version for the backend

And the dockerfile I used

![](RackMultipart20220615-1-avd5ar_html_f060d0a20d35b657.png)

![](RackMultipart20220615-1-avd5ar_html_8ec3fe361bc874.png)

Later I added in Sonarcloud as well to perform static code analysis and discover potential weak point in my code which I wrote about in the previous chapter

![](RackMultipart20220615-1-avd5ar_html_f2270f62456a96aa.png)

All tasks completed and a new image was pushed to docker

I also did this for the frontend in order to be able to run it together this also pushes an image to another docker repository

![](RackMultipart20220615-1-avd5ar_html_24402bceebab5b90.png)

And the dockerfile

![](RackMultipart20220615-1-avd5ar_html_71f79d3b4ce10911.png)

![](RackMultipart20220615-1-avd5ar_html_dcfc38236aecaec2.png)

All tasks completed and an image is pushed.

![](RackMultipart20220615-1-avd5ar_html_3b2114c5ed161504.png)

Both running on different ports I did have some issues getting them to run together but after I added the -p tag in the console it worked

## 8. You act in a professional manner during software development and learning.

I uploaded every research I made unto github in the portfolio and in its own public repository so everyone can find and use it.

Project board here I have user stories im working on and under every user story there&#39;s different tasks I need to finish to split up the user story even more. I started the semester really not using my jira board but gradually towards the end of the year is started using it more and more helping me keep track of my progress and my todos

![](RackMultipart20220615-1-avd5ar_html_d6dff085225a2471.png)

I have a lot of problems keeping my concentration when I&#39;m working I was recommended a certain method by my teacher called pomodoro. Pomodoro breaks up your workday in 25 minutes of work and then a 5 minute break, this helped me keep my concentration and the 5 minute break helped me get a fresh look at things the website I used

-https://pomofocus.io/

![](RackMultipart20220615-1-avd5ar_html_847c7ec124e1be2f.png)

![](RackMultipart20220615-1-avd5ar_html_e8ce63b1c70315d3.png)

I also wrote a few researches where I used the dot framework and apa style for references
