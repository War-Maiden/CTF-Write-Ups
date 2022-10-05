Have you ever wondered what people can know about you? Probably not. But if you have uploaded anything on the internet, chances are that someone can trace it back to you or use it to trace you. Would you like to be able to do the same? Try the OhSINT room where you get the chance to track someone's online shenanigans and even (!) crack their password! (The link to the OhSINT room can be found here: https://tryhackme.com/room/ohsint )

What you'll need:
- Your favourite EXIF viewer (in this write-up, I'm using https://exifdata.com/index.php an online tool that lets you view picture metadata).
- Google
- Your favourite wireless network mapping tool (WiGLE will be used for this one).
- A lot of patience for the upcoming HTML games.

When you download the file offered by the room you get a very popular landscape photo (see below):

![WindowsXP (1)](https://user-images.githubusercontent.com/36206945/194040411-37b67ebb-5551-44bb-947c-e27e3e49bb7d.jpg)

So how do you get someone's password from this picture? There are a few steps involved. Disclaimer - when using Open Source Intelligence it's about where the information takes you. The methodology presented here is not a template for any OSINT project.

Firstly, run the picture through the EXIF viewer. The data received gives us some useful information.

![#2](https://user-images.githubusercontent.com/36206945/194042944-2f89864c-7679-486a-85e2-5ef7823b13f4.png)

From here, we see that the picture belongs to someone named OWoodflint. The name is peculiar so only one thing to do - google OWoodflint.

![#3](https://user-images.githubusercontent.com/36206945/194043460-0b429bc4-806b-4568-9b91-a06ae3cff462.png)

Now we have everything we need to go through the questions one by one.

1. What is this user's avatar of?

Avatar usually refers to a person's profile picture. Based on the above screenshot, if we go into his Twitter account, we can see that his profile picture is as below.

![#4](https://user-images.githubusercontent.com/36206945/194044214-143cf8e7-81d7-4b30-ad2d-0ce702451776.png)

A cat! 

2. What city is this person in?

Going into his GitHub account, we can see him mentioning London as the city he is from. From his Twitter account, we can see him publicly broadcasting a BSSID. 

![#5](https://user-images.githubusercontent.com/36206945/194045012-4dcb92a0-4373-4293-a73a-83cf1fabd1af.png)

Maybe this will be a clue to his location. Using WiGLE, let's run an advanced search using the BSSID provided. 

![#6](https://user-images.githubusercontent.com/36206945/194045427-78240ee5-5193-47c8-a7d0-0e5d62ff5594.png)

Going into the map, we see that the network is located in London. Thus, his location is London.

3. What's the SSID of the WAP he connected to?

If we look again at the results of the WiGLE search, we can see that the SSID is Unilever WiFi.

4. What is his personal email address?

His personal email address can be found on his GitHub page and is OWoodflint@gmail.com

5. What site did you find his email address on?

That would be GitHub as previously stated:)

6. Where has he gone on holiday?

When we go back to his blog, we see that he mentions New York as his holiday destination.

![#7](https://user-images.githubusercontent.com/36206945/194047528-85ca10af-eaf4-4092-b200-73dc1a514f2c.png)

7. What is this person's password?

Before you read the solution, look through his site's HTML:) Hint, it's in the comments!

If you look hard enough you will see that his password is -- pennydr0pper.! -- 

Hope you enjoyed! OSINT is an incredible thing, is it not?
