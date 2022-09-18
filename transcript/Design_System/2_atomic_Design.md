Transcript
Let's talk about atomic design.

It's a concept created by the awesome first, and it's basically a way of thinking about design systems

that bring everything down to really simple levels.

So we want to create a design system, but where do we start from?

How do we start designing?

How do we organize everything together?

That's what the atomic design methodology tries to solve.

It's a framework or a way of thinking about design systems.

So it's going to take our design system and break them into five different parts.

And again, this is just one methodology that could be many different frameworks for developing design

systems.

This one just got really popular.

So let's look at it.

So the idea behind atomic design is breaking down the components or the parts of our design systems

into five different parts atoms, molecules, organisms, templates and pages.

So let's get started looking at what this actually means.

So we almost already do atomic design in real life.

This is just a methodology to make it really understandable and put everything in perspective.

So first of all, an atom is the tiniest little unit that can exist on its own, an atom with a combination

of many atoms.

We can create a molecule and with a combination of many atoms and molecules, we can create an organism.

And with a combination of organisms, we can create a template.

And with a combination of templates, we can create a page.

That's the basic understanding.

Now let's transform this into web development terms.

When we talk about an atom, we talk about a simple label, for example, because a label can exist

on its own is very small, but it can exist on its own.

So that's what an atom would refer to a small piece of our system that can exist on its own.

For example, a label, an input book can exist on its own, but without any other elements wouldn't

really make a lot of sense.

But yes, it can exist on its own.

A button also can exist on its own, and a button with no reference wouldn't make much sense.

But yes, a button can exist on its own.

So atoms are those tiny little pieces of our system.

Now, if we look at molecules, you'd realize that it's a combination of atoms.

So how would this apply to Web development?

You'd realize that if we take one atom, which is the label and then another, which is an input and

then another which is a button and put all three together.

Now what we have is a such form and that is what we would call a molecule.

Now you can see that we are breaking down our UI into tiny, little understandable pieces, and that's

the whole point of atomic design.

Now let's look at what an organism is.

It should be a combination of many molecules and atoms together.

So notice on the far right we have a molecule right here and notice that we have some text or some labels.

So this individual items would be tiny atoms and then a combination of all of these atoms and the combination

of this molecule on the right all together from an organism, an organism is a larger structure.

It can actually make sense to the user.

For example, this is another another good example of an organism might be a blog post, a future.

So the larger the structure, the more meaning it gets.

For example, organisms have more life than molecules and molecules have more life than atoms.

They make more sense.

Now, let's look at what real life organisms would look like.

If you look at the Yahoo!

Facebook, Tumblr on Google, Etsy websites, you'd realize that they have a combination of atoms,

molecules and organisms.

So let's look at Yahoo!

For example.

You'd realize that there are many molecules, organisms and atoms in this whole system.

So first of all, we have a logo and the logo can exist on its own.

So we would say the logo is an atom.

Next, we have an input and a button.

And this would be able to create a such form called a molecule, because it's a combination of two items

to form one single item that can function together.

Next, we have a top bar that has an icon and some text, and all of these can form a top bar.

So this would be a molecule because it's a combination of tiny atoms that come together.

And on the far right, we also have a small action menu personalized to the user.

And this is a combination of icons which can exist alone.

So that would be an atom.

Then we.

Have some liberal checks or links, so those items and they all together combine together to form a

molecule.

OK, so that's the basic idea.

We look at ILUA, we break it down into tiny little pieces and then we develop with that mindset.

So now let's look at the example of our own design system that we build in this course.

So if you look at storybook, it actually breaks down our components into atoms, molecules, organisms,

even though we have just atoms and molecules here.

So let's look at the example of the atom.

It's a color component and the color component is just a box with a background color.

Now, this can exist on its own, but on its own it doesn't make much sense.

So let's say you want to represent a color.

This is the atom or the component that you would use.

It's very tiny.

It can be used in combination with other elements to make sense.

Now, let's look at the molecule we have.

The molecule is a solar component and it should be a combination of different atoms in our system to

make sense.

So if you look at this select first, there is a button that you can click and it opens and overlay

menu and it has some text.

So the button in combination with the text, in the overlay all together can form a functional molecule.

Now, if we check our source code, you'll realize that the packages themselves are a representation

of our system.

So if you check the source, you'd realize that we organize our source into atoms, molecules.

And if we have organisms that the organisms so the atoms, we have text, we have a merging atom, we

have some Coloradoan and then four molecules.

We have the select.

And if we also check our access package, we have atoms, we have molecules, and if we had organisms,

we would have that.

So the basic idea is designing a system with this concept in mind.

Now let's talk about the remaining two parts templates and pages.

So a template is a combination of different organisms to actually make sense together.

An example would be a logging page.

A login page would be a combination of a form, a Butson, maybe a Hedin, a card so that the user can

actually log in.

It would also have a checkbox or forgot your password link.

All of this coming together to actually make sense to what the user would use.

Now let's look at an example.

This is a homepage for a blog.

This is a template, but it does not contain real data.

So it's like a layout or a representation or a skeleton of what the actual homepage would be.

So you would build a template for your design system by sketching out a representation of what the actual

page or part of your site would be.

So this is an example template, and the only difference between a template and the page is the data

used in it.

So this is a template because it has some fake data, but then this is a page because it has real life

data in it.

So a template is a representation of what a page would become when fed with real data.

So that's the basic idea of design systems and we are going to follow these concepts when developing

our own system.
