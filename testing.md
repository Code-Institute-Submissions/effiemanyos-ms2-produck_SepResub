# **Content** 

- [Testing](#testing "Testing")
  - [HTML, CSS, JAVASCRIPT Validation Testing](#html-css-validation-testing "HTML, CSS, JAVASCRIPT Validation Testing")
  - [Testing Performance](#testing-performance "Testing Performance")
  - [Testing Accessibility](#testing-accessibility "Testing Accessibility")
  - [Testing User Stories](#testing-user-stories "Testing User Stories")

  [Return to README.md Document](https://github.com/effiemanyos/ms2-produck/blob/master/README.md)

# **TESTING**

![the webpage on different devices](assets/images/mockup-img.png "the webpage on different devices")

The website was tested in the following **browsers**:

- Chrome √
- Firefox √
- Microsoft Edge √
- Safari √
- Internet Explorer X
- Opera √

It was also tested in the following phone **operating systems**:

- iOS √
- Android √

Finally, it was tested in the following **devices**:

- Desktop √
- iPhone 5/SE √
- Pixel 2/2XL √
- Moto 4G √
- Galaxy S5 √
- iPhone 6/7/8 (+Plus) √
- iPhone X/iPhone XS Max √
- iPad/iPad Pro √
- Surface Duo √

*Results:* 

The website had an great performance and could be used perfectly, no funcional issues were found during the testing. However, the layout was not exactly the same (or the intended design) in all systems and devices but the users could interact with ease and achieve their goals successfully.

## **HTML, CSS, JAVASCRIPT Validation Testing**
-----

### **1. HTML Validation**

The tool used for this code validation was the [W3C Markup Validation Service](https://validator.w3.org/), which was used by **URL** to make sure there were no errors in none of the **HTML Files**. The results were the following:

![w3c html validation service one error results](assets/images/html-initial-validation.png "w3c css validation service one error results") 

***Date:*** Monday, May 10th, 2021

**1. Issue:** The element `a` must not appear as a descendant of the `button` element.

- **Fixes:** Remove the `a` inside the button `button` element like the example bellow:

*Before:*
```HTML
<li class="nav-item" data-toggle="collapse" data-target=".navbar-collapse.show">
    <div class="dropdown menu-dropdown">
        <button class="dropbtn page-scroll menu-dropbtn active"><a class="nav-link" href="index.html"><i
                    class="fa fa-home"></i> Home</a></button>
        <div class="dropdown-content menu-dropdown-content">
            <a href="index.html#about">> About Produck</a>
            <a href="index.html#services">> Our Services</a>
            <a href="index.html#contact">> Contact Us</a>
            <a href="index.html#footer">> Favourite Links</a>
        </div>
    </div>
</li>
```

*After:*
```HTML
<li class="nav-item" data-toggle="collapse" data-target=".navbar-collapse.show">
    <div class="dropdown menu-dropdown">
        <button class="dropbtn page-scroll menu-dropbtn nav-link active"><i class="fa fa-home"></i> Home</button>
        <div class="dropdown-content menu-dropdown-content">
            <a href="index.html#about">> About Produck</a>
            <a href="index.html#services">> Our Services</a>
            <a href="index.html#contact">> Contact Us</a>
            <a href="index.html#footer">> Favourite Links</a>
        </div>
    </div>
</li>
```

**2. Issue:** Stray end tag `i`.

- **Fixes:** Remove the `</i>` element from the code as it is no longer in use to finally get the following:

```HTML
<h4>Hey There!</h4>
```

**3. Issue:** Duplicate ID `contactForm`.

- **Fixes:** Replace the `id` name of the newsletter form from the footer to the following:

```HTML
<form onsubmit="return sendEmail(this);" id="newsletterForm"></form>
```

**4. Issue:** The `type` attribute is unnecessary for JavaScript resources.

- **Fixes:** Remove the `type` attribute (~~type="text/javascript"~~) from all of the following:

```HTML
<script type="text/javascript" src="assets/js/filename.js"></script>
```

The **final report** would have shown no errors in the html files as these would have been properly fixed as indicated above. However, due to a lack of time, the changes won't be implemented before the project deadline.


### **2. CSS Validation**

The tool used for this code validation was the [W3C CSS Validation Service](https://jigsaw.w3.org/css-validator/), which was used by **URL** to make sure that there were no errors in the **CSS Style Sheet**. The results were the following:

![w3c css validation service no error results](assets/images/css-initial-validation.png "w3c css validation service no error results") 

***Date:*** Monday, May 10th, 2021

The CSS yielded no major errors, so I proceeded with further testing after fixing the first two issues (the `transition-delay` and `box-sizing` values).

Just in case, the testing was performed again, this time by **File Upload** and **Direct Input**, and the results were exactly the same. 

### **3. JAVASCRIPT Validation**

The tool used for this code validation was the [JS Hint V2.12.0](https://jshint.com/), which was used by **Direct Input** of all the js files in this project to make sure there were no errors in none of the **JavaScript Files**. The results were the following:

**bookmarks.js**

![JS Hint JavaScript validation initial results](assets/images/bookmarks-validation.png "JS Hint JavaScript validation initial results") 

***Date:*** Tuesday, May 11th, 2021

**booknotes.js**

![JS Hint JavaScript validation initial results](assets/images/booknotes-validation.png "JS Hint JavaScript validation initial results") 

***Date:*** Tuesday, May 11th, 2021

**resources.js**

![JS Hint JavaScript validation initial results](assets/images/resources-validation.png "JS Hint JavaScript validation initial results") 

***Date:*** Tuesday, May 11th, 2021

**sendemail.js**

![JS Hint JavaScript validation initial results](assets/images/sendemail-validation.png "JS Hint JavaScript validation initial results") 

***Date:*** Tuesday, May 11th, 2021

**sendnewsl.js**

![JS Hint JavaScript validation initial results](assets/images/sendnewsl-validation.png "JS Hint JavaScript validation initial results") 

***Date:*** Tuesday, May 11th, 2021

**tobuylist.js**

![JS Hint JavaScript validation initial results](assets/images/tobuylist-validation.png "JS Hint JavaScript validation initial results") 

***Date:*** Tuesday, May 11th, 2021

**toreadlist.js**

![JS Hint JavaScript validation initial results](assets/images/toreadlist-validation.png "JS Hint JavaScript validation initial results") 

***Date:*** Tuesday, May 11th, 2021

## **Testing Performance**
-----

In order to test the website's performance on **desktop** and **mobile**, [Google Lighthouse](https://developers.google.com/web/tools/lighthouse) was used in both cases.

### **Desktop & Mobile**

The **initial results** were the following:

![google lighthouse results](assets/images/lighthouse-p1.png "google lighthouse results") 

![google lighthouse results](assets/images/lighthouse-p2.png "google lighthouse results") 

![google lighthouse accessibility results](assets/images/lighthouse-p3.png "google lighthouse accessibility results") 

![google lighthouse best practices results](assets/images/lighthouse-p4.png "google lighthouse best practices results") 

![google lighthouse runtime settings](assets/images/lighthouse-p5.png "google lighthouse runtime settings") 

***Date:*** Friday, May 14th, 2021

[Back to Content](#content)

## **Testing Accessibility**
-----

To test the website accessibility [Wave Web Accessibility Evaluation Tool](https://wave.webaim.org/) was used. The obtained results are the following:

![wave accessibility results](assets/images/wave-accessibility-results.png "wave accessibility results") 

***Date:*** Saturday, May 15th, 2021

[Back to Content](#content)

## **Testing User Stories**
-----

*Crucial User Stories to Test MVP & Validate Hypothesis:*

1. As an **Entrepreneur/Solopreneur**, I want to **register** to Effie's **online workshops** so that I can boost my business' monthly sales.
    > Feature that will be implemented in the next iteration (Training Page: Online Workshops).
2. As a **Tech Startup**, I want to **use** Effie's **free online resources** so that we can create a robust Digital Marketing strategy.
    > Feature that will be implemented in the next iteration (Resources Page: Free Resources).
3. As a **SME**, I want to **book** a **free consultaiton** with Effie so that we can increase our business' online presence and engagement.
    > Feature that will be implemented in the next iteration (Contact Me Page: Calendly Integration).
4. As a **Non-Profit**, I want to **contact** Effie for a **collaboration** and **consulting session** so that we can grow the organization organically.
    > Users can contact Effie through the following: Navigation Bar (Contact), About Me Section (CTA Button), How Can I Help Section (CTA Button), What I Do (CTA Button), Get In Touch Section (Contact Information & Form).
5. As a **Mentee**, I want to **apply** to Effie's **mentorship program** so that I can get the proper guidance to build my professional career.
    > Feature that will be implemented in the next iteration (Services Page: Mentorship Program Applycation).

[Back to Content](#content)

[Return to README.md Document](https://github.com/effiemanyos/ms2-produck/blob/master/README.md)