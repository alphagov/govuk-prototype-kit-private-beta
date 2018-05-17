## 5 - Branching

Our first question asks the user how many balls they can juggle. We're going to send them to an 'ineligible' page if they can only juggle 2 or less.

To do this, we're going to need an 'ineligible.html' page to send them to, and some logic to decide when to send them there.

The logic takes the answer the user has given to the first question, and depending on what the answer was, either show them the next question or send them to the ineligible page.

### Create the ineligible page

1.  Make an **ineligible.html** page by copying **template-content-page**
1.  Update the content to tell the user why they're ineligible.
1.  Update the back link to point at question 1
1.  Check it works by visiting [https://localhost:3000/ineligible](https://localhost:3000/ineligible)

### Route users to the ineligible page

We're going to write some logic to look at the user's answer to question 1. If the user can juggle 3 balls or more (the first answer), we'll show them question 2. If they answer with anything else, we'll send them to the ineligible page.

1.  Open the **routes.js **file: **/app/routes.js**
1.  Insert new javascript into **line 10**, before **module.exports = router**

```
router.post('/juggling-trick', function (req, res) {

  // Make a variable and give it the value from 'juggling-balls'
  var jugglingBalls = req.session.data['juggling-balls']

  // Check whether the variable matches a condition
  if (jugglingBalls == "3 or more"){
    // Send user to next page
    res.redirect('/juggling-trick')
  }
  else {
    // Send user to ineligible page
    res.redirect('/ineligible')
  }

})

```

Check it works - test each of the answers.

[Next lesson - Put your prototype online >](6-put-your-prototype-online)
