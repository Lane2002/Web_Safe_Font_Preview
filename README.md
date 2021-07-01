# Web_Safe_Font_Preview JQUERY
My Home
Course Menu
Get Unstuck
Tools


Avatar
Learn jQuery: Web Safe Font PreviewBrief
Objective
LEARN JQUERY
Web Safe Font Preview
While there are many fonts you can purchase and add to your site, there are also several free, web safe fonts that work across all browsers. Your company wants you to build a simple app to preview different web safe fonts, sizes, and weights. With jQuery, it’s a snap!

If you get stuck during this project or would like to see an experienced developer work through it, click “Get Unstuck“ to see a project walkthrough video.

Tasks
10/10 Complete
Mark the tasks as complete by checking them off
1.
To begin, look at index.html:

There are three fields in the <form>, two <select> menus, and an <input>. We will target each of these fields by its id.

There is also a <textarea> where the user will enter the text to preview. We can also target this field by id.

We will use the keyup event handler to update the preview text, so we don’t need a submit button.

Now navigate to main.js to start coding.

2.
In the main function in main.js, add a keyup event handler to '#text'. Make sure it takes a parameter: event.


Stuck? Get a hint
3.
In the keyup callback function, call the html method on the '.preview' element and pass it the current value of $(event.currentTarget), the updated input field, by using the .val() method.

Then test that entered text is being added to the preview after each keystroke.


Stuck? Get a hint
4.
Under the keyup method, attach a change event handler to the <select> field with an id of "font".

The change event handler will fire anytime the selected value of the '#font' menu changes.


Stuck? Get a hint
5.
In the callback function of the change event handler, use the css method to change the value of the '.preview' element’s font-family property to the current value of this menu.

Now test your app to see that the font of the preview text changes when you select a different font.


Stuck? Get a hint
6.
Now add another change event handler, this time to the weight menu.

Just like in the last task, have the callback function set the preview element’s font-weight property to the current value of this menu.

Test that the font-weight changes.


Stuck? Get a hint
7.
Since the font-size input field requires text to be entered, we’ll use a keyup event handler to change the font-weight of the preview text.

Add a keyup event handler to the font-size field.


Stuck? Get a hint
8.
In the callback function of the keyup event handler, create a variable called fontSize. Set it to the current value of this field, and use the + operator to add 'px'. We do this because we will need to specify the unit for the CSS font-size property in the next step.


Stuck? Get a hint
9.
Change the font-size property of the preview text to the value stored in fontSize.


Stuck? Get a hint
10.
Now give it a try! You can now easily preview font sizes, families, and weights to determine the right combinations.

And you could go even further! You can see list of web-safe fonts here. Feel free to add them to your <select> menu to make your app even more comprehensive!
