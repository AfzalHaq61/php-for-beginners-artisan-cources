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

make index file in root folder and run this command your project will run on this port.
php -S localhost:8000 // command

http://localhost: //port running

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

# Video 5 (Conditionals and Booleans)

For this next episode, we'll build a quick webpage that displays a dynamic message based upon whether or not you've read a particular book. This will give us the opportunity to review both conditionals and booleans.

------------------------------------------------------------------------------------------------

# Video 6 (Arrays)

# At this point, you know how to create a variable for a primitive string or number. But what about situations when we want to declare a collection, or list of things? A list of usernames, or book titles, or tweets? In these situations, we can reach for arrays.

# In PHP, an array is a data structure that allows you to store multiple values in a single variable. Arrays in PHP can be of different types: numerically indexed, associative, or multidimensional. Here is an explanation and examples of each type:

# 1. Numerically Indexed Array
# A numerically indexed array uses numeric indices to access its values. The indices start from 0.

<?php
# Defining a numerically indexed array
$fruits = array("apple", "orange", "banana", "strawberry");

# Accessing an element of the array
echo $fruits[1]; // Prints "orange"
?>

# 2. Multidimensional Array
# A multidimensional array is an array that contains one or more arrays. It is useful for storing tabular data.

<?php
# Defining a multidimensional array
$products = array(
    "fruits" => array("apple", "orange", "banana"),
    "vegetables" => array("lettuce", "carrot", "broccoli")
);

# Accessing an element of the array
echo $products["fruits"][0]; // Prints "apple"
?>

# Creating an Array in PHP
# Arrays in PHP can be defined using the array() function or the [] syntax.

Using array()

<?php
# Numerically indexed array
$colors = array("red", "green", "blue");

Using []

<?php
# Numerically indexed array
$colors = ["red", "green", "blue"];

# Using foreach

<?php
$fruits = ["apple", "orange", "banana"];

# Looping through a numerically indexed array
foreach ($fruits as $fruit) {
    echo $fruit . "\n";
}

<!doctype html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Demo</title>
</head>
<body>
    <h1>Recommended Books</h1>

# our array
    <?php
        $books = [
            "Do Androids Dream of Electric Sheep",
            "The Langoliers",
            "Hail Mary"
        ];
    ?>

# one way which is concatenation
    <ul>
        <?php foreach ($books as $book)
            echo "<li>" . $book . "</li>"
        ?>
    </ul>

# second way is just write in Commas
    <ul>
        <?php foreach ($books as $book)
            echo "<li>$book</li>"
        ?>
    </ul>

# third way is write in one curly bracket
    <ul>
        <?php foreach ($books as $book)
            echo "<li>{$book}</li>"
        ?>
    </ul>

# fourth way: if html element are more then we can use this method html elemnts are without php 
    <ul>
        <?php foreach ($books as $book) : ?>
            <li><?php echo $book ?></li>
        <?php endforeach ?>
    </ul>

# we can use shorcut for <?= $book ?> instead of <?php echo $book ?>
    <ul>
        <?php foreach ($books as $book) : ?>
            <li><?= $book ?></li>
        <?php endforeach ?>
    </ul>

# we can use bracker insted of : and endforeach
    <ul>
        <?php foreach ($books as $book) {?>
            <li><?= $book ?></li>
        <?php } ?>
    </ul>

</body>
</html>

------------------------------------------------------------------------------------------------