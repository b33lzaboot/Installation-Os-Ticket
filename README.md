<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 11</b> (21H2)

<h2>List of Prerequisites</h2>

- A computer
  - Where you set up OS ticket 
- A web server
  - This is where the website is hosted usually this will already be provided by default, when connected to the internet your computer is already running through this. The only thing that is different is the group that you are apart of on OS ticket
- A database (HeidiSQL)
  - A place where files are stored, most databases are cloud based now so having something stored on a hardware based server would be company based.
- PHP
  - A coding language that helps the OS ticket work in the background, this is not something that you need to know.
- A web browser
  - This is where you would go to find the website, Google chrome, firefox, opera. your choice.

<h2>Installation Steps</h2>

<p>
<img width="1332" height="955" alt="Screenshot 2026-10-19 175350" src="https://github.com/user-attachments/assets/ac5c1abb-b1c7-4bb2-a4b4-66806cecbe51" />

</p>
<p>
In order to install OS ticket you must first navigate to the website https://osticket.com/editions/ This will take you to three different versions of the same program, for this tutorial we will install the free open source version.
</p>
<br />

<p>
<img width="1242" height="958" alt="Screenshot 2026-10-20 225141" src="https://github.com/user-attachments/assets/6c83feef-d270-43a1-9baa-55659063ce94" />

</p>
<p>
Once you see this screen make a custom version based off what you comapany requires, usually you won't have to do this cause most companies already have a version downloaded on a company computer or virtual cloud when using a virtual machine.
</p>
<br />

<p>
<img width="902" height="507" alt="Screenshot 2026-10-21 160102" src="https://github.com/user-attachments/assets/48393bf2-fe7d-4029-91c7-77d692fba23f" />

</p>
<p>
Once you have chosen the customized version for you company you will get a zip file that looks like this in your downloads section of your file explorer, you are going to unzip it.
</p>
<br />

<p>
<img width="393" height="508" alt="Screenshot 2026-10-20 231550" src="https://github.com/user-attachments/assets/3b3a2b7f-c18d-442a-8a66-efa9b93922ed" />

</p>
<p>
 Once unzipped you will get a file that looks like this and you want to install all of the programs within, these are all required to run OS ticket
</p>
<br />

<p>
<img width="897" height="506" alt="Screenshot 2026-10-21 161445" src="https://github.com/user-attachments/assets/6d24784e-e67b-47fd-b7df-aabe28611a11" />

<img width="329" height="297" alt="Screenshot 2026-10-21 161525" src="https://github.com/user-attachments/assets/59d07d54-4e41-421c-aea9-9c0c2751bd8d" />

<img width="328" height="292" alt="Screenshot 2026-10-21 161539" src="https://github.com/user-attachments/assets/be82cde2-13ba-4801-8056-2ffd71c37075" />

</p>
<p>
Before you can fully install OS ticket you must first install the IIS using CGI, in order to do this you must go to your programs and click on turn on and off windows features. once you click on this you must enable Internet information services, once enabled click on the plus sign right next to it and find world wide web services and enable that, once you have done that click the plus sign next to it and find Application Development features, make sure thats enabled and click the plus sign next to it and find CGI and enable it and it should find and download the file for you.
</p>
<br />

<p>
<img width="388" height="506" alt="Screenshot 2026-10-21 154903" src="https://github.com/user-attachments/assets/270bb29c-217b-40c8-aa0f-449dbb88d284" />
<img width="389" height="505" alt="Screenshot 2026-10-21 154931" src="https://github.com/user-attachments/assets/7fd2b664-d76d-4fc6-81fd-cdaaefd9f47a" />


</p>
<p>
Now you can install the PHP manager and rewrite
</p>
<br />

<p>
<img width="530" height="507" alt="Screenshot 2026-10-21 155014" src="https://github.com/user-attachments/assets/845902f8-64fe-4d9a-a7d9-bb4f1a2c6387" />
<img width="600" height="772" alt="Screenshot 2026-10-21 155117" src="https://github.com/user-attachments/assets/76500196-fdd8-4045-978c-4162e09ff474" />

</p>
<p>
Now you must make a folder within you C drive called PHP this is for the PHP zip file, unzip the file and put this file win the PHP file you just created
</p>
<br />

<p>
<img width="440" height="569" alt="Screenshot 2026-10-21 221613" src="https://github.com/user-attachments/assets/b48fff2f-aefe-4990-b362-9226a7607ae1" />
<img width="391" height="305" alt="Screenshot 2026-10-21 165245" src="https://github.com/user-attachments/assets/b050f709-95ca-4cc8-9ac3-8fb533a35a47" />
<img width="456" height="347" alt="Screenshot 2026-10-21 221152" src="https://github.com/user-attachments/assets/1c48a68f-f483-4efa-adab-f3accd024f73" />
</p>
<p>
Next step is to install mysql which is a database for OS ticket, the username and password that is used is just an example for the standard configuration, this would normally not be the username and password, its just an example but I used ROOT for both. the install for the database is very simple, so just follow the prompt that the computer gives you. 

</p>
<br />

