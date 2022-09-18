Transcript
Before you dive into this section, I think it's really important for you to understand exactly what

we are trying to achieve.

So first, I'm going to demonstrate to you the sixth package or the structure of the success that we

want to achieve.

And then we are going to start building this from scratch till we get to our destination.

So this is kind of like me coming back from the future to show you what we are going to achieve.

So first, I have a script run in.

In development mode and they have a sample application, so we are going to set up this morning repository.

You don't have to worry too much about it for now, but basically it's a real application that is running

in the browser with a button.

OK, so we have an example button component mounted in the index file.

And let's check the source code of that button.

The button.

Is going to use a class called a button container.

Now, where is this class defined?

It's going to be defined in a package called success.

And if you visit Atom's Button that says we are going to define the class here.

Now, when we define this class, we are going to have a script called Bude, which would fetch that

file and build the success into success and dump the results in this life folder so you can see it generates

success at the end of the day.

Now, the playground, when important the component is going to also important access for that component.

And in the browser we would see the class being applied.

So let me inspect right here.

Click on the button and you can see the button container and you can see the stoush right here.

Now, this is really important because you realize that if we have to use just four components from

our design system, then we would import justice for those four components and no other extra seats

will be added to our bundle.

Now, we also use variables, as you can see.

So the background for this button is var, so that's available and then there is a default so that we

that's how the background comes.

Right here now, if we want to override this, what we would do is create maybe an index case file and

then define some loose variables.

And the one we would be defining in this case is.

Jessie button for my background, and this would be read.

OK, now, finally, we would go back to our index file and then we would import index DOCSIS and see

that in the past, now our button becomes red y because we have over Ritson the default green value

and now we are using a red button.

So this is what we want to achieve.

We want people to import access by default, but be able to override that access by defining their own

variables, just by defining variables.

They can completely override the background color of all the buttons in the system.

So our design system supports customization and every single decision we make is going to be permitting

users to do this.

So again, you do not have to worry about all the files that we have here.

All you need to focus on is how the design system would be used.

We import a component, then we import the access for the component and then we can override using access

variables.

Now, if we were compiling which source, you would realize that our system also allows overriding variables

in access for customization.

So in the next lesson, we are going to get started setting up the repository from scratch, setting

up the access folder from scratch, and we will start writing the access for the foundation of our design

system, global overwrites best practices and things like that.

OK.

So I hope you understand what we are trying to achieve.

Go ahead and dive into the next lesson.
