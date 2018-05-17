# 2 - Create pages
In the file browser on the left, open these folders:
  -  **/app/views** - this is your 'views' folder, where your work lives
  -  **/docs/views/examples** - this is the examples folder, where templates live

![Screenshot of Atom showing folders](/public/images/docs/atom-folders.png)

Copy the start page template to your views folder: in the examples folder, right click **start-page.html**, and **copy**. Right click your views folder and **paste**.

You can check it works by visiting [http://localhost:3000/start-page](http://localhost:3000/start-page)

Note that the URL **/start-page** shows the page at **app/views/start-page.html**.  

For any new page - such as **example-page.html** you can view it by visiting **[http://localhost:3000/example-page](http://localhost:3000/example-page)**  

If you put the new page in a folder, you can view it by visiting **[http://localhost:3000/folder-name/example-page](http://localhost:3000/folder-name/example-page)**

Create two question pages - the template is **template-question-page-blank.html**. Copy it twice and right-click **rename** to **juggling-balls.html** and **juggling-trick.html**.

Edit the h1 in **juggling-balls.html **to be **"How many balls can you juggle?"**

Edit the h1 in **juggling-trick.html **to be **"Describe your most impressive juggling trick"**

Create a check your answers page. The template is **check-your-answers-page.html**. Copy and rename it **check-your-answers.html**.

![Screenshot of Atom showing Check your answers](/public/images/docs/atom-check-your-answers.png)

## Link the pages together

If we visit **[http://localhost:3000/start-page](http://localhost:3000/start-page)** and click 'Start now' it won't do anything. We need to link it to the next page.

There are two ways to link pages in HTML: links and forms. We use links when moving between pages that just show content, and forms when submitting user data.

Open **start-page.html** (make sure it's your copy in **app**, not the examples folder) and edit the start button link on line **52**. **Href** should be **/juggling-balls**:  
href="/juggling-balls"

Open **juggling-balls.html** and edit the form 'action' on line **22**. **Action** should be **juggling-trick**:  
action="/juggling-trick"

Do the same for **juggling-trick.html**. The action should point to the check your answers page.


## Finishing touches

Update the content in **check-your-answers.html** to refer to the two questions.

Use **[Answer goes here]** in place of the real answers.

Update the **change** links in **check-your-answers.html** to link back to those pages.

Set a service name - change **serviceName** in **/app/config.js**. Service name is used on start pages and in the header.

Go through your prototype and update the 'back' links so that they work.

Add some realistic content to the start page.

Create an **application-complete **page that links from **check-your-answers**. The template is **confirmation-page.html**

[Next lesson - Add questions >](3-add-questions)
