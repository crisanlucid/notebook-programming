Lecture thumbnail
0:32 / 5:56
Transcript
Let's talk about visual testing when you're building a large application with a lot of team members.

Things can change that can slide through the test, such as the stylus for the components.

And if the components change visually, since we are using an atomic design system, the molecules changing

would affect organisms and organisms changing would affect the pages at the end of the day.

So taking a visual snapshot of every component and comparing with the previous one we want to make changes

is a really great way to avoid this.

Now the creators of Storybrooke have a tool called for Mattick, and the points of Komati is to visually

test all of the components we have in Storybrooke to make sure that there are no visual regressions.

Chromatic would take all of our storybook stories and then upload them to the cloud, take visual snapshots

of each component and store them.

And when we try to make changes for our pull, request or push, it's going to compare the previous

one with the new changes to make sure that there is no large difference visually between the different

states to get started.

Go ahead and register a free account, and once you do visit your dashboard, you'll be able to add

a new project and give the project name.

So in this case, the project name is going to be DDE, which is the name of the scope of our packages.

Now, once done, it's going to give us a bunch of really useful instructions and what we are interested

in, your first of all, is installing chromatic.

So I visit the application then into packages react unwarned at Def Chromatic.

Now, once that's done, the next step is to publish the story, but we have to the specific project

that we've created in the cloud.

So I would copy this.

Common, and this is my terminal I one young Komachi and provide the Project Tolkan, which is what

I copied for my Komachi dashboard.

Now what this would do is detect the storybook installation we have, pull out all of the stories from

the story directories and bundle them with storybook, publish them to chromatic, and it would begin

taking the snapshots in the cloud.

OK, so once it's done, it would give us a report, found two components with five different stories

and they took five snapshots now will be from to add acousmatic scripts.

And I think that's great.

And once we set up Komati for our CIA involvement, we are going to add the token as an investment vehicle.

That way, it does not appear in our package that Jason.

So right now it's in our package to Jason file and our change this to yarn and we should be good to

go.

Now let's visit Chromatic Dashboard and we should have a change of your to continue our setup.

Notice that it takes a snapshot of our component.

And it also has a snapshot of a select component.

Now, if we want to spot your changes, we can make a change that actually affects the UI, like changing

the course of a component, giving it the wrong color or something like that.

Automated says wouldn't catch this, but Komachi would be able to detect the changes.

So to test this last visit and it's all.

Viscid the select the six.

And I'm going to make a change that actually changes things.

So, for example, the select label has a background of some background color.

What if we change the color of the budget, so change the color?

And I would give this a color of green.

And that's a different color from what we had before.

So let's see if Komachi would be able to catch these visual change first.

Let's make sure there's actually a visual change in our component.

And that's it.

That's a visual change.

So now this was a big or huge mistake from our engineers.

We are going to one young chromatic to see if this changes.

So when we want this, it's going to on chromatic with our project token and send this to the cloud.

OK, so you took five snapshots, just like the last time, but this time around it found three visual

changes and notice that it filled with an exit code of one.

And that's really good, which means that we can one access in the environment and it would feel if

the any visual changes detected.

So now let's visit our application again in the cloud.

And you can see that there's a notification on the dashboard that says one component changed.

And you can see the select actually has a snapshot.

So the baseline is the black one on the left and then the new change is the green one on the right.

We also have an option to accept the change.

So would accept it.

And we can also add comments, talking with our team mates about the change, making this as complete

and learning how to merge.

OK, so that's actually it.

We can also visit a dashboard to view a list of all of our components.

We can also invite our team mates.

View a list of all our components and look at how nice they are, they are broken down into atoms,

molecules, just like we did in our storybook.

All right.

So that's the basic of using chromatic to be able to detect visual changes that happen in your application.
