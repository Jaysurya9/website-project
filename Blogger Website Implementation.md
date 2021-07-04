# Project-1 - Creating a Blog Website

<hr>

<b>Step 1:</b> Choose a Hosting Platform 

Select Hosting platform – [“Azure" | "Wordpress” | “Blogspot/Blogger” | “Google Cloud” | "GitHub Pages"] 

Choosing a Hosting Platform

Choice -> Blogspot/Blogger

Reasons for Choosing Blogspot/Blogger
<ul>
    <li>Hosting is Free</li>
    <li>Free Domain Linkup</li>
    <li>Free SSL/HTTPS</li>
    <li>Easy Navigation and Creations using UI</li>
    <li>Easy Integrations</li>
 </ul>
 
Step Below are for Blogspot/Blogger

<hr>

<b>Step 2:</b> Create a Blog in Blogger.com

<a href="https://Blogger.com" alt="Create a Blogspot" target="_blank">Click Here to create a Blog</a>

Choosing a Blog Name: 

Add Blog Title and Name and get started
        
Go to Setting and add basic details of the Blog

<ul>
    <li>Add Title</li>
    <li>Add Description</li>
    <li>Select Blog Language</li>
    <img src="Images/Blog Basic Settings.PNG" alt="Blog Basic Settings">
    <li>Add Google Analytics property ID <br>Property ID Startswith/looks like <b>UA-12345678-1</b></li>   
    <li>Add Favicon</li>
    <img src="Images/Congifure Favicon.PNG" alt="Congifure Favicon">
    <li>Enable Privacy - Visible to Search Engines to find on Website/Blog</li>
    <img src="Images/Enabling Privacy - Visible to Search engines.PNG" alt="Enabling Privacy - Visible to Search engines">
</ul>
 
<hr>

<b>Step 3:</b> Choose a Domain Name 

<ul>
    <li>Search Pricing and Costing of a Domain</li>
    <li>Analysis of Selecting Domain name keywords - that which users use frequently</li>
    <li>Purchase a Domain (.com, .in, .net)</li>    
</ul>

REGISTER Domain (For Example: NameCheap | GoDaddy | Freenom)

Your Choice -> Freenom

Choosing a Domain Name:
      
<hr> 

<b>Step 4:</b> Configure Domain Settings in DNS Management <br> 

connect domain to hosting platform<br>
Blogger Settings<br>
--> Custom Domain <br>
--> add Custom Domain For Example: <b>www.<domain_name>.com</b>  <br>

Adding Records to Domain Settings in DNS Management<br>
Add the following two CNAMEs 

Add a 1st CNAME Record

    Type = CNAME	
    Name = www	 
    Value = ghs.google.com
    TTL = 1/2 Hour
    
Add a 2nd CNAME Record
    
    Type = CNAME	
    Name = 	<Unique-blogger-Host-Value>  //get it from Blogger Domain Settings
    Value = <blogger-Host-Value>.dv.googlehosted.com  //get it from Blogger Domain Settings
    TTL = 1/2 Hour
    
    
**Reference Image**

<img src="Images/Add CNAME Record.PNG" alt="Add CNAME Record">
    
Add A Record  ---> Reference: To Get A Record List -> https://www.blogger.com/go/customdomain

    Type = A	
    Name = 	@
    Value = 216.239.32.21
    TTL = 1/2 Hour

Add these 4 A-records that point to Google IPs:

    216.239.32.21
    
    216.239.34.21
    
    216.239.36.21

    216.239.38.21
       
    
**Reference Image**

<img src="Images/Add these 4 A-records that point to Google IPs.PNG" alt="Add these 4 A-records that point to Google IPs">
    
--> Redirect Blog to Website Domain Name <b>www.<domain_name>.com</b>  

<hr>

<b>Step 5:</b> Enable SSL/HTTPS and HTTPS Redirect in Blogger Settings

**Reference Image**

<img src="Images/Enable SSL_HTTPS and HTTPS Redirect.PNG" alt="Enable SSL/HTTPS and HTTPS Redirect">

<hr>

<b>Step 6:</b> Choose a Theame 

Select a responsive web theme and upload XMLfile to blogger.

<b>Adding Website Home SEO Meta Tags</b>

Enable website html concent add the below script content at the beginning

**Note** : Change Script Modifications according to website template content

    <head>
    <!-- SEO -->
        <!-- Primary Meta Tags -->
        <title> add website title here </title>
        <meta name="title" content="add website title here">
        <meta name="description" content="add website description">
        <meta name="robots" content="index, follow">
        <link rel="alternate" hreflang="en-in" href="https://<domain_name.in/com"/>
        <meta content='add site domain name' property='og:site_name'/>
        
        <!-- GeoLocation Meta Tags -->
        <meta content='20.593684; 78.96288' name='geo.position'/>
        <meta content='INDIA' name='geo.placename'/>
        <meta content='ISO 3166-2:IN' name='geo.region'/>
        <meta name="country" content="IN">
        
        <!-- Open Graph / Facebook -->
        <meta property="og:type" content="website">
        <meta property="og:url" content="https://<domain_name.in/com">
        <meta property="og:title" content="add website title here">
        <meta property="og:description" content="add website description">
        <meta property="og:image" content="website-Logo.jpg/png">
        
        <!-- Twitter -->
        <meta property="twitter:card" content="summary_large_image">
        <meta property="twitter:url" content="https://<domain_name.in/com">
        <meta property="twitter:title" content="add website title here">
        <meta property="twitter:description" content="add website description">
        <meta property="twitter:image" content="website-Logo.jpg/png">
        
        <meta name="keywords" content=" add website keyword here seperated by "," ">
        
        <link rel="shortcut icon" href="add website favicon.png" type="image/x-icon">
        <link rel="icon" href="add website favicon.png" type="image/x-icon">
        
    <!-- End Of SEO -->
    </head>