<p>
<img width="626" height="516" alt="Screenshot 2026-10-21 165728" src="https://github.com/user-attachments/assets/548d6d53-92f2-4297-9e86-f9ad92ec4fc8" />
<img width="742" height="837" alt="Screenshot 2026-10-21 165705" src="https://github.com/user-attachments/assets/443081ab-bc66-440a-a685-2d36cdc68621" />
<img width="860" height="713" alt="Screenshot 2026-10-21 222648" src="https://github.com/user-attachments/assets/75b85c4e-e114-44ed-9181-d1e3f9403473" />
<img width="850" height="760" alt="image" src="https://github.com/user-attachments/assets/da8dc0d8-69fa-41da-90b0-b58ae6227a75" />
<img width="816" height="516" alt="Screenshot 2026-10-21 222836" src="https://github.com/user-attachments/assets/f6c4cc16-aaef-46ea-8b37-c13159b17fe6" />
<img width="464" height="200" alt="Screenshot 2026-10-21 222858" src="https://github.com/user-attachments/assets/0b47a537-b300-4212-9546-2fee2737de88" />
<img width="184" height="228" alt="image" src="https://github.com/user-attachments/assets/8f2b9a5b-33c3-4fd9-8cb9-7d7571457236" />
</p>
<p>
The next step is to set up the PHP within the IIS that you configured within your windows programs earlier in the tutorial, when you open up the IIS you want to go to PHP manager, then select Register new PHP and select the PHP.CGI file within the PHP folder that you created earlier, once this is done go ahead and restart the server, by stopping it and starting it back at the homepage
</p>
<br />

<p>
<img width="614" height="583" alt="Screenshot 2026-10-21 225752" src="https://github.com/user-attachments/assets/e98989fc-5606-4a81-9bac-d220e00cde39" />
<img width="722" height="607" alt="Screenshot 2026-10-21 225936" src="https://github.com/user-attachments/assets/c6aaa772-2129-4ccb-acb6-553fa92de8e6" />
<img width="796" height="939" alt="Screenshot 2026-10-21 225911" src="https://github.com/user-attachments/assets/e2a4c73d-db14-48d5-84dc-296286f08fb7" />
<img width="614" height="403" alt="Screenshot 2026-10-21 230002" src="https://github.com/user-attachments/assets/682edd56-181a-4a1b-b92f-e14f340f65bb" />

</p>
<p>
Next you are going to open the inetpub folder and clicking wwwroot, open the os ticket folder that you unzipped and find the upload folder and copy that folder into the wwwroot folder and change the name of the upload to osticket make sure it is done exactly how you see it in the photos otherwise it can cause errors to show on the website. The process of moving the file over depending on your internet or the internet that is hosting the VM could take some time, so take a stretch if needed
</p>
<br />

<p>
<img width="183" height="291" alt="Screenshot 2026-10-21 231240" src="https://github.com/user-attachments/assets/11066e78-83df-4c13-b178-4183524beb9c" />
<img width="146" height="224" alt="Screenshot 2026-10-21 231251" src="https://github.com/user-attachments/assets/292b7d64-a452-49a1-bd8e-e39abbcb0b3e" />
<img width="841" height="946" alt="Screenshot 2026-10-22 025609" src="https://github.com/user-attachments/assets/3aa10a49-93c0-47b4-839c-0a0136c4a6f6" />

</p>
<p>
Once the file is moved and changed go back to the IIS and find the osticket-vm tab on the left side of the window in the data base and click on it to expand it and find the HTTPS 80 on the right hand side and click on it, this should bring you to the website with a checklist if done correctly.
</p>
<br />

<p>
<img width="858" height="957" alt="Screenshot 2026-10-22 031126" src="https://github.com/user-attachments/assets/7a3fdeea-066c-411f-a1a7-3587fa39e82c" />
<img width="825" height="972" alt="image" src="https://github.com/user-attachments/assets/6c07033a-1bb8-4518-a2d5-10e5dc7a1cb3" />

</p>
<p>
we are near the final step, I know this has been a bit of a marathon, but you're doing great, from here you are going to go back to the IIS and active the remanding X's you see on the website. When back in the IIS you want to go to PHP Manager and Enable php_imap.dll, php_inti.dll and php_opache.dll. Once you do this go back and refresh the webpage that OS ticket is on and the everything should be check marks accept for the bottom two do not worry about these.
</p>
<br />

<p>
<img width="644" height="446" alt="Screenshot 2026-10-22 031533" src="https://github.com/user-attachments/assets/3ad66976-4c90-4b06-9f2e-1e4e69dd7ed4" />
<img width="614" height="605" alt="Screenshot 2026-10-22 031547" src="https://github.com/user-attachments/assets/31dde849-0e1b-4aac-9f44-83fd39f502c2" />
<img width="605" height="556" alt="Screenshot 2026-10-22 031614" src="https://github.com/user-attachments/assets/e47dfd1f-35ab-4216-a3dc-46a2e7c0ef54" />
<img width="259" height="253" alt="Screenshot 2026-10-22 031626" src="https://github.com/user-attachments/assets/b9e2ab1a-0c2e-464c-97de-d2b0e73e8abe" />
<img width="139" height="59" alt="Screenshot 2026-10-22 031644" src="https://github.com/user-attachments/assets/16aacbd7-d785-416b-b7bc-b9179421a8b9" />

