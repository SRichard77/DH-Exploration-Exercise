**Name:** Skylar Richard

**Date:** June 17 2022

#### Wget 

For the DH exploration exercise, I used Wget to pull Abbie Bright's 86 page diary from [Kansas Memory](https://www.kansasmemory.org/). 

**Challenges that I faced and what I did to help:** 

It was difficult to navigate Wget and I ran into a few problems. The first issue I ran into was when I used this command in the terminal: wget https://www.kansasmemory.org/item/223662. This url was the one from the main page of the diary on the website. When I entered this, in the directory was a document that led to this:

Following this, I attempted this command at the terminal: Wget https://www.kansasmemory.org/item/223662/text. The url that I used here is the url for the text version of Abbie Bright's diary. This pulled something, however, when I opened it, it led to this: 

After encountering these errors, I went back to the [Wget Tutorial](https://craftingdh.netlify.app/tutorials/wget/#basic-usage) on the class website and used what I learned from Part Two, and I inspected the images of the diary and found the numbers and format of their urls. From this, I created a list of urls in Sublime Text with all 86 pages as I was having a hard time using Python to generate a list of urls, so this was easier for me to tackle, even though it was more time consuming. I saved the file as urls.txt and put it into my folder for Abbie Bright's diaries. I then went back to the terminal from the folder, and used this command: 'wget -i urls.txt -r --no-parent -nd -w 2 --limit-rate=100k' to pull the 86 page diary from [Kansas Memory](https://www.kansasmemory.org/). Finally, it worked! 

