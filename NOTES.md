## Week 8, Friday
On a phone, the information in specific catogories were more indented.  I fixed it by redcing the left padding to .5 in li.

## Week 9, Wednesday
1. What are your three pages, and why those three?

The three pages are Home, Projects, and Contact, so the user can not only learn information about me but contact me if neccessary.

2. You changed one thing in styles.css and all three pages changed.
What would you have had to do if each page carried its own copy?

If each page carried its own copy, each copy would have to be altered respectively to their corresponding page.

3. What is one thing on your page you don't know how to change yet?

One thing I dont know how to change yet is the addition of animated visuals or features within it 

# Week 9, Friday
1. What width did you pick for your breakpoint, and how did you choose it?

I chose 40 rem as everything seemed to fit perfectly within the page using the measurment.

2. The two things you found and fixed at phone width.

I did not find anything that necessarily needed to be fixed. Everything fit perfectly.

3. In your own words: what is the difference between justify-content
and align-items? 

The command align-items moves items vertically while justify-content moves them horizontally.

4. Why does the plain rule hold the narrow layout and the media query
hold the wide one, instead of the other way round?

The plain rule handles small screens by default, and the media query adjusts the layout for a wider more complex designs.

## Week 10, Wednesday
1. In your own words: what is the difference between HTML, CSS and
JavaScript? One sentence each.

HTML is the base setup for your ui. CSS is to change aspects or elements of the ui in more detail. Javascript is to add  features and functionality to your ui.

2. What does `defer` do on the script tag, and what breaks without it?

`defer` tells the browser to dowload the JavaScript while reading HTML without its execution until the HTML is read. without it themeButton would be null.

3. Dark mode changed your whole site with five lines of CSS. Why did that work? What would you have had to do without variables? 

It worked because the five lines called all the recolored elements needed to change the page. Without the variables you would have to change each of the base colors set.

4. Something went wrong this week and the Console said nothing at all. What was it, and how did you eventually find it?

One thing that went wrong was the dark mode not functioning when pressed, I later solved this by debugging my code and found it had been a syntactical mistake as I had missed hashtags in certain spots.

5. What is one thing on your page you don't know how to change yet?

I dont know how to make my image more dynamic or add dynamic features within my pages in general.

## Week 10, Friday
1. What does event.preventDefault() do, and what happens without it?

event.preventDefault() stops the browser from performing its default action for an event. Without it the page would reset.

2. You got "Cannot read properties of null" in class. In your own
words, why did it happen, and why did if fix it?

The error happened because JavaScript was trying to access an HTML element that it couldn't find. The if fixed it as if checks whether the element exists before trying to use it.

3. What rule did you write for your form, and why that rule?

For my rule chose to give errors if messages a less than 10 characters and that messages couldnt only be special characters so messages could be more coherent and not random while also being a reasonable length.

4. The two things you found and fixed at phone width.

I did not find anything that really needed to be fixed and felt content with how the phone width behaved.

5. Your form does not actually send anything anywhere yet. What do
you think is missing? 

I think that the website is missing a method of sending the users responses to the developer in some way, whehther it be through messages or email, the developer should be notified.

## Week 11, Wednesday
Live site: https://anthonyosorio.netlify.app
1. In your own words: what does GitHub do, and what does Netlify do?

Git hub holds the code for your project or website, while Netfily hosts the code and displays it to the public.

2. You are about to merge into development and your live site will
   not change. Why?

The branch Netlify takes which is the release branch has not been changed only the development.

3. What does the padlock in the address bar actually mean?

The padlock icon in the browser's address bar indicates that the connection to the website is using HTTPS,


4. Your repository is public and now your site is too. Is there
anything in your repo you would not hand a stranger?

Something in my repository I would most likely not give to a stranger are the screen shots i've taken.


## Week 11, Friday
1. Your form has a hidden field nobody can see. Explain what it is
for, and why it works better than asking people to prove they
are human.

The field is a honeypot which users dont have access to but spam bots usually end up filling, marking those messages as spam. This is better than asking people to prove they're human as it removes an obstacle or steps that delay the process of sending the message, making it a smoother process.

2. What is a Deploy Preview, and when would you actually use one?

Deploy preview is a private viewable version of your build, that gives you the oppurtunity to verify it to see whether it is functioning how you expect.

3. The two things you found and fixed on a real phone.

I added the go back buttons to tabs that did not have it, and changed the header name of my form page to "Contact Form", as I already had a contact page that used "Contact" as a heading. functionality wise everything is working fine.

4. Describe the path a change takes from your laptop to the public,
naming every branch it passes through.

First your change happens in a sepereate branch that later gets merged into development, if the code is working as expected it will then get merged from development to the release branch where everything is finalized and the website changes are publically shown.

5. Your site now has two addresses, the netlify.app one and your
own domain. Why do both still work?

Netlify doesn't remove its original URL when you connect a custom domain. Instead, it allows multiple addresses to point to the exact same deployed website.

6. Your site is on the internet now. What is one thing you want to
add before the end of the semester?

One thing I would like to add is more movable ui elements like pictures, or tabs that slide in certain directions.

## Week 12, Wednesday, Lab 19
1. In your own words, what is stored in a database table?

A database table stores organized information in rows and columns.

2. What is the difference between a table and an API endpoint? 3. What does GET do? What format did your endpoint return?

A table is where information is stored in a database, while an API endpoint is a URL that allows an application to interact with that information, such as retrieving or updating records. GET is an HTTP request method used to retrieve information from a server without changing the stored data. My endpoint returned the information in JSON format, specifically as an array of objects.

4. Why do we use a publishable key, not a secret key?

We use a publishable key because it is designed to be used in client-side applications and is safe to expose publicly when proper security is used. A secret key provides elevated access and should stay private because exposing it could allow unauthorized people to access or modify database information.

5. What changed when select=* became select=title,category?

When we used select=*, the endpoint returned all available columns for each record. Changing it to select=title,category limited the response to only the title and category columns. This allows us to retrieve only the information we actually need.

## Week 12, Friday — Lab 20
1. What does fetch() send and what does response.json() return? 2. Why does the page use textContent instead of innerHTML?

fetch() sends an HTTP request to the Supabase API endpoint to retrieve database records. response.json() reads the response and converts the JSON data into a JavaScript object or array that the page can use. The page uses textContent as it displays text without interpreting it as HTML. This is safer because it helps prevent malicious code or HTML from being injected into the webpage.

3. What happens when Supabase returns an empty list?

The page receives an empty array, meaning there are no records to display.

4. How does the page behave when the network fails?

The request fails, and the error is caught by the error-handling code, which ends up displaying an error message instead of pretending the data loaded successfully.

5. What is the proof that a card is NOT hardcoded in HTML?

the proof is that the cards appear after the JavaScript fetches records from Supabase. The Network tab shows a successful HTTP 200 response, and the page displays five items, demonstrating that the cards are generated dynamically from database data.