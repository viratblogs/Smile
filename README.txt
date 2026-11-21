FOR MANVI — source package
==========================

WHAT'S IN HERE
  index.html          The finished site, one self-contained file.
                      All CSS, all JS, and all five images are inside it.
                      This is the one to upload / deploy.

  index-source.html   The same site with readable, separate image files.
                      Use this if you want to edit the code. It needs the
                      five scene-*.webp files sitting next to it.

  scene-1.webp ...    The five illustrations, 1000 x 1250 (4:5).
  scene-5.webp

  (You only need ONE of the two HTML files. index.html is the safe one.)

HOW TO CHANGE THINGS  (open index-source.html in any text editor)
  1. Your name
     Search for:  — Virat
     It appears twice: screen 01 and screen 05.

  2. WhatsApp button
     On screen 05 find:
       href="https://wa.me/?text=Haan%20bolo%2C%20main%20theek%20hoon"
     Replace with your number, country code, no + and no spaces:
       href="https://wa.me/91XXXXXXXXXX?text=Haan%20bolo%2C%20main%20theek%20hoon"

  3. Her song
     Make a folder called  audio  next to the HTML file and put
     her-song.mp3 inside it.
     If the file is missing the play button still works: it falls back to a
     20-second melody generated in the browser.

     Hosting in a sub-folder (username.github.io/manvi)? In the script,
     change   var SONG_SRC = '/audio/her-song.mp3';
     to        var SONG_SRC = 'audio/her-song.mp3';

HOW TO PUT IT ONLINE
  Easiest: go to app.netlify.com/drop and drag the whole folder in.
           You get a link in about ten seconds.
  Or: push the folder to a GitHub repo, then Settings > Pages > main branch.

NOTES
  - No build step. No libraries. No npm. Just open index.html.
  - The only outside request is Google Fonts (Fraunces, Nunito, Caveat).
  - Navigation is click-only: arrows, dots, keyboard arrows, or swipe.
    There is no scrolling anywhere.
  - The illustrations are from Pixabay (Pixabay Content Licence, free for
    any use, no credit required).
