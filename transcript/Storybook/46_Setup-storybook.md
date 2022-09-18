Lecture thumbnail
4:13 / 7:52
Transcript
Let's set up a storybook for the package first I would get into packages, large react, and the first

thing we need to do is install storybook.

Slash react.

Once that's done, installing in our packages react, we would add a dot storybook for the.

And the first fire we need in this folder is, I mean, the Jets and this is the woods where we actually

configure a storybook, for starters, so we can export an object.

And the first thing we need to define is those stories.

So where would Storybook find our stories?

Stories would be an array, and Furnari would configures stories in the sauce and would find any foul's

in the sauce that end with those stories.

So that means for the sauce folder and the components such as atoms and molecules, would have their

own stories.

Now, for the select, we would have a select short story and story book would be able to find out based

on this configuration.

Now we have typescript installed.

So Stollberg needs to know how to compare our typescript down to stories that we can understand.

And for that we are going to add another part each.

Storybook slash preset type script and storybook behind the scenes makes use of weapons.

So this Brissette kind of sets up everything that Wepa, Babbo and Storybook need to compile and render

typescript correctly.

OK, so what's that's done installing in the configuration file, we can add and add ons property and

this takes in an array of Add-Ons kind of extensions for Storybrooke and in this case, we want to register

storybooks preset TypeScript.

OK, so all that's left right now is to actually launch storybook.

If you check the packages react and you check the node modules, you realize that in the beginning we

have two scripts that builds to a book and starts to reboot.

And this is actually all we need to work with Storybrooke.

So in the package there, Jason, I'm going to add a new script called Start Storybook, and this would

be Yahn Start Storybook.

Or we could actually just execute it directly.

Now, I'm also going to add one called Build Storybook.

Which would execute the build storybook.

Binary, now we can one start storybook.

And the first thing Storybook does is find stories based on the configuration and then once we're able

to compare them.

Now, you might receive a bunch of arrows, for example, the first one we have here is we are actually

missing baseball loader, which is required by storybook.

So let's go ahead and add that.

And once that's done, there's one young starts to walk again.

And now it found more errors and notice that it wants to rebook on a random spot on a computer and it

opened to the right.

So storybook, first of all, tries to use the configuration we have in the main file to find any stories

that we have available.

And here we are saying you should find stories and any dot stories, dot CSX.

But we have known.

So the message says there is no story available.

So let's add a story to see how this works.

So in the molecules select in the select folder, I'm going to add or select the stories that Kazaks

now in here, I'm going to import, react from, react so that it's in scope and I'm also going to import

the actual select component.

From Select and now Storybook expects us to export a different object where we can define configurations

for this story, first would have the title and the title would be select because that's the name of

the component.

So to render the select let's export a constant code common.

And this would be an example.

Select rendering source select.

I was passing options to be called to an empty RV, OK, so look at that, once we render an export,

come on, we have it showing up in the browser.

So notice that storybook is able to detect that we have a select story and it needs to render an example

of that component.

So that's why we have one for the export with the name which shows up here.

And the second export is a name called Common, which is a representation of how that component can

be used.

So if we have many use cases for that component, we can have a common one, common to common three,

common four.

And all of these are going to show up in Storybrooke.

You can see right there.

And that's really cool.

So for each of these cases, we would render the component in a different way to demonstrate how this

component can be used.

In this case, we have just the common case, which is putting in the options.

And of course, if you check the rendering of the component, you would realize that there's something

weird going on, and that's because the styles are not applied.

So right here in Storybrooke, we can import the case files required to correctly render this component.

So I would import ideas that e slash.

Access slash, life slash select DOCSIS.

And now you can see that the states applied correctly.

Now we have no options, we can create some dummy options or we can just copy from our test since we

have those.

And in those stories that CSX.

I'll pace this in.

Probably give them some reasonable values.

And possible options.

To the common example.

OK, so now if we check our story book, great, you can see that it works correctly.

So in this lesson we got started with story book and the first thing we did is install some basic packages

required to run Storybrooke.

First, we installed Storybook React and actually installed Bubble Luder and Storybook Preset TypeScript.

Once we had this installed, we created a DOT storybook folder and had a mean just file in the first

configuration, Tolstoi Storybook, where our stories are located and the second configuration is an

add on that helps to compile typescript correctly.

Now in Select Dog Story Statistics file, which is our first story, we import the actual select component

and we imported the CSS as required for that.

So the components work correctly.

Then we define some dummy data and we exported a different object that has the title of the component.

So here the title is Select and on the storybook menu it shows up as select.

Now, the default export is going to be the top level that we see right here, and the other exports

are going to be samples of that component being rendered.

So the first sample we have here is the common sample and the common sample is the most common use case

of this component.

And the most common use case is just passing in some options into the select OK.

And once we do that, we were able to figure them out and display them right here.
