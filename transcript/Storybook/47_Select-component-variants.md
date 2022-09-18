Lecture thumbnail
0:00 / 4:05
Transcript
Let's add some more variance to the select component in the selected stories that we are going to add

a new exports, constant random option, and these variants would be the case where the user wants to

render a custom option.

So this would render with no difference, but we can add the render option prop and this would return

a spine and we can get the get option recommend that props and spread on the spine.

And we can also get the option and render the option Laboe in the spine.

And we can also get the selected and we are going to conditionally see is selected.

Alice, I'm just trying so this would probably have.

So like that, and now if we check that in the browser select selection element, you can see there's

a select that string right there.

So it kind of demonstrates that we can customize the rendering of the option.

OK, so the variance that you provide here should be really developer hopeful that we, a developer,

can look at how you render the variance and know exactly how to use the component in your code.

Also, it should be able to show the power of your components to whoever wants to adopt your design

system, and another variants we have is when the user customize is the label so we can pass in custom

label and would render the select.

And pass in label right here, and this would be Selecter culo.

And now if we check the custom label, you can see that the label has changed to select a color, and

that's really good.

So we have three variants, one for common, one for the option, one for custom label.

And this should always represent how customizable your component can be.

And a good place to start is by looking at the interface.

So we've got three vans and these three rounds, actually much props that are passed into the component

now for the fourth one, this represents functionality, but you would realize that most of the vans

you have here are related to props that change the rendering of the component.

OK, so one final thing I want to add in this lesson is the ability to view the source code of the story

in the browser.

When someone is checking out the stories, it would be really helpful if they could see what you did

in the browser to render that.

So I'm going to be into packages react and they have a package called Story Book out on the story source.

OK, once that's installed in the main, the Jaspal, I'm going to add a new add on to the other are

a.

And that should actually be enough.

So let's give this a restart.

Bernini unstopped storybook.

And now if we check the browser, noticed that there's a new section at the bottom called Story, so

this shows the source code of the example we are looking at.

So you can see common is highlighted.

If I click on when the option, you can see that is highlighted correctly, showing exactly what I did

to render this example.

And the custom label also shows.

Now, another fun thing I want to show you is how group your stories together.

So notice that if I just add molecules and the pipe operator here, it's automatically going to group

the select into molecules.

And that's really good so that you can segment all of your components into bits.

OK, so I think we've covered enough for this lesson.

See you in the next one.
