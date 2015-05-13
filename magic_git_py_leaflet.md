layout: true
class: center, middle, inverse
---
#An intro to Git, Python, and Leaflet    
Eric Goddard  
Center for Applied Earth Science and Engineering Research
---
layout: false
class: left, middle
# Outline
- Git

--

    - What is it?
--

    - Why use it?
--

- Web mapping app with Python and Leaflet
---
class: center
#Git: What is it?
--

.left[##A distributed version control system]

--

.left[- Used to store:
    - code
    - data
    - Anything that is represented in a text file
        - can also store images, pdfs, word files, etc., but you don't get the line by line changes.
]
--

.left[- that allows:
    - many editors
    - tracking changes over the life of the file
    - rolling back changes
]
---
#Git: Why use it?
.left[
- Easier to keep track of files
- Easier to see how (and by whom) files have changed over time
    - Especially helpful if someone new joins the project and needs to get up to speed
]
---

background-image: url(./images/git_history.png)
---
#Git: Why use it?
.left[ 
- Easier to manage staffing transitions 
    - insurance 
    - no more directories with multiple versions of code
]
---
background-image: url(http://www.explainxkcd.com/wiki/images/0/0a/documents.png)
---
background-image: url(./images/bus.png)
---
#Tutorial
--

.left[
##The Plan
- Fetch the files from Github using the Git command line
    - Go over some of the most common git commands  
- use the Flask microframework to serve a Leaflet map that queries the Yelp API for
humanity's favorite beverage
]
---

.center[##[https://github.com/egoddard/magic_git_py_leaflet](https://github.com/egoddard/magic_git_py_leaflet)
![beer](http://egoddard.github.io/geospatial_colloquium/images/beer_prediction.jpg)]
