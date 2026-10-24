CBLOCK.IN CLIENT FEEDBACK APP
==============================

FILES
- index.html: client feedback form
- thankyou.html: confirmation page
- cblock-logo.jpg: add your company logo image using this exact filename

EMAIL
The form is configured to send submissions to syedfordm@gmail.com using FormSubmit.
On the first test submission, FormSubmit may send an activation/verification email to that inbox. Open it and confirm before testing again.

PUBLISH FREE WITH GITHUB PAGES
1. Sign in or create an account at https://github.com/
2. Create a new PUBLIC repository, e.g. cblock-client-feedback.
3. Upload index.html, thankyou.html, and cblock-logo.jpg to the repository root (top level).
4. Open repository Settings > Pages.
5. Under Build and deployment, select Deploy from a branch.
6. Select branch main and folder /(root), then Save.
7. Wait for the published URL shown in Settings > Pages, usually https://YOUR-USERNAME.github.io/cblock-client-feedback/
8. Open the site URL and submit a test form. Confirm the FormSubmit activation email if requested.

IMPORTANT REDIRECT SETUP
The form currently has _next="./thankyou.html". FormSubmit may require an absolute redirect URL. After GitHub Pages publishes the site, edit index.html and replace:
<input type="hidden" name="_next" value="./thankyou.html">
with:
<input type="hidden" name="_next" value="https://YOUR-USERNAME.github.io/cblock-client-feedback/thankyou.html">
Use your actual GitHub username and repository name. Commit the change and wait for the site to redeploy.

TESTING AND PRIVACY
- Test on the published site, not just by opening the HTML file on your computer.
- Form delivery and redirect depend on FormSubmit accepting the submission and its current service behavior.
- Do not share the site with clients until you have confirmed the email delivery and thank-you redirect.
- GitHub Pages hosts static files; submissions are not stored in a private database by this app.
- The repository must contain only public-safe files. Never upload passwords, API keys, or private client data.
