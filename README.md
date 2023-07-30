# Code Refactor Starter Code

Live Deployment Link: https://mjjust31.github.io/Code.Refactor

Based on the feedback I received, I believe my deployment link did not contain the most recent changes - particularly to the CSS file. To rectify this, I made a new repo with the latest changes along with addressing any feedback. 

User Story: 

AS A marketing agency
I WANT a codebase that follows accessibility standards
SO THAT our own site is optimized for search engines


Acceptance Criteria

GIVEN a webpage meets accessibility standards
WHEN I view the source code
THEN I find semantic HTML elements
WHEN I view the structure of the HTML elements
THEN I find that the elements follow a logical structure independent of styling and positioning
WHEN I view the image elements
THEN I find accessible alt attributes
WHEN I view the heading attributes
THEN they fall in sequential order
WHEN I view the title element
THEN I find a concise, descriptive title

Step 1: Review the HTML file to make more accessible and add semantic HTML. 

Step 2: Review CSS Code to determine duplicates to make code more efficient. 

In the HTML, there were many "divs" that could be changed to make it easier to read and accessible. I sorted the HTML in the following way: header, main, aside, and footer to make it easier to visualize the page without needing to. I also divided the content in sections to visualize the "break" on the page.  I also added a title and alt to the images. 

In the CSS code, there were many items that held the same design features that would be condensed for more efficient code. As I review, I attempted to keep items in order when reviewing the html. For example, keeping the header near the top of the CSS and moved classes lower if they appeared lower on the page.

Some of the same similarities were and were consolidated for more efficient code. 
/* 
.benefit-lead {
  margin-bottom: 32px;
  color: #ffffff;
}

.benefit-brand {
  margin-bottom: 32px;
  color: #ffffff;
}

.benefit-cost {
  margin-bottom: 32px;
  color: #ffffff;
} */

.aside-section h3 {
  margin-bottom: 10px;
  text-align: center;
}
/* 
.benefit-lead h3 {
  margin-bottom: 10px;
  text-align: center;
}

.benefit-brand h3 {
  margin-bottom: 10px;
  text-align: center;
}

.benefit-cost h3 {
  margin-bottom: 10px;
  text-align: center;
} */

.aside-section img {
  display: block;
  margin: 10px auto;
  max-width: 150px;
}
/* 
.benefit-lead img {
  display: block;
  margin: 10px auto;
  max-width: 150px;
}

.benefit-brand img {
  display: block;
  margin: 10px auto;
  max-width: 150px;
}

.benefit-cost img {
  display: block;
  margin: 10px auto;
  max-width: 150px;
} */

/* .search-engine-optimization {
  margin-bottom: 20px;
  padding: 50px;
  height: 300px;
  font-family: "Gill Sans", "Gill Sans MT", Calibri, "Trebuchet MS", sans-serif;
  background-color: #0072bb;
  color: #ffffff;
} */

/* 
.online-reputation-management {
  margin-bottom: 20px;
  padding: 50px;
  height: 300px;
  font-family: "Gill Sans", "Gill Sans MT", Calibri, "Trebuchet MS", sans-serif;
  background-color: #0072bb;
  color: #ffffff;
} */
/* 
.social-media-marketing {
  margin-bottom: 20px;
  padding: 50px;
  height: 300px;
  font-family: "Gill Sans", "Gill Sans MT", Calibri, "Trebuchet MS", sans-serif;
  background-color: #0072bb;
  color: #ffffff;
} */

/* .box-media img {
  max-height: 200px;
}

.box-media img {
  max-height: 200px;
} */

/* 
.online-reputation-management h2 {
  margin-bottom: 20px;
  font-size: 36px;
}

.social-media-marketing h2 {
  margin-bottom: 20px;
  font-size: 36px;
} */


I also noticed that all text (except for the footer) had the font color of #ffffff. Therefore, I applied this universally to the page and added a special CSS code for the footer - which had black font applied. 