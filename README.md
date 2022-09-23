# Kickstart-Project
New Project Kickstart
For every new freelance website that I do, I've noticed a lot of redundancy. I finally got fed up with recreating the same files and folders over and over again. This repo solves that by having a ready-built template to start from.

It comes complete with my custom gulp file that automates the following tasks:

Autoprefixes CSS (up to the last 2 browser versions)
Minifies the CSS
Concatenates CSS
Compresses/optimized images
Minifies HTML
Concatenates JS
Minifies JS
Terminal Error Handling (any errors detected in CSS/JS will cause a tone and a notification in the terminal window)
LiveReload (see step 5 below)
Instructions
If node is not already installed on your machine, you can do so by by visiting https://nodejs.org/download/. The install process is quick. You can check to see that you already have node installed on your machine by typing npm -v in a terminal. If you see anything OTHER than a number (i.e. 1.4.28), then you need to install node.
Additionally, you can update node/npm by using the following commands:

sudo npm cache clean -f
sudo npm install -g n
sudo n stable
Next, install gulp globally by entering sudo npm install -g gulp in your terminal. Again, you can check to see that gulp is already installed on your machine by typing gulp -v.

LiveReload is also supported in the gulpfile. To get that running:

Install the 'LiveReload' extension (https://chrome.google.com/webstore/detail/livereload/jnihajbhpnppcggbcgedagnkighmdlei?hl=en)
Enable it through settings in Chrome
Check the box under the extension settings that says "Allow access to file URLs"
Restart Chrome <-- This is pretty crucial
Open build/index.html in your browser.
Click on the little icon in Chrome that looks like two arrows, with a small black circle in the middle. This will enable LiveReload on that specific page.
Once you're finished, type gulp in the terminal to begin the Gulp task.

In your favorite text editor (I prefer Sublime), make changes to the files in the src directory. Gulp will automatically watch these files, and rerun the various tasks if it detects any changes to the files. Chrome should automatically update to reflect the changes.

Happy coding!
