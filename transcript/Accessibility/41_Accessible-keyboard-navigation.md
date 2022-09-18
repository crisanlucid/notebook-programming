Transcript
We are able to automatically set focus on the first element of the list when the list is open, but

the user can still not navigate using the keyboard.

So that's what we want to work on now.

We should have an event listener listening in on key press events and should be able to navigate one,

two, three down to the bottom and they can press the up key to move up the list.

So for us to go to our select component and on each list item we want to add and on key down handler.

And this would be an option key down.

So let's create this function and this option will be called every time there's a key down event on

one of the options.

So what type unnoted this to be keyboard, Iran, Knysna.

Would receive the keyboard event, and now if the user is navigating the list, a cool thing we could

do is check if this key is escape and if it's a skip, we can close the list.

So escape key.

I'm just going to add Etsy to our key quotes, and this would be key.

Twenty seven and twenty seven is going to close the list.

So we'll just check here if the event the key code is equal to key codes, dot Etsy, which is the escape

key we are going to set, is open to force and return.

And that's just a nice little functionality we can add, so if the user is navigating and person says

keep it close is the list.

Now what if the user pressed the down arrow?

What we want to do is check if it's the arrow.

So if the event the key code is equal to key codes, the arrow, then we want to go to the next item

in the list.

So we want to highlight the next item in the list so we can correlate item, but we need to get the

next item based on the current highlighted index.

So we should probably create a helper function.

So at the top, right outside of the select, I'm going to create a helper function called Get Next.

Option.

Index and this would receive the current index, which should be a No.

And this should probably be a number on law and it's also going to receive options.

Which is an array of select options.

So what do we want to do in this method?

We want to check if the current index.

Is law, which means that there is no current index or the highlighted index is no, then we are going

to return zero that we the user is on the first next if the current index.

Is equal to options at length minus one, it means that the user is currently highlighted on the last

item in the list.

In that case, we are also going to return zero so that we take the user back to the first item in the

list.

And finally, in any other case, we are going to return current index plus one.

OK, so let's try this method out.

I'm going to call get the next option index and I'll pass in highlighted index and pass in options.

OK, so I'm not very comfortable with this method being called highlight item, so I'm just going to

search and replace and rename this to highlight option because that's what we are highlighting.

OK, so now if I hover over this press space and I press the donkey, noticed that the highlight moves,

I press the donkey again, it moves, but there's something strange, OK?

There's nothing strange.

It's OK.

So you can see we can navigate using the donkey.

Now we need to also be able to navigate using the upkeep and the upkeep should go in the opposite direction.

So that means we should have another helper method called get previous option index.

This would take in the.

Current index on the options, just like the first one and in this case will check if the current index.

Is a question or then would return zero, which means the first item now we are also going to check

if the current index is equal to zero, which means the U.S. is on the first item, then we are going

to return options the length minus one, which means we'll take the user back to the last item.

And finally, we are going to return current index minus one.

So we take the user one step upwards.

OK, so we have to do all of this in case the user press the upkeep or we don't have a key code for

the object.

So let's please that the key is key for each eight.

So this would be up our key thirty eight and.

We have to check for Keith in our Hannelore.

So if events.

But could.

Is equal to keycards, the up arrow.

Then highlights option.

I would call gets previous option index and would pass in highlighted index on options.

OK, so now in the browser we can test this out.

I would press the donkey.

Remember, the donkey can open this menu.

It opens now I president kick in and they can highlight and move the highlights.

Now what if I pressed the of key.

You can see it does the same thing and that's really cool.

But did you notice that the focus did not move and that's really strange.

So let's check it out.

Effect's.

Checks for the is open and then sets the focus.

What if this also checks for the highlighted index?

Let's see if that's going to fix that.

So if we pressed down to open this, notice that it changes now because we are listening to the highlighted

index changing to execute that effect, and that's really good.

So now this select can be completely navigated using the keyboard.

Now, what happens when we hit enter on an item at the moment, nothing happens, but we need to be

able to select an item or an option using enter.

So what we'll do is listen to the Kentucky.

So that's the final event listener.

So if the event called.

Is a quarter key codes that enter, then we are going to code on option selected method and pass in

the highlighted index.

And let me check out what that method takes.

It takes in the option, actually, and then the option index.

So what we should be doing instead is passing in the option and there should be options.

Highlighted index.

And then the highlighted index, so we know that there was a key purpose, which means that the highlighted

index is definitely set.

So I'm going to put the exclamation mark to force typescript to ignore that.

OK, so now let's try this out it up for space.

So like the second one by hitting enter and great, you can see that it actually selects and that's

really good.

Now we need to add some area to our list so that the screen with our or assistive software can know

exactly which this item is checked and which one is not to do that will add an area checked and this

will be selected.

And if it's selected, then we would add two hours.

This would be undefined.

So that's how the assistive technology would know if this is checked.

But what is the role of this list item?

The wall is going to be menu item REIJO because the user can select just one option from this list.

So the word is appropriate for this use case.

We should also give this label so I could give this area a label and this is going to be option the

label just in case some screen readers can pick up the label text.

And I think that's it.

This is the most customizations I can think of that we need to add on our select.

So now make sure to navigate your select with the keyboard without the mouse and make sure that it's

completely possible to do so.

Make sure that chrome box can read these labels as you move up and down with your key board.

Make sure that when you hit enter conversations, take that this is closed.

Make sure that you can still select this and select a different option.

Make sure that if Chrome Box is reading through this list when it reaches this one, it actually says

it's checked because we have our area checked attributes right here.

And when it selects a new one, then if you highlight what that element work, should be able to read

the correct thing.

All right.

So that was a lot and I hope it all made sense.

Thank you so much for watching and see you in the next lesson.
