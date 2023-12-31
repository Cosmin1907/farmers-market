# Farmers Market

## Overview

Farmers Market is a website dedicated to connecting local farmers with nearby consumers, providing access to fresh and cost-effective agricultural products. The landing page highlights the positive impact of supporting local farmers on both the community and the economy. The website also features a contact form with an option for new farmers to express interest and join the platform. View the live site [here](https://cosmin1907.github.io/farmers-market/)

![Responsice Mockup](docs/media/mockup.PNG)

## User Stories

- **Local Food Enthusiast**

Loving the farmers market website's simple layout, I easily explore a list of vendors and connect directly with local farmers through the provided contact details.

- **Health-Conscious Shopper**

The clean design of the farmers market website guides me to organic vendors, and direct contact info lets me inquire about their products seamlessly.

- **Local Farmer**

The website's contact form has a fantastic feature for new farmers to register and showcase their products.
This approach fosters connections with the community, and helps to expand my customer base.

## Features

- **Navigation Bar**

  - The responsive navigation bar is featured on all pages, offering easy access to the landing page, market, and contact page.
  - This feature enables users to effortlessly move between pages on any device, eliminating the need to use the 'back' button to return to the previous page.

![Navigation Bar](docs/media/navbar.png)

- **The Footer**

  - The footer of the page features links to Farmers Market associated social media platforms, which open in new tabs for user-friendly navigation.

  - This section is beneficial for users, promoting connection and engagement through social media.

![Footer](docs/media/footer.png)

## Landing Page

- **Landing Page Image**

  - The landing page incorporates an image with overlaid text, providing users a direct view of the project's core values, which focus on enhancing both individual health and community well-being.

  - Together the image and the text convey the message that such exchanges contribute to individual well-being and enhance community health.

![Hero Image](docs/media/heroindex.png)

- **Values**

  - This section emphasizes the positive impact of local farmers on the community and economy, fostering awareness and appreciation for their vital role in shaping the local landscape.

  - Additionally, it encourages users to support and engage with local farmers through compelling content and messaging, aiming to motivate participation in activities that strengthen the bond between consumers and the agricultural community.

![Core Values](docs/media/values.png)

## Market Page

- **Main Purpose**

  - This page is designed to connect consumers with farmers, offering a direct line to the source of fresh produce and artisanal goods.
  - It features a thematic hero image of a cultivated field, emphasizing its focus on a farmers market.

![Market Hero Image](docs/media/heromarketsnip.PNG)

- **Main Features**

  - Farmers' contact phone numbers and addresses are prominently displayed, facilitating direct communication between consumers and producers.
  - The photos provide a snapshot of the diverse products available. Images and text seamlessly blend for an engaging browsing experience.

![Market Overview](docs/media/gallery.PNG)

## Contact Page

- **Main Purpose**

  - The contact page provides a convenient way for users to get in touch trough the contact form.

![Contact Form](docs/media/contactform.PNG)

- **Aditional Features**
  - A dedicated checkbox option has been implemented to reveal previously hidden fields, enabling new farmers to express interest and join the platform.
  - The additional fields require users to provide both direct contact information and detailed product descriptions.
  - Upon successful submission of the contact form, users will be directed to a dedicated thank-you page, confirming the successful submission and suggesting that our team will promptly review it.

![Contact Form revealed](docs/media/formrevealed.PNG)
![Thank you Page](docs/media/thankyou.PNG)

## Features Left to Implement

Create a JavaScript functionality that enables sending an email to the website owner when a new message is submitted through the contact form.

## Design

### Wireframes

Home Page

![Home Page](docs/media/homewire.PNG)

Market Page

![Market Page](docs/media/marketwire.PNG)

Contact page

![Contact page](docs/media/contactwire.PNG)

Thank You Page

![Thank you page](docs/media/tywire.PNG)

## Testing

### Responsivness

- **Testing Criteria**

Conducted testing on all pages for responsiveness across screen sizes from 320px upwards, following [WCAG 2.1 Reflow criteria for responsive design](https://www.w3.org/WAI/WCAG21/Understanding/reflow.html)
Utilized Chrome, Edge, Firefox browsers.

- **Steps to Test**

Opened the browser and navigated to [Farmers Market](https://cosmin1907.github.io/farmers-market/).
Opened developer tools and set to responsive mode.
Decreased width to 320px, set zoom to 50%, and clicked/dragged the responsive window to maximum width.
testede phone numbers

- **Expected**

Website should be responsive on all screen sizes.

1. No pixelation or stretching of images.
2. No horizontal scroll.
3. No overlapping elements.

- **Actual**

  - Issue: The website experienced an irregularity in presenting the row count when viewed on medium-sized screens.
  - Fix: Modified the media screen to achieve a smoother transition between different screen sizes.

Overall, the website demonstrated responsive behavior as intended

### Accessibility

[Wave Accessibility](https://wave.webaim.org/) tool was used throughout development and for final testing of the deployed website to check for any aid accessibility testing.

Testing was focused to ensure the following criteria were met:

- All forms have associated labels or aria-labels so that this is read out on a screen reader to users who tab to form inputs
- Color contrasts meet a minimum ratio as specified in [WCAG 2.1 Contrast Guidelines](https://www.w3.org/WAI/WCAG21/Understanding/contrast-minimum.html)
- Heading levels are not missed or skipped to ensure the importance of content is relayed correctly to the end user
- All content is contained within landmarks to ensure ease of use for assistive technology, allowing the user to navigate by page regions
- All not textual content had alternative text or titles so descriptions are read out to screen readers
- HTML page lang attribute has been set
- Aria properties have been implemented correctly
- WCAG 2.1 Coding best practices being followed

  - Issue: Error involving an empty form label, attributed to the concealed checkbox employed for toggling the navigation menu.
  - Fix: Applied ( .sr-only ) CSS technique to hide the specified element, resolving the hidden checkbox issue for navigation. Enhances accessibility with clear explanations for blind or low-vision users.

### Functional Testing

| Feature | Expected Outcome | Testing Performed | Result | Pass/Fail |
| ---------------------- | -------------------------------------------------------------------------------- | ---------------------------------------------- | ------------------------------------------------- | --------- |
| **Navbar** | | | | |
| Home  | Clicking will redirect the user to the home page.                      | Clicked Home | Redirected to the Home page.  | Pass  |
| Market       | Clicking will redirect the user to the market page.  | Clicked Market  | Redirected to the Market page.   | Pass |
| Contact | Clicking will redirect the user to the home page.                   | Clicked Contact | Redirected to the Contact page. | Pass      |
| **Footer**  | | | | |
| Social Icons-Facebook  | Clicking will open a new window, redirecting the user to the Facebook page.  | Clicked icon   | Redirected to the Facebook page in a new window.  | Pass  |
| Social Icons-Instagram | Clicking will open a new window, redirecting the user to the Instagram page. | Clicked icon   | Redirected to the Instagram page in a new window. | Pass  |
| Social Icons-X  | Clicking will open a new window, redirecting the user to the X page.| Clicked icon  | Redirected to the X page in a new window.   | Pass  |
| Social Icons-Youtube   | Clicking will open a new window, redirecting the user to the Youtube page.  | Clicked icon  | Redirected to the Youtube page in a new window.   | Pass |
| **Contact Form** | | | | |
| Contact form | If certain items were omitted, a message prompted the user to fill in the corresponding section. | Clicked submit while leaving the form unfilled | Form requested sections to be filled in. | Pass |
| Contact form | Typed everything in but email is in the wrong format | Clicked submit | Form requested the @ element to be included | Pass |
| Contact Form | Typed everything correct and should expect the form to submit | Clicked submit | Form submitted | Pass |
| Checkbox Interaction | Checked the box and tested if hidden fields appeared | Checked box  | Hidden fields appeared | Pass |

- **Navigation**

Confirmed all navigation links lead to the correct pages.
Verified links on all pages, ensuring expected navigation.

- **Forms**

Tested the contact form for various scenarios.
Correct inputs led to successful submission and redirection.
Detected and displayed appropriate error messages for missing or incorrect inputs.

- **Footer**

Validated Social Media Icons: Confirmed they open in new tabs.

In summary, comprehensive testing covered navigation, form functionality, and footer elements, ensuring a smooth user experience.

### Validator Testing

- HTML

  - No errors were returned when passing through the official [W3C validator](https://validator.w3.org)

  ![Home Validator Results](docs/media/indexvalidator.PNG)
  ![Market Validator Results](docs/media/marketvalidator.PNG)
  ![Contact Validator Results](docs/media/contactvalidator.PNG)

- CSS

  - No errors were found when passing through the official [(Jigsaw) validator](https://jigsaw.w3.org)

  ![CSS Validator Results](docs/media/cssvalidator.PNG)

### Lighthouse Testing

![Home Testing](docs/media/lighthousehome.PNG)
![Market Testing](docs/media/lighthousemarket.PNG)
![Contact testing](docs/media/lighthousecontact.PNG)

- **Additional Device Testing**

Aditional testing was performed on the following devices:

1. Ipad Pro
2. iPhone SE

- **Browsers**

I used for testing the following browsers:

1. Google Chrome
2. Mozilla Firefox
3. Microsoft Edge

### Unfixed Bugs

No major bugs were left unfixed. Any minor issues or limitations are detailed here:

Additional warnings were identified regarding labels connected to hidden content on the contact form. After investigating, I determined that this issue does not hinder functionality or accessibility, and therefore, no further action is required.

## Deployment

### Version Control

The site was created using Codeanywhere code editor and pushed to github to the repository ‘farmers-market’.

The following git commands were used throughout development to push code to the remote repo:

`git add <file>` - This command was used to add the file(s) to the staging area before they are committed.

`git commit -m “commit message”` - This command was used to commit changes to the local repository queue ready for the final step.

`git push` - This command was used to push all committed code to the repository on github.

### Deployment to Github Pages

- The site was deployed to GitHub pages. The steps to deploy are as follows:
  - In the GitHub repository, navigate to the Settings tab
  - From the menu on left select 'Pages'
  - From the Build and deployment section, Branch sub section drop-down menu, select: main Click 'Save'
  - A live link will be displayed when published successfully.

The live link can be found here - <https://cosmin1907.github.io/farmers-market/>

### Clone the Repository Code Locally

Navigate to the GitHub Repository you want to clone to use locally:

- Click on the code drop down button
- Click on HTTPS
- Copy the repository link to the clipboard
- Open your IDE of choice (git must be installed for the next steps)
- Type git clone copied-git-url into the IDE terminal

The project will now of been cloned on your local machine for use.

## Credits

I incorporated elements from the Love Running code for the navbar and header, customizing them to align with my vision for the farmers market site. Additionally, I integrated components from the gallery and meetup sections, combining them uniquely to create a new page.

I drew inspiration and incorporated additional code from:

[Medium Web accessibility](https://medium.com/web-accessibility-tips-tricks-and-techniques-for/web-accessibility-tip-visually-hidden-text-for-screen-readers-a52d954d9711#:~:text=sr%2Donly%20declaration%20block%20does,invisible%20to%20the%20human%20eye)

[Mmdn](https://developer.mozilla.org/)

[W3schools](https://www.w3schools.com/css/css3_flexbox_responsive.asp)

- **Media**

  - Images and visual elements sourced from Open Source repositories:

  - Icons from [Font Awesome](https://fontawesome.com/) were utilized not only in the footer but also in other sections such as the navigation bar and in various places throughout the website to enhance user experience and visual elements.

- **Content**
  - The content developed for this website includes mock details and names for farmers to ensure privacy. This approach allows effective demonstration of the website's features while respecting the confidentiality of real individuals.
