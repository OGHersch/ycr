<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>The web site of commercialherschel</title>
    <!-- The style.css file allows you to change the look of your web pages.
         If you include the next line in all your web pages, they will all share the same look.
         This makes it easier to make new pages for your site. -->
    <link href="/style.css" rel="stylesheet" type="text/css" media="all">
  </head>
  <body>
         <style>
            :root {
                /* These variables exist so you can make quick and simple style changes without much CSS knowledge */

                /* applies to all areas */
                --font-family: sans-serif;
                --font-size: 14px;
                --line-height: 1.3em;
                --font-color: white;
                --link-color: #FDFF92;
                --link-text-decoration: none;

                /* main content (between sidebars) */
                --content-padding: 35px;
                --content-bg-color: #1F3848;

                /* header */
                --header-height: 230px;
                --header-background: url('https://commercialherschel.neocities.org/you-couldnt-resist-herschel-sterling.png');
                --header-margin-bottom: 10px;

                /* sidebar */
                --sidebar-margin: 100px;
                --sidebar-width: 320px;
                --sidebar-padding: 15px;
                --sidebar-bg-color: #1F3848;

                /* footer */
                --footer-height: 30px;
                --footer-bg-color: #1F3848;

                /* navbar */
                --navitems-alignment: center;
                --space-between-navitems: 20px;
                --navbar-margin-bottom: 10px;
                --nav-bg-color: #58110F;

                /* container */
                --container-width: 800px;
                --container-bg-color: #58110F;

                /* controls the gap between the content and the footer */
                --row-gap: 5px;

                /* To add scrollbars to your sidebars, just make the height a px value and change overflow to 'auto' */

                --sidebar-height: 80%;
                --sidebar-overflow: hidden;
                --background-color: #58110F;
            }

            html,
            body {
                margin: 20;
                padding: 0;
                background-color: var(--background-color);
                font-family: var(--font-family);
                font-size: var(--font-size);
                line-height: var(--line-height);
                color: var(--font-color);
            }

            body a {
                color: var(--link-color);
                font-weight: bold;
                text-decoration: var(--link-text-decoration);
            }

            #main-container {
                max-width: var(--container-width);
                margin: 0 auto;
                background-color: var(--container-bg-color);
            }

            .flex {
                display: flex;
                margin-bottom: var(--row-gap);
            }

            .content-wrap {
                margin-top: var(--content-margin-top);
            }

            #content-container {
                width: 60%;
                margin-bottom: var(--row-gap);
                background-color: var(--content-bg-color);
            }

            #left-sidebar {
                width: var(--sidebar-width);
                margin-right: var(--sidebar-margin);
                margin-bottom: var(--row-gap);
                height: var(--sidebar-height);
                overflow: var(--sidebar-overflow);
                background-color: var(--sidebar-bg-color);
            }

            #right-sidebar {
                width: var(--sidebar-width);
                margin-left: var(--sidebar-margin);
                margin-bottom: var(--row-gap);
                height: var(--sidebar-height);
                overflow: var(--sidebar-overflow);
                background-color: var(--sidebar-bg-color);
            }

            #header-contained {
                height: var(--header-height);
                margin-bottom: var(--header-margin-bottom);
                background-image: var(--header-background);
                background-position: center center;
            }

            #footer {
                height: var(--footer-height);
                text-align: center;
                color: var(--font-color);
                background-color: var(--footer-bg-color);
            }

            #header-full {
                display: none;
                height: var(--header-height);
                margin-bottom: var(--header-margin-bottom);
                background-image: var(--header-background);
                background-position: center center;
            }

            #navbar-contained {
                margin-bottom: var(--row-gap)
            }

            #navbar-full {
                display: none;
            }

            .nav {
                margin-left: 0;
                text-align: var(--navitems-alignment);
                margin-top: 0;
                margin-bottom: var(--navbar-margin-bottom);
                padding-top: 1em;
                padding-bottom: 1em;
                background-color: var(--nav-bg-color);
            }

            .nav li {
                display: inline-block;
                padding-right: var(--space-between-navitems);
            }

            .wrapper {
                padding: var(--content-padding);
                padding-top: var(--sidebar-padding);
            }

            .sidebar-wrapper {
                padding: var(--sidebar-padding);
                height: var(--sidebar-height);
                overflow: var(--sidebar-overflow);
            }

            .footer-wrapper {
                padding: 5px;
            }

            /* To keep your site RESPONSIVE, make sure this variable matches the width for --container-width UNLESS --container-width is 100% - if it's 100%, you'll need to manually input a breakpoint. */
            @media only screen and (max-width: 800px) {
                .flex {
                    flex-wrap: wrap;
                }

                #left-sidebar {
                    width: 100%;
                    display: block;
                    order: 2;
                    margin-right: 0;
                    margin-bottom: 10px;
                }

                #right-sidebar {
                    width: 100%;
                    display: block;
                    order: 3;
                    margin-left: 0;
                }

                #content-container {
                    width: 100%;
                    display: block;
                    order: 1;
                    margin-bottom: 10px;
                }

            }
        </style>
        <div id="header-full" style="display: block;"></div>
        <div id="navbar-full" style="display: none;">
            <ul class="nav">
                <li><a href="/">Home</a></li>
                <li><a href="#">Link</a></li>
                <li><a href="#">Link</a></li>
                <li><a href="#">Link</a></li>
                <li><a href="#">Link</a></li>
                <li><a href="#">About</a></li>
            </ul>
        </div>
        <div id="main-container">
            <div id="header-contained" style="display: none;"></div>
            <div id="navbar-contained" style="display: none;">
                <ul class="nav">
                    <li><a href="/">Home</a></li>
                    <li><a href="#">Link</a></li>
                    <li><a href="#">Link</a></li>
                    <li><a href="#">Link</a></li>
                    <li><a href="#">Link</a></li>
                    <li><a href="#">About</a></li>
                </ul>
            </div>
            <div class="content-wrap flex alignment">
                <div id="left-sidebar" style="display: block;">
                    <div class="sidebar-wrapper"
                    <br>
                    <br>
                    <br>
                    <br>
                    <center><img src="https://commercialherschel.neocities.org/algorithm.png"><br><br>
                    <br>
                    <br>
                    <br>
                    if you must use $$
                    <br>
                                        <a href="https://ycr.info"target="_blank"</a><img border="0" alt="commercial herschel is your daddy" src="https://commercialherschel.neocities.org/ycr.png" width="180" height="40"