</p>
<p>
Next step is to go back to the wwwroot folder, click on osticket and find the include file, once within the include file scroll down until you find ost-sampleconfig.php and rename it ost-config.php
</p>
<br />

<p>
<img width="250" height="254" alt="Screenshot 2026-10-22 033259" src="https://github.com/user-attachments/assets/1456fc98-e6d8-40ea-84d7-c8058eac9062" />
<img width="330" height="470" alt="Screenshot 2026-10-22 033349" src="https://github.com/user-attachments/assets/04aa9d3d-149a-46cd-831a-11caf9d20c3f" />
<img width="684" height="473" alt="Screenshot 2026-10-22 033409" src="https://github.com/user-attachments/assets/a379ab6d-ee01-4bf1-9ad1-194390214c35" />
<img width="474" height="244" alt="Screenshot 2026-10-22 033436" src="https://github.com/user-attachments/assets/a21c28ae-3348-4afe-97e2-8842eed3dcf5" />
<img width="706" height="473" alt="Screenshot 2026-10-22 033512" src="https://github.com/user-attachments/assets/ca925450-8867-4dfd-b5c5-c91d0a16fd33" />
<img width="840" height="538" alt="Screenshot 2026-10-22 033522" src="https://github.com/user-attachments/assets/7813e3b5-825c-4f37-a86e-519ec9750ef4" />
<img width="836" height="542" alt="Screenshot 2026-10-22 034633" src="https://github.com/user-attachments/assets/54457bd2-54dd-4b65-bca6-1633053e37de" />
<img width="830" height="538" alt="Screenshot 2026-10-22 033559" src="https://github.com/user-attachments/assets/758d4905-166f-4c7a-87bd-f4b393c70c0b" />
<img width="704" height="470" alt="Screenshot 2026-10-22 033610" src="https://github.com/user-attachments/assets/9b606b79-3d7c-470d-b71e-5c1a8f2c2709" />


</p>
<p>
Once you have done this right click on the file you just switched and go to properties and navigate to the security tab, once in the security tab and click advanced, at this point you should be under permissions, go ahead and disable all permissions and when the window comes up say get rid of all permissions, once this is done the page that you were on before should be blank and go ahead and click add to add permissions select add a principle. For the sake of the tutorial we put everyone just to make sure that it will work no matter what. In a real life seniero your company would tell you what permissions to give OS ticket to.
</p>
<br />

<p>
<img width="747" height="869" alt="Screenshot 2026-10-22 035618" src="https://github.com/user-attachments/assets/1f3d798e-a7b0-49e3-8101-fcf686b433e2" />

</p>
<p>
Now go back to the os ticket website and click continue to finish setting up the account, follow the prompt that is given and fill out what ever name you want for os ticket, for the sake of the tutorial I used for the admin user, username: adminuser and password: Password1. your company will likely have this already provided for you. Before you can finish the installation however you must fill out the SQL field and in order to do this we must now install HeidiSQL
</p>
<br />

<p>
<img width="619" height="372" alt="image" src="https://github.com/user-attachments/assets/5b001282-8654-462b-95e1-4dc74ac8af8b" />
<img width="627" height="438" alt="image" src="https://github.com/user-attachments/assets/bc8c3bc3-155f-4d6c-9635-0591fddcb4cd" />
<img width="624" height="423" alt="image" src="https://github.com/user-attachments/assets/4ca12772-e609-4f4f-9f48-6fb6c1146aed" />
<img width="255" height="420" alt="image" src="https://github.com/user-attachments/assets/00cce2f2-fb76-47fa-93ec-8d15e63cd13b" />
<img width="435" height="385" alt="Screenshot 2026-10-22 040655" src="https://github.com/user-attachments/assets/4e7b9611-6181-465b-a397-caf0ceea2740" />
<img width="288" height="226" alt="Screenshot 2026-10-22 040723" src="https://github.com/user-attachments/assets/e6cb7598-d512-4c5c-a4a2-1d9b8d818a76" />

</p>
<p>
HeidiSQL allows us to make a connection to our database, when installing just hit next on everything and when the install is done, hit new at the bottom and it should bring you to settings where you can see the username we made earlier in MySQL just use the password that you provided and click open, this will open the connection to your database, after you click open you will see the unnamed data base, right click on it and rename it to exactly what you see in the picture and click ok.
</p>
<br />

<p>
<img width="753" height="369" alt="image" src="https://github.com/user-attachments/assets/56ddc943-03b0-4d3b-9085-757200d15c6f" />
<img width="750" height="583" alt="image" src="https://github.com/user-attachments/assets/d433f2dd-db57-473f-89c8-131b156ce1d6" />

</p>
<p>
From here go back to the browser and fill out the MySQL section of the install page the username and password will be the same as the MySQL and the name of the data base will be osTicket. Once you have done this click install and you should be done. the second picture is what it should look like. And don't forget that if you are using a VM make sure you delete everything and make sure everything is uninstalled before you close out the VM.
</p>
