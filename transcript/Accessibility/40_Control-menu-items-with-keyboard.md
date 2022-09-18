Transcript
OK, next, accessibility issue, we need to solve this, Selex should be completely navigated well

with a keyboard's.

So first of all, we should be able to open it with the answer key, the space key.

And once we open it, it should move focus into the dropdown that we the user can move up and down in

the dropdown.

So the first thing we want to do for that is in our select component itself.

I'm going to add an event is not on the button on Keadle, and this is going to call on button key down.

And how could this method here?

And this method is going to be of type keyboard events handler.

That way we can get the events here and the first thing I want to do is events that prevent default

because we are taking total control of the keyboard navigation.

Now, if the user press the space key or the key, we want to open the dropdown.

And also, if the user pressed the down our key, we also want to open the dropdown.

So first I would create a map of these keys.

So key codes.

Is an object, and here I would have the answer, this would be key 13, then we would also have the

space.

This would be key for to and would also have the down on the score arrow, and this is key 40 now in

our component.

Or in our method, we are going to check if every dot includes events, dot code and what are we do.

We want to check ones to check.

Key codes don't enter key codes, door space and key codes dot down arrow.

So if any of these keys were oppressed, then what we are going to do is called set is open to true.

OK, so now if we visit the browser, press the donkey, the dropdown is open, if I refresh, press

the space key, it's open, I refresh again, press the enter key, it's open.

So that works.

So we are able to open it.

Now we need to move focus into the dropdown.

So first of all, if we need to be able to move focus into the items of the dropdown, we need to have

room for all the items from the dropdown.

So we need an array of less.

Interesting.

So let's go to the top and create an array of refs.

So Konstanz option was.

And set option rates would be equal to your states and the states is going to be react that ref objects

and it would be an array of objects and by default it would be an empty array.

But the Reft object needs the type.

And we know that items are of type Eskimo Elai elements.

So it would be an object of type liste elements.

Now we have an array of refs, but we haven't yet assigned them to the elements.

So would come down here where we have a list item and it's kind of impossible to assign the ref if we

do not have the ref available.

So we need a use of a hook to dynamically create the refs.

So in the use of fake hook, the dependancy is going to be options that length.

So if the user maybe is passing in some dynamic options, maybe there are three.

That too.

Sometimes that 10, this would still work.

And what we want to do is called set option refs and we need to pass in an array of all the refs.

So we would look through the options.

So options that map and for each option we want to return react that creates ref and would pass in nothing

and this would be of type ascherman.

Ally elements.

OK, so for each of the options that are passing would create a ref and if there were five options,

then it would be five and would set them into the options.

Have now finally in the loop where we are looking through our list items.

I'm going to create a ref or available.

And this would be.

Option refs will pass in the option index, so that way we are Mappin here and we know that there's

an equal number of options and option refs, then the index is going to identify which ref belongs to

which option.

Now, here we can pass in.

Raif equals Raif.

Now, I do not want to keep passing the options here because they keep going, so what we can do is

spread.

Get the default options by calling when the option pops.

That gets option recommended right here.

OK, so we don't have to do that twice now, we need to pass in the ref here so that it's spread on

the list item.

So to confirm that we actually have the rest, we can console that lock option refs to see what we get

in the browser console.

So you can see it starts with known, then it goes to three and they are calling in all because our

job is not open.

So if we open the dropdown.

You can see that we have three and they are actually the options, and that's great.

So we haven't yet made use of this.

We are going to make use of this real soon back to our own buttinsky events.

What we want to do is set focus on the list item.

OK, so what we want to do in this case, to achieve this, I'm going to create a method called highlight

item and this would be a function and it will take in the index that needs to be highlighted.

So I would call this option index, which should be a number or maybe not.

In case we want to not highlight an element.

So what do we want to do in this case?

We need to highlight a specific item.

So let's say we want to highlight item zero.

OK, so the highlight item is going to save the index of the element that is supposed to be highlighted.

Keep in mind that our highlighted item right now works with just over and this needs a mouse, but we

need to be able to have it highlighted item if the user is using the keyboard and to keep track of this,

we actually need state.

So what I'm going to do is come here.

So where we are.

So that's an index.

I'm going to duplicate this and we are going to have highlighted index and set highlighted index.

And the highlight item is going to set.

Highlighted index to read option index, OK, and the highlights index now needs to control how the

element looks or if the element is highlighted instead of using the Hoover effect.

So I'll show you this.

Here we have the get option recommended, pops.

I'm going to add on mouse.

And so I'm going to call highlights item and I'll pass in the index of the options.

So option index and on mouse leave, I'm going to call highlights item and will pass in.

No.

Now what is this doing?

When the user enters the item, it's going to highlight it.

When the user lives with the mouse, it's going to on highlighted that way we are going to add a slice.

If it's highlighted now, we are going to come here and see is highlighted is equal to selected index

equals option index.

This should be highlighted index.

OK, now if it's highlighted with other class, so it's highlighted with a select.

Option.

