# Mission to Mars

## Overview of Project
> Robin's web app is looking good and functioning well, but she wants to add more polish to it. She had been admiring images of Mars’s hemispheres online and realized that the site is scraping-friendly. She would like to adjust the current web app to include all four of the hemisphere images. To do this, you’ll use BeautifulSoup and Splinter to scrape full-resolution images of Mars’s hemispheres and the titles of those images, store the scraped data on a Mongo database, use a web application to display the data, and alter the design of the web app to accommodate these images. 

1. ***Deliverable 1***: Scrape Full-Resolution Mars Hemisphere Images and Titles
2. ***Deliverable 2***: Update the Web App with Mars Hemisphere Images and Titles
3. ***Deliverable 3***: Add Bootstrap 3 Components
4. ***Extra***: A written report on the employee database analysis [`README.md`](https://github.com/emmanuelmartinezs/Mission-to-Mars). 

## Resources and Before Start Notes:

* Data Source: `Mission_to_Mars.ipynb`, `app.py`, `scraping.py` and `index.html`
* Data Tools: Jupyter Notebook, Python and MongoDB
* Software: MongoDB, Python 3.8.3, Visual Studio Code 1.50.0, Flask Version 1.0.2

For more information, read the [`Documentation on MongoDB and other data typess`](https://docs.mongodb.com/). 

## HTML Keys
Tables in HTML are basically made up of many smaller containers. The main container is the `<table />` tag. Inside the table is `<tbody />`, which is the body of the table—the headers, columns, and rows.

`<tr />` is the tag for each table row. Within that tag, the table data is stored in `<td />` tags. This is where the columns are established.


![name-of-you-image](https://github.com/emmanuelmartinezs/Mission-to-Mars/blob/main/Resources/Images/s1.JPG?raw=true)




## Deliverable 1:  Scrape Full-Resolution Mars Hemisphere Images and Titles
### Deliverable Requirements:
Using BeautifulSoup and Splinter, you’ll scrape full-resolution images of Mars’s hemispheres and the titles of those images.

1. Make a copy of your `Mission_to_Mars.ipynb` file, and rename it `Mission_to_Mars_Challenge.ipynb`. 
2. Download the `Mission_to_Mars_Challenge_starter_code.ipynb`, copy the starter code, and paste at the end of your `Mission_to_Mars_Challenge.ipynb` file.
3. ​In Step 1, use your browser to visit the [`Mars Hemispheres`](https://astrogeology.usgs.gov/search/results?q=hemisphere+enhanced&k1=target&v1=Mars) website to view the hemisphere images.
4. Use the DevTools to inspect the page for the proper elements to scrape. You will need to retrieve the full-resolution image for each of Mars's hemispheres.

 
### Results with detail analysis:

1. **Make a copy of your `Mission_to_Mars.ipynb` file, and rename it `Mission_to_Mars_Challenge.ipynb`.**

> Image with `Python`, `MongoDB` & `HTML` Code below.

**Code and Image**


````python
# Mission to Mars (Module Code)
# by Emmanuel Martinez

# Import Splinter and BeautifulSoup
import pandas as pd
from splinter import Browser
from bs4 import BeautifulSoup as soup
from webdriver_manager.chrome import ChromeDriverManager
````

![name-of-you-image](https://github.com/emmanuelmartinezs/Mission-to-Mars/blob/main/Resources/Images/1.1.JPG?raw=true)

![name-of-you-image](https://github.com/emmanuelmartinezs/Mission-to-Mars/blob/main/Resources/Images/1.1.1.JPG?raw=true)

2. **Download the `Mission_to_Mars_Challenge_starter_code.ipynb`, copy the starter code, and paste at the end of your `Mission_to_Mars_Challenge.ipynb` file.**

> Image with `Python`, `MongoDB` & `HTML` Code below.

**Code and Image**


````python
# Here start the Mission to Mars Challenge Starter Code
# by Emmanuel Martinez

# Import Splinter, BeautifulSoup, and Pandas
from splinter import Browser
from bs4 import BeautifulSoup as soup
import pandas as pd
````

![name-of-you-image](https://github.com/emmanuelmartinezs/Mission-to-Mars/blob/main/Resources/Images/1.2.JPG?raw=true)

![name-of-you-image](https://github.com/emmanuelmartinezs/Mission-to-Mars/blob/main/Resources/Images/1.2.1.JPG?raw=true)

3. ​**In Step 1, use your browser to visit the [`Mars Hemispheres`](https://astrogeology.usgs.gov/search/results?q=hemisphere+enhanced&k1=target&v1=Mars) website to view the hemisphere images.**

> Image with `Python`, `MongoDB` & `HTML` Code below.

**Code and Image**


````python
from flask import Flask, render_template
from flask_pymongo import PyMongo
import scraping

app = Flask(__name__)
````

![name-of-you-image](https://github.com/emmanuelmartinezs/Mission-to-Mars/blob/main/Resources/Images/1.3.JPG?raw=true)

4. **Use the DevTools to inspect the page for the proper elements to scrape. You will need to retrieve the full-resolution image for each of Mars's hemispheres.**

> Image with `Python`, `MongoDB` & `HTML` Code below.

**Code and Image**


````python
from flask import Flask, render_template
from flask_pymongo import PyMongo
import scraping

app = Flask(__name__)
````

![name-of-you-image](https://github.com/emmanuelmartinezs/Mission-to-Mars/blob/main/Resources/Images/1.4.JPG?raw=true)



## Deliverable 2: Update the Web App with Mars’s Hemisphere Images and Titles
### Deliverable Requirements:
Using your Python and HTML skills, you’ll add the code you created in Deliverable 1 to your `scraping.py` file, update your Mongo database, and modify your `index.html` file so the webpage contains all the information you collected in this module as well as the full-resolution image and title for each hemisphere image

1. The `scraping.py` file contains code that retrieves the full-resolution image URL and title for each hemisphere image. 
2. The Mongo database is updated to contain the full-resolution image URL and title for each hemisphere image.
3. ​The index.html file contains code that will display the full-resolution image URL and title for each hemisphere image.
4. After the scraping has been completed, the web app contains all the information from this module and the full-resolution images and titles for the four hemisphere images.

 
### Results with detail analysis:

1. **The `scraping.py` file contains code that retrieves the full-resolution image URL and title for each hemisphere image.**

> Image with `Python`, `MongoDB` & `HTML` Code below.

**Code and Image**


````python
from flask import Flask, render_template
from flask_pymongo import PyMongo
import scraping

app = Flask(__name__)
````

![name-of-you-image](https://github.com/emmanuelmartinezs/Mission-to-Mars/blob/main/Resources/Images/2.1.JPG?raw=true)

2. **The Mongo database is updated to contain the full-resolution image URL and title for each hemisphere image.**

> Image with `Python`, `MongoDB` & `HTML` Code below.

**Code and Image**


````python
from flask import Flask, render_template
from flask_pymongo import PyMongo
import scraping

app = Flask(__name__)
````

![name-of-you-image](https://github.com/emmanuelmartinezs/Mission-to-Mars/blob/main/Resources/Images/2.2.JPG?raw=true)

3. ​**The index.html file contains code that will display the full-resolution image URL and title for each hemisphere image.**

> Image with `Python`, `MongoDB` & `HTML` Code below.

**Code and Image**


````python
from flask import Flask, render_template
from flask_pymongo import PyMongo
import scraping

app = Flask(__name__)
````

![name-of-you-image](https://github.com/emmanuelmartinezs/Mission-to-Mars/blob/main/Resources/Images/2.3.JPG?raw=true)

4. **After the scraping has been completed, the web app contains all the information from this module and the full-resolution images and titles for the four hemisphere images.**

> Image with `Python`, `MongoDB` & `HTML` Code below.

**Code and Image**


````python
from flask import Flask, render_template
from flask_pymongo import PyMongo
import scraping

app = Flask(__name__)
````

![name-of-you-image](https://github.com/emmanuelmartinezs/Mission-to-Mars/blob/main/Resources/Images/2.4.JPG?raw=true)



## Deliverable 3: Add Bootstrap 3 Components
### Deliverable Requirements:
For this part of the Challenge, update your web app to make it mobile-responsive, and add two additional Bootstrap 3 components to make it stand out.

1. The webpage is mobile-responsive. 
2. Two additional Bootstrap 3 components are used to style the webpage.

 
### Results with detail analysis:

1. **The webpage is mobile-responsive.**

> Image with `Python`, `MongoDB` & `HTML` Code below.

**Code and Image**


````python
from flask import Flask, render_template
from flask_pymongo import PyMongo
import scraping

app = Flask(__name__)
````

![name-of-you-image](https://github.com/emmanuelmartinezs/Mission-to-Mars/blob/main/Resources/Images/3.1.JPG?raw=true)
    
    
2. **Two additional Bootstrap 3 components are used to style the webpage.**

> Image with `Python`, `MongoDB` & `HTML` Code below.

**Code and Image**


````python
from flask import Flask, render_template
from flask_pymongo import PyMongo
import scraping

app = Flask(__name__)
````

![name-of-you-image](https://github.com/emmanuelmartinezs/Mission-to-Mars/blob/main/Resources/Images/3.2.JPG?raw=true)


#### # Mission to Mars Analysis Completed by Emmanuel Martinez
