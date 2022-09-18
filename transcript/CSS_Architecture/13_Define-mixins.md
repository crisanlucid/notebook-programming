Transcript
As your design system grows, you would realize that could duplication is unavoidable.

That's why we have mixes.

We want to make our code more reusable and having a bunch of mix things can really make this easy.

Now, all Mexicans are going to be in this file.

But as your design system skills, if you have maybe two hundred lines of code in this file, you would

want to create a folder called Make Sense and then import all of the make sense into this file.

In this lesson, we'll be defining a really common mixing that is used in almost products.

Now, in a typical Sears's project, you would have a.

Excess rule, maybe that body and maybe the font size is.

Twelve pixels and you would have access at Major.

That takes in Menwith.

Of maybe 48 eight web and ads are accessible to that, and this would seem fine at first, but there's

a couple of problems with this approach.

Number one, we had in the Menwith and this should actually respect the variables that we defined as

break points.

Number two in this whole line of code over and over becomes cumbersome and kind of loops duplicated

all over the place.

So what we would do is create a mix in.

So I would create a mix in called tablets.

And this mixing is going to have a major query, men with for this media query is going to be the big

point.

So I would call the map, get function to get Brigg points and I would get M.G. for the tablet and I

would print out the content here.

Now, this mixin is going to be years like this.

So let's say we have a body and we had font size of 12.

So we can see at include tablets.

And pass in font size of 14 pixels, and I think this is really, really good because it solves all

of the problems you mentioned.

Number one, we do not need to target the breakpoint right here.

We just call the mixin.

And it would target the specific viewpoint that we if we want to change the value of this breakpoint,

is going to change year in our project.

Now, I would duplicate this because we have just three points and this is going to be laptop.

And the big point in this case is large and the final one is going to be the next stop.

And the big point is.

Extra large that we if we want to style for the laptop, we just need to include.

Laptop define the font size.

And if we want to design for next up, we just need to include the stop and the font size for the next

stop.

OK, so I think that looks really clean and we would be able to write scrapbooks with these helpful

makes sense.

So in this lesson we talked about makes sense and how they can help us kind of refactor our code so

that it's not duplicated and not cumbersome to write.

We created a mix in called Tablet Laptop.

And next up and these basically abstract the with major query so that we can easily define responsive

components when writing our styles.
