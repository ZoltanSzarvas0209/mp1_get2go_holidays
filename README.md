
![logo](assets/images/get2goholidays_logo.png)

## Introduction

Hi there, 

Get2Go Holidays is a made up travel agent website. It was created for educational purpose as my first milestone project for Code Institute's Web Development course.

It is a static website developed using html, css and bootstrap. The content of the site is limited for simplicity , however fully scalable for future extensions.



## UX

The metholody of UXD was used in the planning and development of the project. 
The choosen project is a travel agent's website to advertise and generate leads for bookings as part of a franchise. As code institute's first milestone project, an at least 3 page static website was required.

### Technologies and Tools Used

* Languages

    * HTML
    * CSS

* Framework

    * Bootstrap

* Version Control

    * Git
    * Github
    * Gitpod


* additional resources
    * FontAwesome: fonhttps://fontawesome.com/search?o=r&m=free&s=solid  - used for icons throughout the site
    * ChatGPT: https://chat.openai.com/   - used to create content for the brochure

### Objective

* The main objective of the website is to establish an online presence and create leads that can be converted into sales

### Research

Get2Go holidays was a side hussle of mine, while it eventually failed it is the base of the idea of this project. 

In order to gain a good understanding of the requirements I conducted a research and visited several travel websites to evaluate what is working and what isn't. The results of this research along with requirements of the milestone project form the base of all the features included.

Websites and travel agents visisted for research:

