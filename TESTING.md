# FACTOR FITNESS  -  Testing

![The Factor Fitness Website shown on a variety of screen sizes](documentation/factor_fitness_mockup.png)

Visit the deployed site: [FACTOR FITNESS](https://factorfitness.herokuapp.com/)

- - -

## CONTENTS

* [AUTOMATED TESTING](#AUTOMATED-TESTING)
    * [W3C Validator](#W3C-Validator)
    * [JavaScript Validator](#JavaScript-Validator)
    * [Python Validator](#Python-Validator)
    * [Lighthouse](#Lighthouse)
    * [WAVE Testing](#WAVE-Testing)
* [MANUAL TESTING](#MANUAL-TESTING)
    * [Testing User Stories](#Testing-User-Stories)
    * [Full Testing](#Full-Testing)
* [BUGS](#Bugs) 

Testing was ongoing throughout the build. I utilised Chrome developer tools whilst building to pinpoint and troubleshoot any issues as I went along.

I used the console in the developer tools to work through sections of code and ensure that it was working correctly, and also troubleshoot where needed.

I have gone through each page using google chrome developer tools to ensure that each page is responsive on a variety of different screen sizes and devices.

---

## AUTOMATED TESTING

### W3C Validator

[W3C](https://validator.w3.org/) was used to validate the HTML on all the site pages. It was also used to validate the CSS file.

* index.html 
* base.html 
* main-nav.html 
* mobile-top-header.html 
* profile.html  
* add_product.html  
* edit_product.html 
* products.html  
* product_detail.html
* bag.html 
* checkout.html
* checkout_success.html

  * HTML:
  To validate the HTML code of the project I did this by pasting code in by direct input method. The W3C Validator for HTML gives errors and warnings for templating syntax used throughout the site so these errors were ignored. All other issues were resolved. 

  * CSS: 
  No issues found on static CSS files. 

---

### JavaScript Validator

[JSHint](https://jshint.com/) was used to validate the JavaScript.
I used the jshint extension I had installed into my Visual Studio Code IDE to check throughout the build. 

Two warnings given for semicolon use and two warnings for template literal syntax use. 

---

### Python Validator 

[PEP8 Online](http://pep8online.com/) was used to validate all Python files

[Flake8](https://marketplace.visualstudio.com/items?itemName=ms-python.flake8) extension for VSCode IDE was used throughout the build.

Due to limited time for completing the project, unfortunately I was unable to finish fixing all PEP8 errors that were shown. 

I need to spend more time on this and fix where lines are too long for pep8 standards. 

---

### Lighthouse

Google Lighthouse within the Chrome Developer Tools was used to test for performance, accessibility, best practices and SEO.

Most performance issues related to the bootstrap library and also image formats. 

In the future I would like to spend more time on this to see how the performance could be improved. Immediate areas to focus on are using file formats such as WebP, improving cache settings and fixing render blocking resources. 

### Desktop Results

Results for desktop.

![Factor Fitness desktop results](documentation/screenshot_lighthouse_desktop.png)

### Mobile Results

Results for mobile. 

![Factor Fitness mobile results](documentation/screenshot_lighthouse_mobile.png)

---

### WAVE Testing 

[WAVE](http://wave.webaim.org/) (Web Accessibility Evaluation Tool) This tool allows developers to create websites that are more accessible to users with disabilities.

I have used the WAVE testing tool to try and ensure there are no accessibility issues with the site.

The report came back with the following warnings: 

Warning giving for contrast usage of the green logo text on the white background. 
In future I would like to have used a border or some other feature around the logo section. 

Warnings given for usage of buttons with no text details such as for the search bar. As I have used placeholder text in the input field I have decided to ignore this warning. 

Warning given for not using a form 'label' tag. I would like to spend further time on this to create an appropriate label as I have not given forms labels in the past. 

---

## MANUAL TESTING

### Testing User Stories

`First Time Visitor Goals`
| Goals | How are they achieved? |
| --- | --- |
|  |
| I want the site to be clear so that I immediately know what the site is intended for upon entering. | When a visitor first arrives on the homepage they greeted immediately with a banner explaining what the store is and what it sells, along with a bold call to action button.| 
| I want to be able to easily find and purchase products. | The main products nav bar is fixed to the top of the screen for desktop with categories and sub categories in the dropdown menus for the products that are available.| 
| I want the e-commerce store to work well on all kinds of devices like mobile phones, tablets and desktops. | Bootstrap has been used on all the template pages to ensure a fully responsive design that can be viewed on all screen sizes.|
| I want to easily navigate the site by using the navigation menu. | The nav bar is clear and easy to understand on the desktop version. The same nav bar content is used on the mobile version but with the use of dropdown menus so that it can fit on the screen. |
| I want an easy way to search and sort products that are relevant to me. | The store search bar is bold and centre at the top of the main nav bar with placeholder text. |
| I want to be able to securely purchase a product with feedback of where I am in the process and the current status of that purchase. | The card input section is clearly defined on the checkout page. A loading spinner is displayed after submitting your card details and is being checked with the Stripe API. A success or failure message is displayed after communication with Stripe API. |
| I want the site to be visually appealing and easy to read. | I have tried to keep the colours and layout as minimal and clean as possible. With whites and blacks and just highlights of green throughout. This is to give the impression of a modern fitness gym feel. |
| I want to be able to register as a returning user to save my details for future orders. | Users are invited to sign up. Upon signing up users are then able to access the profile section where they can save address details for future orders. |
| I want to be able to get in contact via social media so that I can follow and contact the team. | Social media links are available on the footer section of every page that opens in a new browser tab. With more time I would have liked to add a dedicated contact page section. |
| I want to be able to add a product to the shopping bag and view the total value of the order. | Via the products details pages a user is able to add to their shopping bag, then click on the shopping bag icon at any time to see the full total amount. |
| I want to view product details and images so I can see the product closer up and in more detail. | Via the product details page a user can click on the image and a larger version of the image will open in a new tab. |
| I want to be able to update and delete products in the shopping bag to be in full control of the purchase. | Users are able to ‘update’ quantities or ‘remove’ items from the shopping bag on the shopping bag section. |
| I want to view my order details to be able to confirm everything before final purchase. | On the checkout page the user is able to see a summary of all the order details and the total final price they will be charged. |
| I want a clear indication of how to pay as well as an easy and secure method to pay for products with my card details. | I have kept the form section at the checkout stage as simple as possible to keep it intuitive for the user. With more time I would have liked to add more details regarding Stripe with perhaps a Stripe logo at the checkout stage. This is to give the user comfort that it is being processed by a well known payment processor. |
| I want to receive appropriate feedback of the order success or failure to ensure the purchase has gone through. | The user is shown a success or failure message after the card details have been processed and communication is complete with the Stripe API. |
#

`Returning Visitor Goals`
| Goals | How are they achieved? |
| --- | --- |
|  |
| To be able to log back into the site with my created username, email and password. | Users are able to create log in details on the sign up section. Users can then come back to the site and log in with these saved details.|
| To view my profile page to see my order history. | After a user has logged in they can see their previous orders via the profile page section. |
| To be able to log in and view, edit, add, delete my personal info. | Via the profile page section a user is able to update the delivery address they would like to use. With more time I would have liked to add more features to this section, such as the ability to change a users password and username/email. |
#

`Frequent Visitor Goals`
| Goals | How are they achieved? |
| --- | --- |
|  |
| When clicking on social media links I want the page to open in a separate browser tab. | Links for the social media sites are set up so that they open in a new browser tab. | 
| I want to be able to easily and quickly see any new products or offers. | By clicking on the offers link on the nav bar users are able to see all latest offers or via the dropdown menu access any new products. | 
#

`Superuser / Admin User Goals`
| Goals | How are they achieved? |
| --- | --- |
|  |
| I want to be able to view, search, edit and delete products. | Once a superuser/admin is logged in they have all functionality as a normal user and can search for all products they would like to view. Via the products pages a superuser/admin can edit or delete the products by clicking on the displayed buttons. | 
| I want to be able to log into the product management section so I can add products to the database. | After a superuser/admin has logged in they can access the product management section via the nav bar by clicking on the account section. From here they can add new products as well as add product images. | 
#

---

### Full Testing

Full testing was performed on the following devices:

* Laptop:
  * Macbook Pro 2020 13 inch screen
  * Macbook Pro 2020 with external 27 inch monitor
* Mobile Devices:
  * iPhone 7 plus.
  * iPhone 6.

Each device tested the site using the following browsers:

* Google Chrome
* Safari
* Firefox

Additional testing was done by friends and family on a variety of devices with the following feedback: 

* On mobile devices the checkout page section is too squashed with not enough room to update quantities to the shopping bag easily. 
* Unable to see the logo on mobile view at top nav bar. Feedback was to add the logo for mobile device view.
* Add more products to the store and have more sections on the product details page such as technical details and specifications. 
* Be able to change password on the profile section. 
* Have a contact page and an 'about us' page. 
* Text is too small on nav bar banner that explains shipping cost is free on orders over $40. 
#

`Home Page`
| Feature | Expected Outcome | Testing Performed | Result | Pass/Fail |
| --- | --- | --- | --- | --- |
|  |  |  |  |  |
| Shop Now Button | When clicked the user will be redirected to the all products page.| Clicked button. | Redirected to the products page showing all products. | Pass |
#

`Sign Up Page`
| Feature | Expected Outcome | Testing Performed | Result | Pass/Fail |
| --- | --- | --- | --- | --- |
|  |  |  |  |  |
| New user details input | New user is able to input a new user details including username, email and password.| Input a new user details using temp-mail email address and click on sign up button. | I am redirected to the 'verify email' instruction page and I receive my confirmation email. | Pass |
#

`Verify Your Email Page`
| Feature | Expected Outcome | Testing Performed | Result | Pass/Fail |
| --- | --- | --- | --- | --- |
|  |  |  |  |  |
| See the 'Verify your email address' and confirmation email | User is redirected to 'Verify Your email' page after signing up and receives confirmation email.| Do a new user sign up test and complete details on sign up page. | I am redirected to the 'Verify your email' page and I see the confirmation email in my inbox. | Pass |
#

`Confirm Your Email Address Page`
| Feature | Expected Outcome | Testing Performed | Result | Pass/Fail |
| --- | --- | --- | --- | --- |
|  |  |  |  |  |
| See the confirm email address page along with 'Confirm' button to click. | After opening the confirmation URL that was sent to my email address I will see the confirm email address page along with the 'Confirm' final button to press.| Open the URL in the Factor Fitness confirmation email in a new browser tab. | I am redirected to the 'Confirm Email' page and I see the 'Confirm' button to press. | Pass |
#

`Login Page`
| Feature | Expected Outcome | Testing Performed | Result | Pass/Fail |
| --- | --- | --- | --- | --- |
|  |  |  |  |  |
| Log into the website via the 'Sign In' page with my registered details. | After inputting my log in details I will be logged into the website. | Enter my confirmed registered details into the input fields. | Redirected to home page and I am logged into the site | Pass |
#

`Profile Page`
| Feature | Expected Outcome | Testing Performed | Result | Pass/Fail |
| --- | --- | --- | --- | --- |
|  |  |  |  |  |
| Able to add my shipping address details and save them. | Input my shipping address details in the form and save them. I am then able to come back to them in my profile and see they are saved. | New shipping address details entered into the form and clicked 'Update Information'. | After inputting shipping details and clicking 'Update Information' I went to other parts of the website and came back to the profile section and could see my details had been saved. | Pass |
#

`Products Page`
| Feature | Expected Outcome | Testing Performed | Result | Pass/Fail |
| --- | --- | --- | --- | --- |
|  |  |  |  |  |
| View products and am able to filter them using the nav bar menus. | The user sees all the products they wish to see by using the nav bar buttons and dropdown menus.| I clicked on the 'All Products' page and then chose other options in the nav bar by categories to confirm I saw a filtered view of products. | All products were filtered as per the dropdown menu items in the nav bar. | Pass |
#

`Product Details Page`
| Feature | Expected Outcome | Testing Performed | Result | Pass/Fail |
| --- | --- | --- | --- | --- |
|  |  |  |  |  |
| Adjust quantity I would like to order. | User is able to adjust quantity they would like to purchase by clicking on the plus and minus icons. | I clicked on the plus and minus icons on the product details page to confirm the quantity would change. | Quantity amount changed as per my clicks on the plus and minus icons. | Pass |
| 'Add to bag' Button. | When clicked the user will have the amount ordered added to the shopping bag ready for checkout. | Clicked button. | I can see the grand total amount on the shopping bag icon has increased as per my order and I can see a toast message alert saying 'Success' and a summery of the order details. | Pass |
#

`Shopping Bag Page`
| Feature | Expected Outcome | Testing Performed | Result | Pass/Fail |
| --- | --- | --- | --- | --- |
|  |  |  |  |  |
| Adjust quantity of ordered items or delete them | User is able to adjust the quantity of each ordered item or delete it completely. | I adjusted the quantity of the amount of one item by clicking the plus icon and then clicking 'Update'. I deleted another from the shopping bag by clicking 'Remove'. | One item quantity amount was adjusted and the other item was deleted from my shopping bag. | Pass |
| Proceed to secure checkout | When clicked the user will be redirected to the secure checkout page showing the items in the shopping bag.| Clicked button. | Redirected to the checkout page seeing items from shopping bag. | Pass |
#

`Checkout Page`
| Feature | Expected Outcome | Testing Performed | Result | Pass/Fail |
| --- | --- | --- | --- | --- |
|  |  |  |  |  |
| Enter my full details including shipping details | User is able to input all relevant details including shipping details so it is stored on the form. Note that the shipping address details would have already been input if saved in the profile section. | Input all data required into the input fields of the form. | All input fields completed and populated with my user details. | Pass |
| Enter card details for payment | User is able to input card details and then have it be checked by the connected Stripe API. | Input Stripe testing card data '4242 4242 4242 4242'. Then clicked on 'Complete Order'. | Loading spinner icon with green background appears confirming that it is connecting with Stripe and waiting for result. | Pass |
#

`Checkout Success Page`
| Feature | Expected Outcome | Testing Performed | Result | Pass/Fail |
| --- | --- | --- | --- | --- |
|  |  |  |  |  |
| Payment success confirming page with summary and confirmation email | User is given a 'Thank you' message for your order along with a toast alert confirming success. You also see a summary of the complete order and will get a confirmation email.| Input all card details on previous screen and waited for spinning icon to complete. | I see a 'Thank you' message along with a summary of the order. I also see the success toast alert and the confirming email in my inbox. | Pass |
#

`Add a Product Page`
| Feature | Expected Outcome | Testing Performed | Result | Pass/Fail |
| --- | --- | --- | --- | --- |
|  |  |  |  |  |
| Superuser / Admin is able to add products to the site | By going to the product management section the superuser can then add a new product via a form and add an image also.| Click on 'Product Management' from the account nav bar item. Enter a new product details in the form input fields. Upload an image. Then click on 'Add Product'. | When I go to the products section I can now see the product that I added. | Pass |
#

`Edit a Product Page`
| Feature | Expected Outcome | Testing Performed | Result | Pass/Fail |
| --- | --- | --- | --- | --- |
|  |  |  |  |  |
| Superuser can edit an existing product | Superuser is able to edit a products details.| I go to the products page and click on the 'Edit' button next to the product I wish to edit. I then am redirected to the 'Edit Product' page and I can adjust any details on that page. I then click 'Update Product'. | I can see the changes that I have made to that product when I now view it along side all the other products on the site. | Pass |
#

`Product Edit and Delete Sections`
| Feature | Expected Outcome | Testing Performed | Result | Pass/Fail |
| --- | --- | --- | --- | --- |
|  |  |  |  |  |
| Superuser can edit or delete products. | Superuser is able to access the edit section or delete a product via the products page. | Go to products pages and check to see I see the edit or delete buttons. I click on a test product I have just added to confirm it will be deleted. | Clicking the 'Edit' button takes me to the edit product section and the 'Delete' button deleted the test product I wish to delete. | Pass |
#

`Log Out Confirmation Page`
| Feature | Expected Outcome | Testing Performed | Result | Pass/Fail |
| --- | --- | --- | --- | --- |
|  |  |  |  |  |
| I can log out 'sign out' and confirm this. | User is able to log out of the site and on the final sign out page they will have to confirm first. | I sign out of the site and then click on the 'Sign Out' button to confirm this. | I am signed out of the website. | Pass |
#

`Base Template Sections`
| Feature | Expected Outcome | Testing Performed | Result | Pass/Fail |
| --- | --- | --- | --- | --- |
|  |  |  |  |  |
| Factor Fitness Logo Link | When clicked the user will be redirected to the home page.| Clicked link. | Redirected to the home page. | Pass |
| Nav Bar Links and dropdown menus | When clicked the user will be redirected to the related page or dropdown menu appears.| Clicked links. | Redirected to the correct related page or menu expanded. | Pass |
| Site wide search bar | When a term is entered into the search bar and then the search icon clicked the related products to that term will be shown.| Searched for the word 'yoga'. | Yoga related products were shown. | Pass |
| Footer Logo Link | When clicked the user will be redirected to the home page.| Clicked link. | Redirected to the home page. | Pass |
| Footer Social Media Links | When clicked a new tab will be opened in the browser for the related social media website.| Clicked links. | New tab opens for social media website in browser. | Pass |
#

---

## BUGS

### Solved Bugs
| No | Bug | How I solved the issue |
| --- | --- | --- |
|  |  |
| 1 | Top section of products page not visible on mobile view. | Fixed spacing and padding to top of that section in css file. |
| 2 | Unable to open the live site due to run server error during development. | Investigated and discovered it was an issue related to Bootstrap, the views and urls files not set up correctly causing issues with connection. |
| 3 | The shopping bag icon was showing up as a different colour on mobile view to desktop view.| I fixed by using my own custom colours in the final version instead of bootstrap colours. |
| 4 | Unable to link products json file to django database, unable to read. | Remade the json for the products checking on jsonformatter tool, fixed syntax errors. |
| 5 | Product filter section not working or filtering products correctly. | This was a section I was trying to build that was seperate from the nav bar and allowed the user to filter by ascending price, alphabet etc. I could not get the layout of it to work and so it was not fixed, I decided to delete that section altogether for now to save time. |
| 6 | Unable to connect to checkout page. | Issue with connection to Stripe and secret key set up, resolved when updated Heroku settings for secret key. |
#

### Known Unresolved Bugs

* At checkout it does not save your name for future orders, only the address part is saved. 

* Logo on nav bar for mobile view not showing. I should have made the nav bar layout so the logo is still visible. 

* On the 'confirm your email' page the footer section doesn't stick to bottom of the screen view. 

* Footer section doesn't fit full width of desktop screen view on profile page, needs to be fixed to fill entire screen width. 

* The responding email address of factor.fitness for the confirmation emails that get sent out has not been set up. Responses currently will go to a dead address. 

* Footer not fixed to bottom of screen view on sign out page. 

* Page load times are too slow, waiting for Stripe connection. With more time I would like to look into further to fix and improve load speeds. 

* No defensive programming set up when a superuser deletes a product, at least a modal should be set up to confirm deletion. 

* Layout of shopping bag page is too squashed for mobile view, buttons are too small. I would like to have fixed this and found a better solution for the layout. 

#