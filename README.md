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

</p>
