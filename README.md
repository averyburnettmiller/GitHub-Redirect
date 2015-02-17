# GitHub-Redirect Setup 
This repository lets you redirect a domain to another domain via GitHub.
(This comes in handy when your domain registrar doesn't support redirecting subdomains; in my case, Squarespace doesn't support this.)

If you'd like to use this script yourself, just follow the steps below.

## Step 1: Forking 
First, click fork (and maybe star? :smile:) in the top right of this repo.
When it's done, you'll see your own copy of **GitHub-Redirect**.

Next, click the button that says **branch:**. Make sure it says **gh-pages**. If it doesn't (it may say **master**), type in **gh-pages**. Next, go over to **settings**. Make sure that the **Default branch** is set to **gh-pages**.

##Step 2:  Editing index.html
Next, open up **index.html** and change the value of **url=** to the URL of the website you want to redirect the page to. (In my case, it was **github.averymiller.org**; **git.averymiller.org** redirects to **github.averymiller.org.**)

Also, change the link in the **You're being redirected to** section to the URL you're redirecting to.

##Step 3: CNAME
Lastly, go into your domain registrar, and set the subdomain that you'd like to redirect to point to **<Your Username>.github.io.**

Then open up the CNAME file, and change **git.averymiller.org** to the domain that you pointed to GitHub previously.

You're now all set! Head over to the repo settings; under **GitHub Pages** it should say that **:heavy_check_mark: Your site is published at <Your Domain>.**
If it isn't yet, wait a couple of minutes and check back.

Your domain will now redirect to what ever domain that you specified!

##Trouble Shooting
Make sure that the **index.html** file is lowercase; it's case sensitive!

Anyways, good luck! :smile:
