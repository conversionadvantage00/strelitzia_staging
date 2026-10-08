Wildcoast Seeds website (staging)

Files
  index.html            The whole site. Photos, styles and scripts are built in.
  og-image.jpg          The picture shown when the link is shared (WhatsApp, LinkedIn etc.).
  apple-touch-icon.png  The icon used if someone saves the site to an iPhone home screen.
  README.txt            This file.

Publish on GitHub Pages
  1. Create a new repository and upload all four files to its main folder
     (not inside a sub-folder).
  2. Settings > Pages > Deploy from a branch > main, / (root) > Save.
  3. The site goes live at https://USERNAME.github.io/REPOSITORY-NAME/ within a few minutes.

After it is live
  - In index.html, search for YOUR-SITE-ADDRESS and replace all four with the real address
    (keep the trailing slash). Link previews will not show a picture until this is done.
  - Check the preview with https://www.opengraph.xyz or LinkedIn's Post Inspector.
  - WhatsApp caches previews: a link shared before the fix can keep showing the old version.

Quote form
  - The form in the Contact section is a demonstration only. GitHub Pages cannot receive
    form submissions, so it checks the fields and shows a thank-you message but sends nothing.
  - To make it live, sign up for a form service such as Formspree, then in index.html:
      1. Add action="https://formspree.io/f/YOUR-FORM-ID" method="POST" to the
         <form class="quote-form" ...> tag.
      2. Delete the "Quote form (demo ...)" block in the script near the bottom of the page.
      3. Remove the "Demonstration form..." line under the button.

Photo pop-ups
  - The small photo cards (On the farm, Reginae, Nicolai) and the four Quality steps open
    into a pop-up. The three small cards only have 200px copies of their photos, so they look
    soft when enlarged. To fix, upload the full-size photo (e.g. sunbird.jpg) next to
    index.html and add data-full="sunbird.jpg" to that <div class="inset-card" ...> tag.

Still to do before going public
  - Phone, WhatsApp and email (currently "[to follow]" in the Contact section).
  - Real Nicolai photos (the two images in that section are reginae placeholders).
  - Connect the quote form (see above).
  - Full-size photos for the three small photo cards (see Photo pop-ups).
