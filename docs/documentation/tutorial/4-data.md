# 4 - Data

Our prototype now links users correctly but their answers aren't appearing on the 'check your answers' page. Realistic prototypes work better in user research, so in this lesson we'll use their answers to fill in the page.

### Fill in previous answers

When users enter data, it is saved using the 'name' attribute. You can use that later to show answers.

For example when the user fills in an input like this:

```
<input name="first-name">
```

The answer can be shown back to the user like this:

```
First name: {{ data['first-name'] }}
```

Let's show the user's answers in the Check your answers page

1.  Locate the answer for question 1 on the check your answers page
1.  Replace the answer with **{{ data['juggling-balls'] }}**
1.  Repeat for question 2 - its name attribute is **juggling-trick**

### Editing previous answers

The user's data is now showing in the Check your answers page, but if a user tries to change their answer, it would be good if their previous answer was shown - again this makes it more realistic.

For text inputs we'll fill data like we did with 'check your answers'.

1.  Go to your **juggling-trick** page
1.  Add **{{ data['juggling-trick'] }}** between the **<textarea\>** tags

The first time the user visits this page, **{{ data['juggling-trick'] }}** will be empty, so no value will be shown. When they visit it again, it will be prefilled with their answer.

Check this works by filling in an answer, continuing to the next page, and then going back to the page.

For radios and checkboxes, we use a function to mark which of the radios needs to be 'checked'.

The checked function looks like this: **{{ checked( "name", "value" ) }}**. We need to add it to each of the radio inputs in our **juggling-balls** page.

Insert the **checked** function above inside the first radio in question 1, like this:


<input class="govuk-c-radios__input" id="juggling-balls-1" name="juggling-balls" type="radio" value="3 or more" **{{ checked("juggling-balls", "3 or more") }}**>

Note the value in the input and the checked function need to be identical, including capitalisation and spacing.

Repeat for the other two radios, updating the value in the checked function.

Check this works by filling in an answer, continuing to the next page, and then going back to the page.

### Clearing data

If you do research with real user data, it's important that you clear any data stored by the prototype.

**Always run usability sessions in incognito windows** (In Chrome: **File > New Incognito Window**). At the end of the session, close all incognito windows.

To manually clear data, click on the **clear data** link at the bottom of any page of the prototype.

1.  Test clearing data by clicking on the **clear data** link at the bottom of the page.
1.  Return to a page that previously had data and refresh - is the data gone?

[Next lesson - Branching >](5-branching)
