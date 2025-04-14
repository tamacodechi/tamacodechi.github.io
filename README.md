# tamacodechi.github.io

# Setup

Before starting, you can use an integrated terminal inside VSCode through the keyboard shortcut (Ctrl + Shift + `), or by clicking 'Terminal' -> 'New Terminal' on the top left taskbar menu

Make sure you have Ruby and NodeJS installed! You can see if they are available by running

    ruby -v
    node -v

Install all dependencies and gems by running

    bundle
    npm i

# Hosting your webpage

Start hosting the website by running

    bundle exec jekyll serve

The website can then be found at

    http://127.0.0.1:4000/

# Modifying the stylesheets

You can update the look of your page by

    A) Modifying the 'main.css' file
    B) Using 'TailwindCSS' classes (Recommended)
        This is achieved through the 'classes' attribute inside your HTML files
        i.e: <p class="text-xl">Hello world</p>

        More info at the documentation website on https://v3.tailwindcss.com/docs/container
        Where you can find all available classes on the list to the left, or by using the search bar on the top left.

# Adding new pages/routes

    1) Create a new 'markdown' file under the 'pages' folder
    2) Add the following content to it
        ---
        layout: sample
        title: Sample
        permalink: /sample/
        ---

       Where 'layout' is the HTML file that your new page will use, 'title' is what will appear as the Tab title on the browser and 'permalink' will be the URL to access it
    3) Add a new 'HTML' file inside the '_layouts' folder, with the same name you set in your 'markdown' file
