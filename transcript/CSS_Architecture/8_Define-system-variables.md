Transcript
The first one of these files will be working on these two variables, that success.

This is the starting point.

First, I have put in some really beautiful comments, and I highly recommend adding these comments

into your actual design system because they give a lot of clarity to whoever is looking at these files.

First, we have a beautiful headline that says variables.

Next, we have a table of contents for us.

We have colors.

Next typography and break points.

This would be responsive.

Breakpoints will use across our project for us.

They are broken down into three brand colors, neutral colors and utility costs.

If we have a look at our design system, you can actually see that they are broken down into the three

categories.

The brand colors, the green light, green, black and the lighter black, the neutral colors.

This one's right here.

And the additional or utility colors that would be used for maybe notification messages.

Our state's success.

These are the red, the light red, the blue, the light blue.

So we want to make sure that our design system reflects exactly what the designer has on the Stargate.

Next, we have typography, and this should also reflect exactly what we have on the.

So, for example, here we have had in style's body styles textiles, and that's exactly what we have.

We have families that are defined for those styles, fund weights, just like the designer defined here.

We have regular, we have lights.

We have the font sizes beside them.

And we also have line Heintz.

So we want to make sure that we reflect those so we have fun with fun families, that the project uses

the heading sizes and body sizes.

Finally, we have three points and this is really important for any system.

We need to know what are the standard break points that we are going to be targeting in the system,

at the mobile devices, at the iPod devices, or do we really not care?

So the first step is extracting the values from the design tool and defining them in this file.

First comes colors.

So I'm going to create are heading for colors and I'm using a tool called voice code access comments.

So if I search the extensions, you realize we have voice code comments and it provides little snippets

that can help you create beautiful headings like this.

So on the colors, I'm going to add another tiny comment for the subheading, which is going to be brand

colors on the brand colors.

The first one we have is green and this is five E, C, seven B, next we have green and we have a lighter

shade and this is nine E to be zero.

Next we have the dark and this is the second set of brown colors.

This is one the one feature.

And we have the dark light or the lighter shade of the dark.

And this is seven three, seven, six, eight.

Next, we add another comments.

And this is going to be for the neutral colors would have the gray, which this one's so the gray,

the gray light, then the really light gray and the white.

I'll just piece those in so I save some time.

And the final one is the utility colors.

And for these ones we're going to have the red, the red light, the blue and the blue light are losing.

OK, so it looks like we are done defining the colors and these are just variables.

We are not going to use these variables to design the components SE.

But you see exactly how all of these pieces come together.

Next, let's create a major hidden for typography.

So comments.

S. Hedin, and once you have that extension installed, you'd be able to type comments and see each

other in your.

We have typography.

And for our first subheading, we have phones, families on the phone.

Families should be defined.

In the projects now, some of the families defined here are premium funds, so I'm just going to replace

these with the low budget or free alternatives.

Our pitocin and the first one we have here is Playfair, and that's going to be the cell phones that

is used for all the headaches and the next one is real way, which would replace the sound that is used

for the body.

The fallback for the railway would be, how can you?

Helvetica era and the default century defined in the user's browser.

Now notice that we have some tiny comments beside these definitions.

So we have one and we have two.

And this is a great way to define comments for some decisions made in the code.

So with one and two, I can come right here after I define typography and paste in some comments.

So one is going to relate to number one and two here is going to relate to number two.

And this is a great way for you to define comments explaining the decisions you made.

So here I provide a you are all to the Playfair forms on Google and I see its four headings and I also

provide a link to the real waveforms on Google and explain that we'll use this for body text that kind

of gives more context so that the developer can click and view the fonts and kind of understand exactly

how the pieces fit together.

The next step is font sizes are comments.

This will be fun sizes and based on the sizes defined in the style guide, would be able to extract

those and actually create a standard set of font size.

Is that this project is going to use, for example, available font size.

Extra small is going to be the tiniest value of font size and this is going to be zero point seven five

REM.

And I'll put a comment beside that size 12 pixels.

Now we are going to be using REM because REM is really responsive in case the user changes the overall

size of the browser.

REM is going to easily adapt, unlike the pixel.

Now, even though we are using REM, it is really important that any other member of the team would

be able to understand and translate this easily in their brains.

So we add a simple coming here that converts this value to Pixel Max would have for other forms of deletions,

one for 14 pixels, 16 pixels, 18 pixels on 24 pixels.

And I've given them some reasonable variable names.

That's for font sizes.

Let's define font sizes for headings.

I create a comment.

This would be heading for sizes and I'll just put this in.

The variable in this case is going to be each so each one is going to be twenty two pixels.

Each two is going to be twenty two pixels and this will kind of differentiate using the fonts.

Wait for the heading.

These are very critical.

Based on the phone formulas we are using, S3 is going to be sixteen and so on.

The final step is the font which so I'll create a comment with font which in this case I just recommend

defining from the lowest to the highest somphone start at two hundred, some start at three hundred

in this case are forms that are three hundred.

So I would start like a three hundred write down to block nine hundred.

OK, so if you look at our table of contents that is the last sub menu item for typography.

The final step is the breakpoints.

In this case I'm going to define.

The head in.

This would be breakpoints.

And this would be a map.

Continuing to defend viewpoints first would have won for MTV and this would be 40 adream and our comment

is to be seven, six to eight pixels.

Next, we're going to have Lache, this would be six forum.

This would be 1024 pixels.

And finally, we're going to have extra large.

This would be a room and this would be one to 80 pixels.

These are the standard big points that our project would use.

OK, so we've been able to extract the designs from our design to or a style guide and define them as

verbose in this file.

Don't worry, all of these pieces are going to come together once we define the other foundation files.

So one last thing before I go.

You can define photos for your sections.

That way, it's really clear.

For example, here I can add a comment folder and this is going to be end of breakpoints.

Then here I can add a comment futer this would be an odd typo gruffy and finally.

Here I can define a comment future.

This would be enough close that way is super, super easy to read and really understandable by any developer.
