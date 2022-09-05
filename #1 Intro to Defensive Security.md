CAUTION - This is a room available only to THM subscribers. If you decide to take out a subscription, create an account using your student email, and a student discount will be automatically applied.
Intro to Defensive Security aims to provide a taste of what a day in defensive security looks like. This write-up will cover the experience of using a SIEM to detect and counter suspicious activity
This room does not require deployment of a virtual machine.
Once Tasks 1 and 2 have been completed, click the launch button at the top right of Task 3.

#1
![(1)](https://user-images.githubusercontent.com/36206945/188478917-4daa262d-2568-45fe-9ee3-6574529a731e.png)

The screen that we would see after launching the site is as follows:

#2
![(2)](https://user-images.githubusercontent.com/36206945/188479241-2382f7ed-af57-4590-a4a7-54597e27be20.png)

The screen is what a SIEM software main screen would look like. We can see statistics on topology and logins and a detailed alert log. It is with this alert log that we will work with in this write-up. If we were to go over the logins with our cursor, the software would tell us if a login is deemed suspicious or safe.

#3
![(3)](https://user-images.githubusercontent.com/36206945/188479704-a345d493-1423-44cd-b293-d427a7608482.png)
#4
![(4)](https://user-images.githubusercontent.com/36206945/188479720-655792fc-69ae-4066-8a42-841436eadfc3.png)

As we can see, the login in the picture above is outlined as red so the software thinks it is suspicious. But we can see on image #3 that the same IP address had successfully logged on. This means that a potential security breach is present.

Our next step is to check if the IP address is suspicious or trustworthy. This can be done by running the IP through a public database as shown in image number 5. In image 6, we get the result that the IP address is suspicious and can move on to the next part of the activity.

#5
![(5)](https://user-images.githubusercontent.com/36206945/188480302-6f872c66-3c12-4b38-ba78-a70a55977a6b.png)
#6
![(6)](https://user-images.githubusercontent.com/36206945/188480352-76ade2c3-6268-403d-a7cf-519824e026b2.png)

Since we are now certain that this is more than likely a security breach, we have to report it. The next screen asks about the most appropriate person to report this security breach too. 
(!: It is important to know that chain of command might differ depending on the workplace and the policies governing it)

#7
![(7)](https://user-images.githubusercontent.com/36206945/188481371-ebb17d22-e2fd-444c-945f-0a1156fac1cc.png)

Finally, permission is given to block the IP address from the system thus stopping the attack. Once the IP is blocked, a flag will be provided that is necessary for completion of the room.

#8
![(8)](https://user-images.githubusercontent.com/36206945/188481612-08a1d859-ce94-43b1-9b3c-75ad004f6c38.png)
