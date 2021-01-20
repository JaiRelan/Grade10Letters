# Grade10Letters
## Resources Used
- The Template for the index.html for the root parent directory was taken from [here](https://github.com/wildbit/postmark-templates). Only copy the .html file, ignore the .txt file there.
- Download [poole](https://github.com/poole/poole) locally on your computer. Go to the `_posts` folder and duplicated the template the number of times it is required. Use `bundle exec jekyll serve` to start the server and go to `http://127.0.0.1:4000/` on your browser and then navigate to the page which is required. After that, press `Command + S` to save it as an html file (Complete HTML, Single File). 
- The files were encrypted by [Staticrypt](https://github.com/robinmoisson/staticrypt). To do this, first install staticrypt by `npm install -g staticrypt`. Once you've down that, navigate to the subdirectory where the person's letter is (make sure the letter is called `raw_letter.html`), and then run the following command `staticrypt raw_letter.html **password**`. Rename the file to `index.html` and put it in this directory. 
An alternative I've considered for the passwords is [pagecrypt](https://github.com/MaxLaumeister/PageCrypt), however, I decided against it as it didn't have a CLI. 

FOR THE TIME BEING, THE INDEX.HTML IN THE JAIRELAN FOLDER HAS THE PASSWORD `password`