<hr>
    
<b>Step 7:</b> Create a Post 

<ul>
    <li>Add a post title - try to add small titles</li>
    <li>Add a post</li>
    <li>Add Page topic related Labels</li>
    <li>Add Custom page Url based on Page Title</li>
    <li>Add Location to appear post on area</li>
    <li>enable search description and full length page title</li>
    <li>Add Custom robot tags to default</li>
</ul>   

<b>Adding Page SEO Meta Tags</b>

Enable post html concent add the below script content at the beginning

**Note** : Change Script Modifications according to page content

    <head>
    <!-- SEO -->
        <!-- Primary Meta Tags -->
        <title> add page title here </title>
        <meta name="title" content="add page title here">
        <meta name="description" content="add page description">
        <meta name="robots" content="index, follow">
        <link rel="alternate" hreflang="en-in" href="https://<domain_name.in/com/<page-titel>"/>
        <meta content='add site domain name' property='og:site_name'/>
        
        <!-- GeoLocation Meta Tags -->
        <meta content='20.593684; 78.96288' name='geo.position'/>
        <meta content='INDIA' name='geo.placename'/>
        <meta content='ISO 3166-2:IN' name='geo.region'/>
        <meta name="country" content="IN">
        
        <!-- Open Graph / Facebook -->
        <meta property="og:type" content="website">
        <meta property="og:url" content="https://<domain_name.in/com/<page-titel>">
        <meta property="og:title" content="add page title here">
        <meta property="og:description" content="add page description">
        <meta property="og:image" content="Page-Featured-Image.jpg">
        
        <!-- Twitter -->
        <meta property="twitter:card" content="summary_large_image">
        <meta property="twitter:url" content="https://<domain_name.in/com/<page-titel>">
        <meta property="twitter:title" content="add page title here">
        <meta property="twitter:description" content="add page description">
        <meta property="twitter:image" content="Page-Featured-Image.jpg">
        
        <meta name="keywords" content=" add page content keyword here seperated by "," ">
        
        <link rel="shortcut icon" href="add website favicon.png" type="image/x-icon">
        <link rel="icon" href="add website favicon.png" type="image/x-icon">
        
    <!-- End Of SEO -->
    </head>
 
<hr>   

<b>Step 8:</b> Create Logo and Change Logo

<hr>

<b>Step 9:</b> Create Pages Add Pages like Contact, About, Support, Feedback, SiteMap,…etc.

<hr>

<b>Step 10:</b> Adding Navigation links Add Page Navigation Links to Top Header Menu and Footer Menu10

<hr>

# Website Integrations

<b>Step :</b> Track and Monitor Website using Google Analytics
    
<b>Analyze performance</b><br>
Gather and analyze data to gain insights on Website/business performance and find areas to improve.   
    
<b>Get to know your customers with Google Analytics</b><br>
Connect Webiste/Blog/Store with Google Analytics to get a deeper understanding of who your customers are, where they come from, and how they interact with your Webiste/Blog/Store
    .
<b>Set Up Google Analytics - Get more detailed insights and reports</b><br>
Learn the number of site visitors, how well they convert to customers, and other important metrics to get a detailed overview of your business performance.
    
Get Started <br>
Create a Google Analytics @ https://analytics.google.com/ 
    
Set up the Analytics global site tag <br>
Refer: https://support.google.com/analytics/answer/1008080?hl=en#zippy=%2Cin-this-article
    
Set up Analytics for a website (Universal Analytics) <br>
Refer: https://support.google.com/analytics/answer/10269537?ref_topic=1009620
    
Add Global Site Tag (gtag.js) tracking code
    
Copy and paste tracking code code as the first item into the <HEAD> of every web page that we/you want to track. <br>
If you already have a Global Site Tag on page, simply add the config line from the snippet below to your existing Global Site Tag.
    
Tracking Code looks like this and property tag has to be added
    
    <!-- Global site tag (gtag.js) - Google Analytics -->
    <script async src="https://www.googletagmanager.com/gtag/js?id=UA-12345678-1"></script>
    <script>
      window.dataLayer = window.dataLayer || [];
      function gtag(){dataLayer.push(arguments);}
      gtag('js', new Date());

      gtag('config', 'UA-12345678-1');
    </script>

<hr>

Step : Add Website to Google Search Engine 

Login to Google Search Console and Add Website to domain or url.

<hr>

Step : Integrate Sitemap 
     
Blogger XML Sitemaps - Easily generate XML sitemaps for your Blogger (blogspot) blogs for better SEO<br>
Generate Sitemap online @ <a href="https://www.labnol.org/blogger/sitemap/" alt="generate XML sitemaps for your Blogger (blogspot) blogs for better SEO" target="_blank">Click Here</a>
<img src="Images/Generate XML Sitemaps for Blogger.PNG" alt="Generate XML Sitemaps for Blogger">

reference link: <a href="https://www.labnol.org/internet/submit-blogger-sitemap-to-google/10149/" target="_blank">How to Add an XML Sitemap to your Blogger Blog</a>

Enable Custom Robot and add sitemap code to Custom Robot in Blogger settings.
    
<hr>
    
<b>Step:</b> Integrate Programmable Search Engine on website   
      https://programmablesearchengine.google.com/  
    
Add a customizable search box to your web pages and show fast, relevant results.
    
<hr>

Step : Website Automation @ https://ifttt.com/

Auto Posting - RSS/ATOM Feed to Twitter

Step : Email Notifications for Google Forms<br>
https://gsuite.google.com/marketplace/app/email_notifications_for_google_forms/984866591130