Highlighted also at a space now in the browser.

The difference now would be that if we inspect this element when I hover over one, you can see it has

a class option highlighted right down there.

You can see the class keeps moving and that's what we want, because now if it is in states, then we

can set that using our keyboard, which is great.

Now, the final step is I want you to come to the select the access and on the hover where we have the

hover styling, this is going to be option highlighted.

So we are using that class instead because on the keyboard there wouldn't be any of us.

OK, so now we make sure this works as expected and that's good.

That's making sure it works for keyboards and also works for the mouse.

Now in the select, we are able to keep track of the highlighted element using a property, so.

We are highlighting the first item when the button is pressed, so let's see how that works with a keyboard.

I'll refresh this.

And then when I hit the space button, notice that strict black is great out.

So the back Wall Street black is great.

So it gives an indication that we are actually highlighting that item.

But that's not enough.

We need to focus on that item so that the screen reader can know that we are focused on that item and

then read it out.

So this is good for keyboard users because maybe they can see the item and recognize that it's highlighted,

but it needs to be better for those who are not sighted.

So we are going to set focus on this item.

So to focus on this item, what we need to do is get the ref and would get option.

Refs will pass in the option index.

And of course, we can't use no honor here.

So what we want to do is check if option index is not equal to No.

Then we'll treat this baby, OK, so we have the ref, so we're going to say if ref and ref the current.

Then what we want to do in this case is focus so with the current focus.

OK, so if you are trying to highlight the item or the option with index of zero, then we are going

to get the rest for index of zero and call the focus method.

So let's see how that works.

So I would hit up, get to that element headspace to open it up and it looks like the focus didn't move.

Let's check out what might be going on.

So maybe we should console the clock option index.

And then in here I'm going to console that, lock the ref to see what we get.

OK, so the console, that log is inside the option index.

Not, not.

So I'm going to heat up.

So like that element hit space and now look at that.

We have zero and Corrine's nor.

Hmm.

Why don't we try to highlight something else.

Hmm.

That's interesting.

That's because the menu is not present on the page when we've set highlights.

So we need to be so we need the ref to be available by the time we are performing this focused action.

So to do that, we can make sure the element is always on the page and that would be some success.

Or we can use the fact and listen to when the element is opened and then trigger the highlights.

So this is what we do.

Our position is open.

And then we are using on the facts here, so I'm would you say if I index is not equal to no and is

open is actually true.

So we are open in it, then what I'm going to do is get the ref.

So option refs and I'll get the highlights index and I'm going to see if ref and ref don't courant's

then ref the Coranderrk focus.

OK, so the reason why it doesn't work here is because we just highlighted the item or actually it's

because we just opened the dropdown and if we open the dropdown, we will need to rebrand up before

the job is actually available.

But while it is re rendering, we are trying to get or set the highlights item and focus it, but we

are hasn't had time to render, so the option is not yet available.

So in effect, we are able to know when the is open is actually done rendering, then we would focus

at that point.

So I would clean this up.

And we would just highlight now let's see if this works, so I would focus headspace.

Amstutz, strange word error, let's consider the look here again that's in the news affects Hook highlighted

index and then ref and then watch the console.

We actually have the correct thing, so we have zero, then we have to correct the list item.

OK, so after having a look at this, it kind of makes sense why we can't focus on that element.

Let me show you.

So if I select on this, it's highlighted, but we can't focus on it because it doesn't have a top index.

So we are going to come to the render option props and inside the get option recommended props.

We need to give this element a top index so that it's highlighted or forecastable or selective.

So we are going to check is highlighted.

Then we would give it a negative one, top index or zero.

OK, so now if we highlight the first item, so we visit the browser, then we select this by space.

You can see that the focus moves directly to it.

You can see that the keyboard focuses on this.

So that's the blue border.

Then the screen with that also focuses.

So that's the red border and that's really good.

All right.

So we've done so, so much in this lesson.

So I'm just going to try and take some time to recap on everything we've done.

First thing we did was to set up some refs.

So we set up an array of refs for all the options we have in the application.

So we use stage and set on MTV, but we needed a use effect so that we can look through all of the options

and set an option we have for each of the options.

OK, so in case the options change in future, then we would set refs again.

Now the next thing we did is in the loop for the list items.

We said the ref on the list item, so we got the ref using the index because if there are ten options

and 10 refs, then each option index corresponds to an option ref.

Next thing we did is we introduced a new state value called highlighter index.

This is going to keep track of what item is highlighted in the menu.

That way we can control the highlighted element from JavaScript instead of success.

And we also created a method called Highlight Item, which sets the highlighted index to the option

index.

Now, once it does this, there is a use effect that checks if the highlighted index has been set and

then it gets the ref and then focuses on the specific option that was highlighted.

Now, the highlight item right now, we tested this by calling highlights zero, but ideally this would

be dynamic.

Maybe we wanted to focus on a specific element based on props, but that works, too.

All right.

So this is a lot try to articulate all of this knowledge together, and I would see you in the next

lesson.
