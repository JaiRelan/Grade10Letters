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
- Open a terminal window in the parent directory and run `bundle exec jekyll serve`. Now open a browser and open `http://127.0.0.1:4000/`. 

### Encryption
- Open a terminal window and run `npm install -g staticrypt`

### Welcome Page
- Download the welcome page which I used from [here](https://github.com/wildbit/postmark-templates/blob/master/templates-inlined/plain/welcome/content.html) and rename it into `index.html`

### Using This Setup
- First, create a new repository in Github and open it clone it onto your computer. 
- Then customise the welcome page which we downloaded as `index.html`. Apart from line # 11, I didn’t feel the need to touch anything before line # 464. 
- Now, minimise this folder and go to the poole directory which you downloaded and edited. Go under the `_posts` folder and then duplicate the template you created as many times as needed. 
- Under the `layout` and `title` definitions, you can start typing whatever message you want to in each.
- Once you are done, save all the files and go to the browser tab with `http://127.0.0.1:4000/` open. One by one, go to the open the contents as required and press `Command + S` to save it. Save it as a complete HTML file (select the *Multiple files* option). 
- Now open a terminal window, navigate to this directory and use staticrypt as follows `staticrypt filename.html password`.
- Rename the output file as `index.html` and put this file and the companion css file in `/name/` directory. 
- Push the chances to Github and you’re good to go!

## File Structure
```
.
|- index.html #main page accessable at https://jairelan.github.io/Grade10Letters/
|- 404.html
|- 404.css #support file for 404.html
|- Personname #page accessable at https://jairelan.github.io/Grade10Letters/personname
	\- index.html #encrypted letter
	\- person.css #support css file
|- Personname #page accessable at https://jairelan.github.io/Grade10Letters/personname
	\- index.html #encrypted letter
	\- person.css #support css file
|- Personname #page accessable at https://jairelan.github.io/Grade10Letters/personname
	\- index.html #encrypted letter
	\- person.css #support css file
```


FOR THE TIME BEING, THE INDEX.HTML IN THE JAIRELAN FOLDER HAS THE PASSWORD `password`
