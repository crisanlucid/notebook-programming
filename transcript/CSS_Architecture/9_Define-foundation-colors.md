Transcript
The next part of our system will be tackling is the cost.

Now, the cost we defined in the variables are just that variables.

They really mean nothing to our system.

For example, white, gray, green.

This does not really mean anything in our system.

The cost of SS as far is going to contain meaningful costs for the system.

For example, have set up some boilerplate here.

We can have global tax colors now.

We can have a color code, body text color.

And this would be.

The dark color from the variables that is found right here.

We can also have a body background color, and this would be the white collar from the variable that

was found and I also am using a plugin called Access.

Intellisense that we can have autocomplete for my variables in the other files.

So these two colors now make more sense.

So body text color is the color that we would use for the whole body of the site or for the components.

And now we would use this color and not this when defining our styles for atoms or organisms.

That way, it makes real sense.

Now, also, another advantage we have is this would be a default and not an actual value.

Remember, that exercise is going to Camperdown success.

So if it compounds don't like this, then there's absolutely no way to customize what the body text

color is.

So we would be replacing this with a variable.

So here we would have, of course, as we were called, design system for engineering.

And this is a short form.

And the short form here is kind of representative to what system we are created that way.

If there are others as variables from different packages in the application, then there is no conflict

or it's clearly distinct that this is coming from a design system.

So it designed system for engineering if you're working at the company, maybe called Airbnb.

This could be a B or something like that.

Now this is going to be E body text color and this is will take in a default value of Duqu.

Also, we are going to have default.

Now, there are three things going on here.

First, we are defining the Zwiebel.

Next, we are making it a success property with the default of dark.

And this, since this property is defined, is going to be the body text color that we if the consumer

of our design system does not use access, they can just define the sites as viable and every instance

of the body text color would adapt.

Also, if the user of the design system is using access, then we have this default flag, which means

that if they define the body text color, then it's going to override.

This one will do exactly the same thing for the background.

Color would have a variable called GSE body background color, which will default to white.

And this would be a default variable.

Now that's for the body.

Let's create some for the buttons of application.

So quit coming here, this would be four buttons.

And the first one that I want to have here is a button.

Primary color.

And they should be using a variable E!

BGN primary color, which will default to the whites.

And a default sasebo, then we would have a Butson primary background, this would be var Jesse b10

primary.

Background.

And this will default to.

The Green Zone would be a default access variable.

So we are defining specifically for the components that we would have in our application.

So, for example, if you're going to have forms, then I recommend having a Section four forms.

If you are going to have input boxes, I recommend defining some labels for input boxes.

And this would kind of be for the items of your design system.

Of course, that could be colors for organisms.

But in my experience, organisms are always a combination of different atoms together.

So this fire would mostly have colors for atoms, but it's completely fine if there are colors for organisms.

So another color I would like to add, maybe four buttons would be Butson, primary background, Hova.

And this would be a one off design system for engineering, but in primary background.

Over and by default, this would be the green light and would have a default.

Now this would contain everything we want for the buttons, maybe some secondary buttons and things

like that.

You get the idea.

Then we would have maybe another Section four forms.

This is another example.

So I'll quit comments, Heather.

And this will see forms.

For forms, I could define the color of the input boxes, so this would be maybe form color.

This would be a color.

Called from color and by default, this would be dark.

I could also have some for the background of reform in the Arab states, the Arab culture, the focus

color and so on.

So I'm just going to put in some examples.

This defines for the border when there's an error for the caller, when there's an error for the border,

when the user is focused on the form element.

So these are the colors that you would actually use when implementing your atoms, your organisms,

your molecules.

So in your atoms, you would never have maybe a hashtag for a specific color code.

What you would do is come here and for the specific atom or the component, you would define those colors

that would be used right here in this file and then use them in your atoms.

So in this lesson, we defined the colors and the main idea of the colors is to use the variables that

we defined to define colors for the different components or atoms or organisms that we are going to

have in application.

We started with the body.

So these are the global text colors would have.

So this is the body text color, the body, background, color.

We can also define the header, text color, the paragraph, text color and so on.

Next, we also have another component, which is buttons.

And this would most likely be an item in our design system.

We also have one who farms and you can have really any components you have in your system.

Now we are using six variables that we this can be overridden in and also in success.

So depends on what the end user of this package is using.

And this is going to make much sense when we finally pair this together with an actual example of a

use case.

So don't worry, if it doesn't make sense, just try to get the concepts and we'll work through it again

in a couple of lessons.
