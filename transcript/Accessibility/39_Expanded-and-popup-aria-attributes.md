Lecture thumbnail
0:06 / 3:24
Transcript
The selective grades, it looks really good for sighted users and they could play with this, but we

want us to work for all users, so it needs to be as accessible as possible to users that make use of

assistive technology.

So that's going to be the focus of this lesson.

We are going to get started with putting in the basics so that the screen with our software can actually

understand how the component works.

Now, the first thing you need to do is install Chrome Vox.

And it should be a chrome extension that you can install from the start.

I really have mine installed and once you do that, you can use it to test or see how easy it is to

understand your component when being used by a screen reader.

So, for example, I'm going to refresh the page and see how the screen reader interacts with my component

playground react.

He selected option ellipsis button.

So the first problem I realize is that he knows this is a button, but it doesn't know about the drop

down under the button.

So that's the first thing I'm going to fix in the select components for the button.

I'm going to add an area has pop up and I'll set this to true.

And let's see what difference that makes.

Playground react, he selected option ellipses, and that's a lot different, it's a pop up button and

now the assistive technologies aware that I have a pop up button, which means it expects to see more

contents when I click on this button.

So another area that we should definitely add to the button is the area expanded and would be able to

tell the assistive technology if the pop up for this button is expanded or not.

So if it's open, then the expanded will be true or else we're passing on the fine because it's recommended

to passing on the fine instead of false.

I also recommend adding an area controls and passing the idea of the select that it controls.

So here I'm giving it a select list and to my on that list, I'm going to give it an idea of just this

list so that the button controls this on that list.

Now, I would give the roll menu to the on that list because it's supposed to act as a drop down menu.

And this is the menu.

So with all the changes we've made, let's see if it makes any difference to our assistive technology.

So I would refresh the page so we can listen in.

Select option ellipses playground react, he selected option ellipses, he selected option ellipses

and expanded OK, and you can see that now it is informed that the pop up button has been expanded and

that's really good.

Now the next lessons would be to move focus from the button into the select.

Immediately the user expands it.

So using the keyboard, if they expand this, then automatically this strict block.

Right, which is the first option, should receive focus and actually be selected.

That way they can navigate up or down to select items.
