# Slide-presentation-easy-template
A template for presenting PowerPoint slides as a web page

This repository is a fully responsive slide presentation web page;

~~ HOW TO USE ~~

1. Save your PowerPoint presentation as JPGs. (make sure to leave the default names of the JPGs i.e. Slide1.JPG, Slide2.JPG etc.)
    (See note below regarding the image resolution.)

2. Place all the slides into the assets folder (replacing the sample slides).
    (maximum number of slides is 100. For more than 100 slides see instructions below.)

3. That's it! Your presentation is ready to be uploaded to the web as a web page.

~~ ADDITIONAL NOTES ~~


    * The build *

The full design and functionality of this template is accomplished with HTML and CSS only. With the exception of the adaptability to the number of slides, which is accomplished by adding the following inline JavaScript to each image: onerror="this.parentElement.remove()", which simply removes any extra HTML as the page loads.

(You may remove the extra slide <section>s from the HTML as well as the extra <a> thumbnails in the sidebar. This will not affect any functionality)


    * Stylesheet *

The stylesheet is organized and has comments separating each style section, so you can easily edit the styles to your liking.


    * Favicon *

The current favicon is a slide-presentation icon in order not to interfere when adding the slides into the assets folder it has been placed in its own folder named favicon. You can replace it there if you wish. Just remember to name it fav.png or change the reference name in the link.


    * Slide Image Resolution *

Note that by default PowerPoint will save the slides with a 96dpi resolution. This can be changed if you're using Windows. Here are the steps to follow:
1. open Windows RUN command (you can so by typing RUN in the Cortana search bar or by right clicking the start/windows button and selecting "Run".
2. type regedit.exe and press enter.
3. Go to the following directory HKEY_CURRENT_USER\Software\Microsoft\Office\ here choose from 11.0, 12.0, 14.0, 15.0 or 16.0 depending on which version of PowerPoint you're using. 2003 = 11.0, 2007 = 12.0, 2010 = 14.0, 2013 = 15.0 or 2016 = 16.0.
Then open the PowerPoint folder and click on options.
4. Now, go to Edit > New > DWORD (32-bit) Value.
5. Type ExportBitmapResolution as the name.
6. Double-Click on it to open it.
7. In the pop-up box that appears, change the base to Decimal and for the Value Data write the preferred DPI value. You can set it to 300, however since in this case we are using it for a web page, 150 would suffice, as 300 would typically slow down the loading significantly. Click OK and you’re done.


    * For More than 100 Slides *

The template is ready for up to a 100-slide presentation. If you want to use it for a presentation more than 100 slides, then copy and paste <section> lines in the HTML for the additional slides and continue the numbers in the for each slide beyond 100. Note, however, that you will need to continue the numbers up to 5 times per section/slide:
1. for the ID.
2. for the <a> "href" to go to the previous slide.
3. for the slide img source.
4. for the slide img alt (optional).
5. for the <a> "href" to go to the next slide.

And then you need to do the same (or similar) process for the thumbnails. And change the numbers up to 3 times per thumbnail:
1. for the <a> "href" to link to the corresponding slide.
2. for the slide img source.
3. for the slide img alt (optional).

There are extensions to speed up this process. I use "VS Sequential Number" in VS-Code. With an extension like this, the entire process will take only around 3 minutes.

THANK YOU FOR READING, I HOPE YOU FIND THIS TEMPLATE USEFULL.