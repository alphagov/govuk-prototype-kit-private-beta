## 6 - Put your prototype online

To put your prototype online, you'll need two accounts: GitHub and Heroku. They're both free.

[https://github.com/join](https://github.com/join)

[https://signup.heroku.com/](https://signup.heroku.com/)

If they ask you about programming language, select Node.js

### GitHub (sharing your code)

Before you can run your prototype online, you need to put the code on GitHub. This is not the only way, but it's relatively easy, and you'll need to use GitHub anyway to share your code with your colleagues.

Some concepts:

**Git**			a way to save versions of your code

**GitHub**		a site that uses Git to share your code online

**GitHub Desktop** 	an app that helps you put your code on GitHub

**Repository/repo** a Git project

Download GitHub Desktop from [https://desktop.github.com/](https://desktop.github.com/)

Run GitHub Desktop, sign in with your GitHub account details.

Click **Add Local Repository** (if it's not on the screen, click the File menu and select it there)

Set the **local path** to your prototype folder

Github Desktop will now show a warning - apologies - this is the correct process!

In the warning, click **create repository**.

On the next screen, titled Create a repository, click the button Create repository.

In the top right, click **publish repository**

Make sure '**Keep this code private**' is not ticked, as we'd like others to be able to see and collaborate on it. Click **publish repository.**

Your prototype code is now on GitHub, other people can see and collaborate on your code.

### Heroku (running your prototype online)

Open [www.heroku.com](www.heroku.com) and sign in if you're not already signed in.

In the top right click **New **then **Create new app**

Names in Heroku have to be unique across all the users of Heroku. It can be helpful to add your name or organisation to the start of the name to make it unique. For example **joelanman-juggling-prototype**

Select **Europe** for the region - this is not important but makes your prototype a bit faster.

For **deployment method** choose **GitHub**.

Scroll down and click **Connect to GitHub**.

In the popup, click **Authorize Heroku**.

In the **repo-name** field, type all or some of your repo name, as it is on GitHub. Click **search**.

Click **connect** on the right of your repo.

Scroll down to the **Manual deploy** section and click **Deploy branch**.

One more thing: we need to set a username and password or the prototype won't run online.

At the top click the **Settings** tab.

Click **Reveal config vars**.

In **KEY** put the word USERNAME

In **VALUE** put a username of your choice, click **Add**.

That will be saved and you can add another KEY and VALUE.

In **KEY** put the word PASSWORD.

In **VALUE** put a password of your choice, click **Add**.

In the top top right, click **Open app** to see your prototype online!
