# Testing 


## Code Validation 

### W3C HTML Validator

#### Home Page

![Home Page HTML Validation](documentation/testing/html-index.jpg)

#### Sheds Page

![Sheds Page HTML Validation](documentation/testing/html-sheds.jpg)

#### Workshops Page

![Workshops Page HTML Validation](documentation/testing/html-workshop.jpg)

#### Menu Page

![Menu Page HTML Validation](documentation/testing/html-menu.jpg)

#### Contact Page

![Contact Page HTML Validation](documentation/testing/html-contact.jpg)

#### Confirmation Page

![Confirmation Page HTML Validation](documentation/testing/html-confirmation.jpg)

### W3C CSS Validator 

![Site-Wide CSS Validation](documentation/testing/css-validation.jpg)

## Lighthouse 

![Lighthouse Check](documentation/testing/lighthouse-check.png)

The Lighthouse check has returned a sub-optimal performance. 

![Lighthouse Fails](documentation/testing/lighthouse-fails.jpg)

A number of these appear to be related to the use of Bootstrap and the Google Maps iframe element. This could be improved dramatically through changes to efficiency which, for the purposes of this project, I am unable to rectify at the time. 


## Responsiveness 

Responsive design tests were carried out using both physical devices and [Chrome Dev Tools](https://developer.chrome.com/docs/devtools/). 

### Physical Device Tests:

#### Samsung Galaxy s10

![S10 responsive check](documentation/testing/samsungs10.jpg)

#### Nokia 5.3

![Nokia responsive check](documentation/testing/nokia5-3.jpg)

#### Samsung Galaxy s21

![S21 responsive check](documentation/testing/ipad.jpg)

#### iPhone 12

![iPhone 12 responsive check](documentation/testing/iphone12.jpg)

### Chrome Dev Tools Tests:

#### iPad

![iPad responsive check](documentation/testing/ipad.jpg)

#### iPad Pro

![iPad Pro responsive check](documentation/testing/ipadpro.jpg)

#### iPhone X

![iPhone X responsive check](documentation/testing/iphonex.jpg)

#### iPhone SE

![iPhone SE responsive check](documentation/testing/iphonese.jpg)

The only device where I feel that the landing page is poorly optimised, however, the share of SE devices among iPhone users is approximately only 2.3%.

#### Samsung Galaxy s20 Ultra

![S20 Ultra responsive check](documentation/testing/s20ultra.jpg)


## A11y Color Contrast Accessibility Checker

![A11y Color Contrast Check](documentation/testing/contrast-check.jpg)


## Browser Compatibility

The site was tested on Google Chrome, Microsoft Edge, Safari and Mozilla Firefox, with no visible issues for the user. Appearance, functionality and responsiveness were consistent throughout for a range of device sizes and browsers, besides Safari, which seems to struggle with load times occasionally. 

## Testing User Stories 

* As a user I would like to ensure my favourite shed is available so that I can enjoy my visit more. 
    * The sheds page is easily accessible from home, giving immediate access to regular users and quick access to the booking page.  

    ![Shed Booking Button](documentation/testing/hero-image.jpg)
    ![SimplyBook Widget](documentation/testing/simplybook-modal.jpg)

* As a user I want to be able to enquire about upcoming workshops so that I can save time.
    * Navigation to the Workshops page is clear and the enquiry form is simple to find. 

    ![Workshops Main Body](documentation/testing/workshops-images.jpg)
    ![Workshops Modal](documentation/testing/workshop-modal.jpg)

* As a user I want to be able to contact the business so that I can enquire about dietry options. 
    * Navigation to the contact form is simple, the form itself is clear and concise and the user is notified that the message has been received. 

    ![Contact Page](documentation/testing/contact-form.jpg)
    ![Confirmation Page](documentation/testing/confirmation.jpg)

* As a user I want to be able to plan my trip for peace of mind. 
    * The home page includes a clear map which can be expanded to generate directions through Google. 

    ![Home Google Map](documentation/testing/google-map.jpg)
    ![Directions](documentation/testing/map-directions.jpg)

* As a user I want to be able to see what other customers think before deciding to visit. 
    * The home page includes reviews from customers and clear links to easily access Trip Advisor which containts additional reviews.

    ![Reviews](documentation/testing/reviews.jpg)

* As a user I want to be able to check what food and drink they offer before visiting. 
    * Navigation to the menu page is clear and simple, with the option to download a PDF copy for offline viewing. 

    ![Menu Page](documentation/testing/menu.jpg)

## Bugs

### Resolved

#### Background image sizing

During the building process, I had a recurring bug which caused issues with the background images. 

![Background sizing bug portrait](documentation/testing/background-height-issue.jpg)

![Background sizing bug landscape](documentation/testing/background-height-landscape.jpg)

In order to resolve this bug, I had to amend how the height was calculated in the CSS. For larger screen sizes, the height was calculated through the viewport height measurement. In order to fit correctly on smaller screens or when a device is in landscape, media queries had to be generated to measure the height in percentages rather than viewport height. 

#### Jumbotron overflow

During the building process, the home page's responsiveness collapsed when devices were approximately 350px wide or smaller. This caused the information contained within the Jumbotron to overflow into the container below. 

![Jumbotron overflow bug](documentation/testing/jumbotron-overflow.jpg)

This was resolved through ammending media queries to factor in much smaller screen sizes, reducing the total height which the jumbotron's content could occupy. 

### Unresolved