</a>
                      <br>
                 <h2>that is like that
                <br>
                <br>
                and
                <br>
                <br>
                   this is like this:</h2></center>
                    
                  <h3>choose one of the three donations,</h3> and know that i worked a lot on this. the fiat price is 17.50. because you like self-custody, you get choices. if you send a tiny amount, i'll only send it back. in the note area, put in your preferred filetype, pdf, eBook, mobi, or kindle/az. and of course your email address. i will email you a nice, secure file link. 
                    <br> <br>
                    now we can show people that we can do business and be honest and grateful about it with the honor system because the blockchain is transparent. <center><h4>the hash don't lie.</h4></center>
ok?
<br>
<br>
ok. you're welcome. i'm commercial herschel, and i'm here to help. <br><br>
<a href="https://ycr.info" target="_blank">ycr.info</a><br>
<a href="https://myspace.com/commercialherschel" target="_blank">Myspace for the w</a><br>
<a href="https://x.com/herschsterling" target="_blank">Freedom of Speech, <br>Not Freedom of Reach</a><br>
<a href="https://substack.com/commercialherschel" target="_blank">Substack</a><br>
<a href="https://stacker.news/r/herschel" target="_blank">Stacker.news is <br>the news now, clownpants</a>
<br>
<br>
   <center><img border="0" alt="Nobody can resist a convergence of the zeitgeist" src="https://commercialherschel.neocities.org/easytopiantransparent3.png" width="200" height="160"></center><p></p>
   
                      <span></span></div>
                </div>
                <div id="content-container" style="flex-grow: 1;">
                    <div class="wrapper">  <center>you know how cool this is<br><br>
                    <img src="https://commercialherschel.neocities.org/herschel-Sterling-85-flash-fiction.png"><br>
                    <img border="0" alt="everybody wants to improve" src="https://commercialherschel.neocities.org/EVOlution40.png" width="400" height="40"></center>
     <a href="" class="blockoPayBtn" data-toggle="modal" data-uid="d804c3048ab34020"> <img width="160" src="https://www.blockonomics.co/img/pay_with_bitcoin_medium.png"> </a>            
  <lightning-widget 
  name="For Those Who Couldn't Resist " 
  accent="#fdff92" 
  to="herschelsterling@getalby.com" 
  image="https://pbs.twimg.com/profile_images/1876142009016369152/ubf5vdVX_400x400.jpg" 
  amounts="10550, 18500"
/>
<script src="https://embed.twentyuno.net/js/app.js"></script>
                   
<script src="https://www.blockonomics.co/js/pay_button.js"></script>                
  </body>
</html>

