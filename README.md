# chajr 🪑

chajr (pronounced chair) is a simple bash script for getting **C**ss, **H**tml, **A**nd **J**avascript **R**eady.

---

## What chajr does 🛠

The script creates a directory in the working directory using the name passed into it as an argument. Inside this directory it creates 3 directories - `css` containing an empty `main.css` file, `js` containing an empty `main.js` file, and an empty `images` directory.  An `index.html` file with some basic HTML 5 boilerplate and links to `css/main.css` and `js/main.js` is also created.

    You, in your terminal:
    
    $ chajr MyFancyNewProject
    
    This script:
    
    📂<-- Current Working Directory
     \
      📁MyFancyNewProject (NEW!)
        \
        |
        |---📄index.html (NEW!) 
        |     (Includes HTML boilerplate and links to main.css and main.js)
        |
        |---📁css (NEW!)
        |    \
        |     📄main.css (NEW!)(Empty)
        |
        |---📁js (NEW!)
        |    \
        |     📄main.js (NEW!)(Empty)
        |
        |---📁images (NEW!)

---

## Installing 📲

1) In the terminal, navigate to the download location of chajr

2) `mv` [chajr](http://chajr.sh) into a `$PATH` directory.

2.1) Unsure of what your `$PATH` directories are? Run the `echo $PATH` command, or learn more [here](https://medium.com/@jalendport/what-exactly-is-your-shell-path-2f076f02deb4).

2.2) If the `/usr/local/bin` directory is among your `$PATH` directories, it is likely a suitable location for chajr. As long as you've followed step 1, you can run the below command to place it there.

    mv chajr /usr/local/bin

2.3) If you lack permission to write to write to directory, check if you have a `$PATH` in your home directory that you have write access to, and place chajr there. If you don't, [learn more about $PATH](https://medium.com/@jalendport/what-exactly-is-your-shell-path-2f076f02deb4) and set up your own.

---

## Running 🏃‍♀️🏃‍♂️

    chajr DirectoryName

Once installed, running chajr is really this simple! The directory name you give to chajr must not contain any spaces. 

---

## Details 🔍

### What HTML 5 Boilerplate are you putting into my index.html file?

    <!DOCTYPE html>
    <html lang="en">
    <head>
      <meta charset="UTF-8">
      <meta name="viewport" content="width=device-width, initial-scale=1.0">
      <meta http-equiv="X-UA-Compatible" content="ie=edge">
      <link rel="stylesheet" href="css/main.css"/>
      <script defer src="js/main.js"></script>
      <title>Title</title>
    </head>
    <body>
      
    </body>
    </html>

### Wow, why did you name your file x / why did you divide your files into directories like that / why did you defer JS execution? This is all terrible, this is truly unusable garbage!

You're welcome to modify or distribute any part of this script! Adapt it for yourself, or your organization and make it you own.

---

# Pull up a chajr, get to work