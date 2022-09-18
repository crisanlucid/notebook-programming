Transcript
When members of our team right, could they have to remember to run Lynnfield that way, it formats

the code properly and when the we request all the code attached to our standards.

Now, this might not always be the case.

So it's always a good practice to automate the process of running Linn's fix on the code after the developer

is done walking.

To do this, we are going to install two packages at Def Huskie and Leane Station.

Huskey is a package that can help us use get hooks, for example, if we want to run a command before

we commit or after we commit or before we pull or after we push and lean.

Stasch is a package that uses Huskie to run commands only on files that we staged before committed.

So let's install this.

And the first step is for us to declare what hooks we are interested in, we are going to call Huskey

and that's in our package to Jason and we are going to have a whole section where we define all the

hooks we are interested in.

In this case, it's pretty comit.

So before the developer actually commits the code, we would run Lenn staged.

When the developer tries to commit now, the stage is going to receive a configuration also, and this

is going to contain the commands to run on stage.

Foust So here we are going to say and how that ends with that success should go through Yune lens fixed

now Youngling Fix is going to try to format the files that the developer joshed and if there are any

errors doing the formatting, it's going to stop the commission process.

So let's try to make some changes to an successful so in the cost of success.

Maybe we want to add a new color or maybe the variables that success.

So we want to.

Maybe remove Israel from the list.

This is just an example, so I'm going to get statures here.

We can see that we modified three Fous package to Jason Yanda block for the packages we installed and

the way that success.

So we need to commit.

And when we commit, we expect that our setup would run checks on the entire file that we touched.

And if there are any in problems, then it's going to indicate so get everything.

Get a message and I'm going to put you in the face of this lesson, because that's what I do after every

lesson.

This will be lesson 13 sets up Huskey.

We commit Hooke's.

Notice that it's running Sask and this wasn't what we had before, the run in to us is because Huskie

is able to listen to the gate command and then run the stage commands on the fires that were changed.

Now let's make another commit, but one that violates one of Allinson rules.

So let's add an empty block to this file, and that's against Clinton rules.

So let's say we had a body with an empty block.

We are going to get at everything.

Remember, this is a successful and if you check the statutes, we have one file, let's get committed

message error.

And if everything works correctly, it should cancel the commit unforced error.

It's one in youngling fix and you can see that it can fix that crowd, so it stops the comet, then

prints out the arrows from the youngling fix.

Come on now.

If you check gridlock, you realize there are no new comets added to the lock.

OK, so that's great.

That's how you can automate running these Clinton checks for your project.
