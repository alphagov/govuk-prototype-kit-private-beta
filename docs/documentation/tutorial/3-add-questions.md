# 3 - Add some questions

In this lesson we're going to add some radio buttons and inputs to the two question pages.

We'll do this by getting snippet code from the GOV.UK Design System. We'll copy the code we need into the pages, then update the content to match our questions.

The question pages link to the snippets, but you can also get them here: [https://govuk-design-system-production.cloudapps.digital/components/](https://govuk-design-system-production.cloudapps.digital/components/)

Note that HTML is a tag-based language, with opening and closing tags. For example:

```
    <p>This is a paragraph</p>
    <a href="/start">This is a link</a>
```

To start we'll add radio buttons to the first question

1.  Open **juggling-balls.html**. We're going to insert a radio button question in the middle.

1.  Locate the **radios** example in the Design System

1.  Copy the HTML

1.  Paste into your question page, replacing the two **<p\>** tags

1.  It's helpful to make sure the code is lined up correctly - select the lines and use **tab **or **shift tab**

1.  Update the new **<h1\>** text to your question text

1.  You can delete the span with hint text, or add your own hint text

1.  Delete the old **<h1\>**

1.  Delete **checked** from the last item.

1.  Copy and paste the last item, from **<div class="govuk-c-radios__item"\>** to the closing **</div\>** so you have 3 items.

1.  Update the content with options: "**3 or more"**, "**1 or 2"** or "**None - I can't juggle"**.

1.  Change the **value** attribute to the same as the question content above. Make sure to use the exact same capitalisation and spacing.

1.  Change **changed-name** to **juggling-balls** on each input **name** and **id** and **for**.  
Note that the name is shared - this represents the question, and the value represents the user's answer

1.  On the last option, change the **id** and **for** to **juggling-balls-3**

Next we'll add a text box to the **juggling-trick.html** page.

1.  Copy the html from the **Textarea** example in the GOV.UK Design System to replace the two <p\> tags.

1.  Delete the <label\>.

1.  Change the **name** and **id** to **juggling-trick**.

Check the question pages in your browser to make sure they look correct.

[Next lesson - Data >](4-data)
