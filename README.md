# Grade10Letters
## Setting Up
### Main Content
- Download the [poole](https://github.com/poole/poole) code as a `.zip` file. Unzip the file, and open the folder in your default code editor.
- Open the `_cofig.yml` and replace all it's contents with the following:

```yml
# Setup
title: Jai Relan's End of Year Letters
tagline: Grade 10 ; 2020-21
url: https://jairelan.github.io/Grade10Letters.RAW/
paginate: 1
baseurl: ""
permalink: pretty

# Gems
plugins:
  - jekyll-gist
  - jekyll-paginate
  - jekyll-seo-tag

# Optimize Jekyll
exclude:
  - .editorconfig
  - .git
  - .jekyll-cache
  - Gemfile
  - Gemfile.lock
  - LICENSE.md
  - README.md

sass:
  sass_dir: _sass
  style: :compressed

# Options

# Replace this value and uncomment to enable Google Analytics tracking
# ga_analytics: UA-000000-0

# Specify the author for blog posts
author:
  name: Jai Relan
  url: https://jairelan.github.io/
  email: jairelan.2005@gmail.com

# Custom vars
version: 3.0.0
```

- Go to the the `_posts` folder and delete all the posts that are there.
- Create a new file naming it `2021-01-01-personname.md` (the date does not matter as it will be hidden in the html page. Be sure to replace `personname` with the name of the person. 
- In the file, paste the following:
```
---
layout: default
title: Introduction
---
```
- Open a terminal window in the parent directory and run `bundle exec jekyll serve`. Now open a browser and open `http://127.0.0.1:4000/`



### Encryption
- Open a terminal window and run `npm install -g staticrypt`
- 


### Using It



## Resources Used
- The Template for the index.html for the root parent directory was taken from [here](https://github.com/wildbit/postmark-templates). Only copy the .html file, ignore the .txt file there.
- Download [poole](https://github.com/poole/poole) locally on your computer. Go to the `_posts` folder and duplicated the template the number of times it is required. Use `bundle exec jekyll serve` to start the server and go to `http://127.0.0.1:4000/` on your browser and then navigate to the page which is required. After that, press `Command + S` to save it as an html file (Complete HTML, Multiple files). 
- The files were encrypted by [Staticrypt](https://github.com/robinmoisson/staticrypt). To do this, first install staticrypt by `npm install -g staticrypt`. Once you've down that, navigate to the subdirectory where the person's letter is (make sure the letter is called `raw_letter.html`), and then run the following command `staticrypt raw_letter.html **password**`. Rename the file to `index.html` and put `index.html` and the folder containing the css in this directory. 
An alternative I've considered for the passwords is [pagecrypt](https://github.com/MaxLaumeister/PageCrypt), however, I decided against it as it didn't have a CLI. 

FOR THE TIME BEING, THE INDEX.HTML IN THE JAIRELAN FOLDER HAS THE PASSWORD `password`