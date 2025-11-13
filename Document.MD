# 1.Project Documentation

> - Project Title:Responsive Portfolio Website
- Student Name: SHIBSANKAR BERA
- Course: HTML & CSS Web Development
- Submitted * To:INTERNSALA PGC
- Date of Submission:[10/11/2025]
> * Introduction

>The Responsive Portfolio Website project is a single-page web application created using HTML5 and CSS3. The objective   of this project is to design a personal portfolio site that highlights my skills, services, certifications, and contact information in an attractive and responsive layout. 
The website adapts smoothly to different screen sizes, including desktop, tablet, and mobile devices, through the use    of media queries. The design includes creative animations, transitions, and hover effects to provide a modern and interactive user experience

# 2.Project Objectives

* To design a visually appealing personal portfolio website using only HTML and CSS.
* To implement responsive design techniques ensuring compatibility with multiple devices.
* To organize information about personal skills, certifications, and projects.
* To use semantic HTML for better accessibility and structure.
* To apply CSS animations and transitions for interactive and engaging sections.
* Adding custom font family like lobster , momo  trust display

# 3. Tools and Technologies Used

* HTML5 – for semantic and structural layout

* CSS3 – for styling, responsiveness, and animations

* VS Code – as the primary code editor

* Google Chrome – for testing and debugging

* Media Queries – to handle responsive behavior

# 4. Project Structure
>   MYPORTFOLIO/
│
├── dist/
│   └── images/
│       ├── certificate/
│       ├── projects/
│       ├── profile.jpg
│       └── icons/
│
├── src/
│   ├── input.css
│   ├── media.css
│   └── index.html
│
└── Document.txt

* _Description_

  * index.html – Contains the main structure of the website.

  * input.css – Contains core styling such as colors, layout, and typography.

  * media.css – Manages responsive behavior across different devices.

  * images/ – Contains images used in certificates, projects, and profile sections.


# 5. Website Sections Overview
>## I.Header

 * Designed using a semantic `<header>` tag.
 Includes a logo, navigation links (Home, About, Skills, Services, Portfolio, Contact), and a day/night mode toggle for theme variation.
 * Fixed at the top for easy navigation (position: stikey).

## II.Home Section

* Contains an introductory heading and a short personal introduction.

* Displays a profile image with smooth animation effects.

* Includes social media icons (LinkedIn, GitHub, Instagram, Twitter).

* Features a “Download Resume” button with hover animation (downlod Enable).

## III.Skills Section

* Displays a section heading titled “My Skills”.

 * Skills are represented using linear progress bars to indicate proficiency levels in HTML, CSS, JavaScript, and React.

 * CSS animations are used to animate the filling of the bars when the section appears.

## IV.Certifications Section

* Displays at least three certification cards with the course name, platform, and year.

* Each card has a View Certificate button that directly links to the actual certificate file.

* The design includes shadows, rounded corners, and hover scaling effects.

## V.Projects Section

* Introduces the section with “My Recent Projects”.

* Displays six projects as interactive cards:

  * CGPA Calculator

  * Explore World Tourist

  * Solar Project Web

  * Restaurant Menu Layouts

  * Product Price Card

  * E-commerce Plants

Each card includes a screenshot, title, and description with hover animations and transitions.

## VI. Contact Section

* Contains a contact form with fields for Name, Email, and Message at left side.

* Includes a “Send Message” button with hover effects.

* Displays contact information such as phone number, email, and location on the right side.

## VII.Footer

Built using a semantic `<footer>` tag.

* Includes “Call Me” and “Email Me” buttons with color transitions and hover BLINK animations.

* Displays copyright:

* © 2025 [Your Name]. All Rights Reserved.

6. CSS Design and Responsiveness

The visual design was achieved using creative color combinations, gradient backgrounds, and consistent spacing. Transitions and hover effects are applied to buttons, cards, and images to enhance interactivity.

>Responsive Design

* The website is made responsive using CSS media queries for three primary device types:

  * Desktop / Laptop: Full-width layout with horizontal navigation and multi-column sections.

  * Tablet (iPad Mini): Adjusted grid layouts and text sizing for comfortable readability.

  * Mobile (Samsung Galaxy S8+): Collapsed navigation menu and vertically stacked content.

>Sample Media Query Example:

```css
 @media only screen and (max-width: 768px) {
  .nav-links {
    position: absolute;
    top: 100%;
    right: -40%;
    height: 60vh;
    width: 60%;
    background-color: transparent;
    backdrop-filter: blur(1.5rem);
    display: none;
  }

  .nav-links ul {
    flex-direction: column;
    align-items: center;
    justify-content: center;
    row-gap: 15px;
  }
 }
```
Animations such as transform, transition, and blur effects were used to create smooth movement and depth.

# 7. Testing and Validation

* Tested responsiveness on multiple devices using Chrome Developer Tools.
* Verified layout adjustments for desktop, tablet, and mobile screens. * Checked for accessibility compliance using semantic HTML tags.

* Ensured proper alignment, color contrast, and hover effects.

# 8. Conclusion

This project demonstrates a practical understanding of front-end web development concepts including semantic HTML, CSS styling, and responsive design.
The website serves as a personal portfolio to display projects, certifications, and contact details in a visually appealing and functional way.
Through this project, I have gained hands-on experience in:

Designing responsive layouts

Using CSS animations and transitions

Structuring HTML for better accessibility and readability

This portfolio can also serve as a foundation for future web development projects by integrating JavaScript and backend technologies.



> /\*     resopnsive nav bar only css             \*/

i have done a responsive nav bar where in big screen menues iterms are shown in horizontal
but in smaller screen they are become disappesrs and insted of this a menue icon appears
by click it ,we can show the menu items in vertical order
behind this ,
        Logic-1:cheklist=unchecked //list hide
        cheklist =checked //list shown
       Logic-2: 1.initialy both(menue and close) icon are hide ,
                2.then set meue icon visible (uncheked state)
                3.when cheklist is in unchecked =menue seen ,close hide
                4.checked=close seen,menue hide
