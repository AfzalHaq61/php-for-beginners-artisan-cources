# Video 1 (How to Choose a Programming Language)

How exactly do you choose a first programming to learn? Why PHP, and not Ruby? And what about JavaScript or Python? How can you possibly be expected to make an educated decision at this early stage of your learning?

you don't have to learn every language in real world. its depend on what language you need to learn. it's the same thing in programming languages so have to learn that langauge which you need the most.

when you learn one language the basic concept of all programming languages are the same then you can learn every language.

Laravel and wordpress === PHP
Shopify === Ruby

------------------------------------------------------------------------------------------------

# Video 2 (How to Choose a Programming Language)

Before we can dig in, we must first create the world, so to speak. To follow along with this series, you'll need to install a handful of essential tools. Let's go over them in this episode.

Here's a list of all tools I mentioned in the video.

- Environments
1. Homebrew *
(how to install: /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)")
(Install php: brew install php)
(Search php version in brew: brew search php)
(Install mysql: brew install mysql)
2. Laragon * (recomended for windows)
3. WSL
4. XAMPP
5. MAMP (for mac)
6. Docker (Advanced but neccesary)

- Code Editors
PHPStorm * (license can be found through university student account).
Sublime Text
Visual Studio Code

- Terminals
Warp * (simple, easy and auto complete options)
iTerm
Windows Terminal

- Database GUIs
Table Plus *
PHPMyAdmin

Remember, there's no wrong choice. Just pick the one that feels good to you. And if you're not sure what "feels" good, stick with the ones I recommend (note the stars above).

---------------------------------------------------------------------------------------------------

# Video 3 (Your First PHP Tag)

Our first order of business is to prepare some basic HTML, boot a PHP server, and view it in the browser.

http://localhost:8888

make index file in root folder and run this command your project will run on this port.

you can print a string by these ways in php.
<?php print "hello world" ?>
<?php echo "hello world" ?>

------------------------------------------------------------------------------------------------

# Video 4 (Variables)

Okay, let's move on and review basic concatenation and variables. The first time I learned about variables, my first thought was, "But why?". Let's talk about it!

diff between "" (double quotes) and '' (single quotes)

- write variables and string simultaneously.
<?php
    $greeting = "Hello";
    echo "$greeting Everybody!"
?>

- can't write variables and string simultaneously but you have to write varible without quotes and conacate them with .
<?php
    $greeting = "Hello";
    echo $greeting . ' ' .  'Everybody!'
?>

------------------------------------------------------------------------------------------------