Transcript
One of the items we have on our checklist is having a consistent code base.

This requires that for our success to be scalable and maintainable, we need to make sure that every

part of the code base is consistent with the order.

We shouldn't be able to tell which developer on the team, what the code based on that developer's preferences.

We should have a bunch of rules that we follow which involve indentation, verbal declaration makes

in declaration how to use maps and generally how our code should be written.

We are going to use two tools for this.

Starling's and Preacher Stalins is going to focus on how the code works.

For example, how to make sense.

Work functions includes use of variables and things like that.

And Preacher is going to focus on the formatting, which is indentation spaces, top sizes and other

configurations relating to formatting.

Let's start by installing this.

And would be installing the Starlene package will also install styling config sales guidelines, which

is a style guide for writing scalable, unmaintainable SACE.

So those rules will check our code to make sure we adhere to the recommended best practices, then styling

on Free Preacher, which is going to turn off all Starlin issues related to formatting because styling

can also format.

But we want to give the formatting job to Puccio and finally styling Puccio, which is going to run

preacher as a leans in and provide arrows when necessary, then would also install the preacher package.

Once it's done, installing the first thing we do is a dot starling's.

Our seat adjacent to our project.

Let's start by adding an object with rules property, which is also an object, and this is going to

have our first rule called indentation.

And Wood said this to to next in particular, Jason Wood at a Scripps section.

And this is going to have a Lindze, come on.

And this is going to run star Lynge.

And we need to provide the force that should be Lintott and here would provide all.

For us and for us and all for us, and then with that success now we can run Yahn Lens and notice that

it detects all of our source files and it wants the indentation on these files.

Some of them are supposed to be zero, but there were more.

Some of them are supposed to be true, but there were more or less.

And that's really great.

Now we have a bunch of errors telling us that our code does not adhere to the Linn's rules defined here.

Now, we do not want Sterling to care too much about formatting.

What we wanted to do is focus on the source guidelines.

So what we are going to be doing is extending the configuration for sousveillance.

So here I'm going to add stallion's config SAS guidelines now for us to make sure that this correctly

extends.

We could come to the GitHub.

And viscid this package, and when we visit this package, we can have a look at all the rules that

are available.

For example, block no empty to disallow entry blocks, so what we would do is go to the SAS.

And maybe to all that success, uncrate an empty block, so maybe that body and this is an empty block.

Now, we would want younglings to see if it would pick that.

And let's find out all that success and notice we have block no empty right here, which means that

the SARS guidelines is working correctly on our code base if we pull out the extends.

And one, this again.

Check the all access you do realize it doesn't show up.

OK, so would please step back in.

And I'm also going to remove the walls right here because we are going to be extending Starling's config

preacher that we all of the formatting rules for Starling's are going to be turned off and we are going

to use formatting rules for preacher.

So to use for rules for preacher, we are going to use Stalins.

Preacher Slash recommended.

And the Australian preacher package has a recommended set of rules that we can extend and finally we

are going to register a plug in.

For Starling's.

Preacher that we when Stalin is running, it would one pressure on force to make sure that the I to

this preacher guidelines defined by Stalin preacher recommended.

So now let's run younglings.

And I think I have a typo.

There should be Starling's.

Let's run that again.

And this should also be Starling's.

Here.

If we run younglings again, now we have preta.

You can see prettier is the arrow that we have on the right and it tells us that there's a bunch of

things wrong with indentation.

And if you also see we have wars such as a gold namespace after and all that.

So this is really good because our lintott is working.

The last thing we want to do is visit a package to Jason and add another one called Lint Fix.

And what this is going to do is run Yahn Linn's.

With a fix option, that way, it automatically fixes any errors that it finds.

So if we want younglings, it shows us the errors and now if we want younglings fix.

It fixes all the errors that it can fix, but it can get rid of this coach, so it still shows us that

error.

So in here, we have to manually remove the code with the empty block, one fix again, and now we have

a success.

That's great.

So in this lesson, we set up Starlene so that we can have a consistent code based structure and way

of writing access or sass.

First we installed plug ins so that we can use tiling and preacher together.

We also installed styling config sales guidelines so that we can follow the best practices for writing

SaaS.

And next in our package.

Jason, we have a lynch so that we can run to check all of our source files if the respective configurations

in the Stallard hours see the JASSA.

OK, so what I recommend to do with your team is to visit this package on GitHub.

Look at the list of rules and you can configure the rules option here if you want to override the rules

that your team does not agree with.

And you can also add a bunch of rules that is going to be really useful to your team.

Make sure you visit these other packages so that you understand what they add to your project and you

can pull out those that you do not like.
