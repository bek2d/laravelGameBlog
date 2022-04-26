# laravelWebsite
Game blog made using Laravel, HTML/CSS, Bootstrap


﻿Screenshots for each feature/requirements for the web site

The welcome page of our blog for guets is Sign In/Sign Up page. Therefore in Laravel the route is '/' or just empty. This layout is typical almost for all social websites on the Internet. Therefore on the left you can observe our logo with the motto below it. On the right side of the page, there is a standard form. On this screenshot we can see an attempt to enter a blank field and front-end validation that prevents it. Another thing is a footer. Footer was t contains feedback form, which is tested on the next screenshot.![](readmeImages/Aspose.Words.42eb1005-8c39-43de-bfc4-f5f46887d748.001.png)

Below is zoomed and filled version of the feedback footer. From grid layout and buttons it is clear that Bootstrap was used.![](Aspose.Words.42eb1005-8c39-43de-bfc4-f5f46887d748.002.png)

After submitting a form a success message pops out, so the user knows that feedback was sent.![](Aspose.Words.42eb1005-8c39-43de-bfc4-f5f46887d748.003.png)

Using Feedback controler and Mail in Laravel, feedback messages are sent to ipprojecttestmail@gmail.com. Below the same message as above in the footer, with details is recieved. 

From the welcome page it is clear that our main colors are red, black and white. However, backround is grayish, as our team observed on many other blogs. It is worth mentioning that our site uses Manrope font from Google Fonts. Our logo is influeced by gaming news company PCgamer(www.pcgamer.com). Our recreation in graphics application has mainly two types of logos, full and compact one. As an experiment our compact logo is in SVG format, so it can be stretched and still have good quality. ![](Aspose.Words.42eb1005-8c39-43de-bfc4-f5f46887d748.004.png)![](Aspose.Words.42eb1005-8c39-43de-bfc4-f5f46887d748.003.png)

![](Aspose.Words.42eb1005-8c39-43de-bfc4-f5f46887d748.005.png)![](Aspose.Words.42eb1005-8c39-43de-bfc4-f5f46887d748.006.png)

Next is the registration page. Route is '/register'. Laravel Breeze was used to create authorization system. Thus, if we assume that a user has logged in on the start page. Trying to access the registration page will redirect an authorized user to '/feed' (will be mentioned later).![](Aspose.Words.42eb1005-8c39-43de-bfc4-f5f46887d748.007.jpeg)

Sign up form has both types of validation front-end and back-end. Below are some examples of back-end validation. After submission all field are stored in database User model.![](Aspose.Words.42eb1005-8c39-43de-bfc4-f5f46887d748.008.png)

After successfully creating an account or signing in. Users are redirected to home feed. With the help of middleware now this is the welcome page for authorized users.  The feed is chronological, fresh articles are showed first. Footer is the same as on screenshots above, with feedback form and mailing functionality. However, now users have the header. Pressing Home button will just refresh the page because we are already on home page. LogOut lets users to sign out from their account and redirects 

to Sign In/Sign Up page. 

![](Aspose.Words.42eb1005-8c39-43de-bfc4-f5f46887d748.009.png)

If we click on Add article '/add\_article' page will open. Inputs are Catergory, Title, Content. 

![](Aspose.Words.42eb1005-8c39-43de-bfc4-f5f46887d748.010.png)

Using dynamic routing right after posting an article user is redirected to a newely added article page.

![](Aspose.Words.42eb1005-8c39-43de-bfc4-f5f46887d748.011.png)

Thanks to Bootstrap articles can be read from mobile devices.![](Aspose.Words.42eb1005-8c39-43de-bfc4-f5f46887d748.012.png)

Now our article is at home feed. On the screenshot below there are two authors that are distinguished by username. Users can delete only their articles. That is why there is no delete option on the second article card.![](Aspose.Words.42eb1005-8c39-43de-bfc4-f5f46887d748.013.png)

Chosing the delete option returns a success message.![](Aspose.Words.42eb1005-8c39-43de-bfc4-f5f46887d748.014.png)