* [CruiseNation](https://www.cruisenation.com/)
* [THG Holidays](https://www.thgholidays.co.uk/)
* [TUI](https://www.tui.co.uk/)
* [Loveholidays](https://www.loveholidays.com/)
* [On the beach holidays](https://www.onthebeach.co.uk/)
* [LuxuryEscapes](https://luxuryescapes.com/gb)

### Target Audience

Generally the target audience for an online agency are people with no specific plans/destination in mind yet but looking to explore. It includes individuals as well as groups looking for help to organise the travel plans. 
Get2Go holidays is thought to be an independent agency/agents and based on the research conducted best targetting couples with out of ordinary itineraries such as multi-destnation breaks and bucketlist destinations.

### User Stories

* User story 1:
    - As a customer at a fantasising/planning stage of a Holiday:

        1. I am looking for inspiration of where to go
        2. I am looking for a peace of mind about holiday security/reliability
        3. I want to see feedback from previous customers to have a better idea what to expect.
        4. I want to see a range of prices so I can make an informed decision before I progress further.

* User story 2:
    - As a customer ready to pick a package/book a Holiday:

        1. I am looking for a good selection of destinations with guide prices
        2. I am looking to be able to submit my specific requests and get my quotes.
        3. I want to see options to get in touch should I wish to progress or my requirements have changed.

### Scope

Viabaility Chart: Insert table here ( viability vs importance )

### Structure and Design

* Layout: The general layout of the site created using bootstrap and breaks into 3 section. A header, a footer and a main section on each page. The header and footer is designed to be straight forward with logo and navigation while the footer is to present a number of alternative way to see the agency through social links and include action button and "other" informtion such as terms and conditions. Both header and footer are the same throughout the site to ensure consistency.

* Features:

    * Header: The header contains a company logo , a call to action button and the main navigation bar.

        * Logo : responsive image of the logo of the company.
        * Contact : call to action implemented with clickable phone number.
        * Navbar : Main navigation feature of the whole site allowing users to easily move around as desired.

    * Footer: Main feature in this section is the clicable social media icons providing an alternative way to see and contact the company. The footer also home for a terms and conditions link( pop up widow with details) and a button to download brochure.

    * Main Page: index.html - present an overall look of the site, showcasing a hero image with eye catching holiday pictures and call to action buttons( see deals), which also provide an alternative way( other than nav bar) to navigate to the holidays.html page. The main page also includes a section of reviews and reasosns to book with us. 
        * Carousel: a slideshow of the main holiday categories, catch users attention quickly.
        * Testimonials: a display of feedback from previous customers.
        * Why book with us: a selection of feature the company offers for peace of mind.

    * Deals Page: presents main holiday categories for user such as multi-destination or bucket-list holidays with large clickable pictures/icons that navigates the user to the second section of the page where all actual deals are avaialble. All deals containers include a see deal button that has a pop-up window with the holiday details.

    * Enquiry Page: The enquiry page's main section have a form , where users can submit holiday requests/questions based on prefered dates, destination and budget. Upon submitting a form a thank you landing page is presented with navigation to return to main site.
    
    * Landing Page: A thank you page letting customers knnow that their enquiry form had been successfully submitted.
 
    * Download Brochure: clickable link to download a brochure with all existing deals. The feature presented in multiple location, namely once in the navigation bar and once in the footer area.

* Design Choices:

    * Color: I chose vibrant summer colors to implement a "good feel" vibe when visiting the page, the approach for these choices were guided by the original website(no longer exist, was provided by franchise at the time) colors and logo.

    *  #b10303, rgba(255,0,0,0.2), rgba(255,0,0,0.4), #c5b720, #faf6f6ce



    * Font: I choose the font family Open sans with san sarif as a fall back font.

* Interaction Design:

work flow graph/ image added here

* Wireframes:

Wireframes below were the original design, however the final product do feature some minor difference as alternative solutions were choosen and additional features implemented during development.

<details><summary>Home</summary>
<img src="assets/images/index.html.png">
</details>

<details><summary>Destinations</summary>
<img src="assets/images/deals.html.png">
</details>

<details><summary>Enquiry</summary>
<img src="assets/images/enquiry.html.png">
</details>

<details><summary>Landing Page</summary>
<img src="assets/images/Landing PAge.png">
</details>



## Testing/Bugs/Fixes

1. Responsive layout issue: sections are overlaying when testing small devices.
    - Solution: sections where given specific heights in px when initial code was written, changed width and height to %. This has solved the issue with the site responsivness.

2. The header appeared to have an unintentional over reach on the side of the nav bar area:
    - Solution: Investigated issue with the help of Developer Tools and found that I missed the bootstrap container in the header section "container-fluid", added it on to each page and this had fixed the issue.
<details><summary> Picture of issue:</summary>
<img src="assets/images/bug.jpg">
</details> 

3. Hamburger icon and toggle not working: Original implementation used bootstrap provided code to create hamburger icon toggle feature. This had later been scrapped as the course dos not require javascript to be used and found this was not justifyable to solve within the given time frame.
    - Issue was not resolved and alternate solution was emplemented.

4. During testing another issue appeared with the responsiveness of the header. Namely the navigation bar and call us section did not respond accurately to smaller screen sizes and some of the content went off screen.
    - Solution: I used media query to reduce the size of the navbar, hide the download brochure element so the rest of the navigation fits nicely. Furthermore, I changed the breakpoint I used in the main structure with bootstrap so the call us section hides earlier.
    The above have solved the issue!

5. Logo image non responsive and partialy covered on smaller screen sizes:
    - Solution: Changed the way the logo was originally implemented in css and used html <img> element instead. Set the parent container max-width t0 100% and the image to max-width:100% and height auto to enure it is fully responsive.
    The above has solved the issue.

6. Bootstrap Carousel not working:
    - The carousel created from bootstrap provided code was not working on the HOME page. The issue was fixed with the help of CodeInstitute tutor support, I found that the 4.2 version of hte CDN links added to the project needed replacing.
        - Solution: 4.6.2 version CDN links were added and that had fixed the issue.

## Media

Below are the links to all images used for the brochure and throughout the website.

* Pixabay: https://pixabay.com/images/search/webpage/

 * https://pixabay.com/photos/barbados-word-text-handwriting-70753/
 * https://pixabay.com/photos/indonesia-bali-ulun-danu-1578647/
 * https://pixabay.com/photos/eiffel-tower-paris-france-3349075/  
 * https://pixabay.com/photos/tiber-bridge-rome-bridge-italy-2263361/
 * https://pixabay.com/photos/church-santorini-d-greece-island-2020258/
 * https://pixabay.com/photos/mykonos-santorini-paros-greece-7317855/
 * https://pixabay.com/photos/bridge-manhattan-brooklyn-new-york-370542/
 * https://pixabay.com/photos/peru-mountains-machu-picchu-2135770/
 * https://pixabay.com/photos/hollywood-united-states-los-angeles-573444/
 * https://pixabay.com/photos/seychelles-indian-ocean-vacations-215253/
 * https://pixabay.com/photos/sydney-opera-house-sydney-354375/
 * https://pixabay.com/photos/beach-resort-jetty-pier-boardwalk-666122
 * https://pixabay.com/photos/beach-ocean-waves-coast-shore-5531919/

## Credits

* w3schools.com:
    * Flip Card: Code used from w3school.com website and changed to suit the needs of Get2Go Holidays destination page.
        * HTML: 

                <!--

                <div class="flip-card">
                 <div class="flip-card-inner">
                     <div class="flip-card-front">
                       <img src="img_avatar.png" alt="Avatar" style="width:300px;height:300px;">
                     </div>
                     <div class="flip-card-back">
                          <h1>John Doe</h1>
                          <p>Architect & Engineer</p>
                          <p>We love that guy</p>
                     </div>
                 </div>
                </div>

                -->

        * CSS:  

                /* The flip card container - set the width and height to whatever you want. We have added the border property to demonstrate that the flip itself goes out of the box on hover (remove perspective if you don't want the 3D effect */
                .flip-card {
                background-color: transparent;
                width: 300px;
                height: 200px;
                border: 1px solid #f1f1f1;
                perspective: 1000px; /* Remove this if you don't want the 3D effect */
                }

                /* This container is needed to position the front and back side */
                .flip-card-inner {
                position: relative;
                width: 100%;
                height: 100%;
                text-align: center;
                transition: transform 0.8s;
                transform-style: preserve-3d;
                }

                /* Do an horizontal flip when you move the mouse over the flip box container */
                .flip-card:hover .flip-card-inner {
                transform: rotateY(180deg);
                }

                /* Position the front and back side */
                .flip-card-front, .flip-card-back {
                position: absolute;
                width: 100%;
                height: 100%;
                -webkit-backface-visibility: hidden; /* Safari */
                backface-visibility: hidden;
                }

                /* Style the front side (fallback if image is missing) */
                .flip-card-front {
                background-color: #bbb;
                color: black;
                }

                /* Style the back side */
                .flip-card-back {
                background-color: dodgerblue;
                color: white;
                transform: rotateY(180deg);
                }
        
    * Bootstrap: Navbar
        * The originally taken navbar below was edited heavily with the toggle feature taken out.

                <nav class="navbar navbar-expand-lg navbar-light bg-light">
                    <a class="navbar-brand" href="#">Navbar</a>
                    <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
                        <span class="navbar-toggler-icon"></span>
                    </button>
                    <div class="collapse navbar-collapse" id="navbarNav">
                        <ul class="navbar-nav">
                        <li class="nav-item active">
                            <a class="nav-link" href="#">Home <span class="sr-only">(current)</span></a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#">Features</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#">Pricing</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link disabled">Disabled</a>
                        </li>
                        </ul>
                    </div>
                 </nav> 

    * Bootstrap: Carousel
        * 
            
                <div id="carouselExampleIndicators" class="carousel slide" data-ride="carousel">
                <ol class="carousel-indicators">
                    <li data-target="#carouselExampleIndicators" data-slide-to="0" class="active"></li>
                    <li data-target="#carouselExampleIndicators" data-slide-to="1"></li>
                    <li data-target="#carouselExampleIndicators" data-slide-to="2"></li>
                </ol>
                <div class="carousel-inner">
                    <div class="carousel-item active">
                    <img src="..." class="d-block w-100" alt="...">
                    </div>
                    <div class="carousel-item">
                    <img src="..." class="d-block w-100" alt="...">
                    </div>
                    <div class="carousel-item">
                    <img src="..." class="d-block w-100" alt="...">
                    </div>
                </div>
                <button class="carousel-control-prev" type="button" data-target="#carouselExampleIndicators" data-slide="prev">
                    <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                    <span class="sr-only">Previous</span>
                </button>
                <button class="carousel-control-next" type="button" data-target="#carouselExampleIndicators" data-slide="next">
                    <span class="carousel-control-next-icon" aria-hidden="true"></span>
                    <span class="sr-only">Next</span>
                </button>
                </div>
            