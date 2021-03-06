Thoughtful Reduction
--------------------

So we built our website up, like a painting, adding this color, that element, but don't get too attached.  It's time to switch hats, and thoughtfully start reducing and reevaluating.

A couple key questions to ask yourself:

1. Are we telling the story? I mean really, are all of these elements together telling a story? Does it flow? In our case the answer is no. Things are looking good, but I move guilty of getting lost in making things look good for getting the story. I'm also going the traditional rules of web design.  Don't get stuck in that period, break free. Allow the story to dictate the design.

2. Is this content really necessary? Don't get attached to content either. Less is more. Keep it simple stupid. There's a reason people say these things. Ask yourself if the content is really contributing to the story, or is it just fluff that sounds good?

With these questions  in mind start reviewing your website, and don't do it alone! Get some feedback. Create a second branch, call it "thoughtful-reduction", and like a sculptor, start whittling away until you are left with the bare essence of your website.

The great thing about mobile first is that this approach really helps you, right from the get-go, whittle away at the gruff, but don't stop now. Keep at it.

Take a look at these laws of simplicity by John Maeda:

- [Laws of Simplicity][]

[Laws of Simplicity]:                     http://lawsofsimplicity.com/tag/laws/

I'm not saying read this book, but look at the title, read the description:

Insanely Simple: The Obsession That Drives Apple's Success

> Simplicity isn’t just a design principle at Apple—it’s a value that permeates every level of the organization. It’s what helped Apple recover from near death in 1997 to become the most valuable company on earth in 2012.

> As ad agency creative director, Ken Segall played a key role in Apple’s resurrection, helping to create such critical marketing campaigns as “Think Different” and naming the iMac.

> This book makes you a fly on the wall inside a conference room with Steve Jobs, and on the receiving end of his midnight phone calls. You’ll understand how his obsession with Simplicity helped Apple perform better and faster, sometimes saving millions in the process.

> Segall brings Apple’s quest for Simplicity to life using fascinating (and previously untold) stories from behind the scenes. Through his insight and wit, you’ll discover how companies that leverage this power can stand out from competitors—and individuals who master it can become critical assets to their organizations.

### Looking at ViewThought

Looking at ViewThought there is a bunch of things I'm seeing that just aren't clicking for me. Why do I need a Work section, a Contact section, a Thoughts section? Here's a live example of ViewThought, version 2:

http://viewthought-2.herokuapp.com

If you bounce around each one of these sections, there really isn't that much content in each. I'm thinking that a single page website might make sense for us. Why move the user from the story flow?

If we go single page, do we really need navigation?

![][Navigation There]

With our contact us form on the same page,  is there anything about the footer that warrants having a traditional footer?

![][Footer]

What is the point of having related sites? Does it really add to the story? I don't think so, and the contact information can be made part of the contact us form, I have been thinking about doing that anyways. Does it matter to the end-user if ViewThought is a subsidiary of Ojala, Inc.? Not really, so why distract from the main storyline with this notation, even though it is minor? Every minor distraction altogether becomes noise.

And then there's the copyright. I'm not actually going to register this website, it is inherently copyrighted as an original creation, but without registration there's not much I can do:

- [Do I Need to Copyright My Website?][Copyright]

[Copyright]:                     http://www.legalzoom.com/intellectual-property-rights/copyrights/do-i-need-copyright

The fact is this website is the sample used for this book, the code is freely available to you to learn from and use in your own works. I'm removing the copyright.

Finally there is the social icons. Those are things I want to share, and I've been asking myself lately why are they so tucked away at the bottom of the website? Are they that unimportant?

Actually, they're not unimportant. They should be prominent, and here's a prominent space for them:

![][Navigation Gone]

That also seems like an interesting idea for the use of traditional navigation space. Here's what it will look like:

![][Navigation Icons]

Now people will know that I'm on all of these different social services – which they probably use, and they'll know this the moment they land on View Thought. I want them to. I want to be found.

As you read each panel are you feeling the story moving from panel to panel? I'm not. It's like elements of the story are there, but it's disjointed. I need to fix this.

Test, Test, Test
----------------

### User Aging Switcher

Throughout development I'm always switching between different

### JavaScript on and off

### Ask friends

### Different devices

Test your site on different devices! Don't just give this action lipservice, it needs to be done, frequently, and nothing can substitute an actual device.

When testing on different devices you'll find some things that worked on your desktop under different screen sizes actually really don't work on the real device.

I found that I needed to turn off JavaScript for certain devices.

Fortunately for us, mobile runs on a whole separate platform targeting JavaScript specifically for mobile is pretty easy.

Of four tablets it's also pretty easy...

### Services

### Emulators

### Cross browser

### CSS3 fallbacks and/or Polyfills

modernizr.js

    <html lang=en
    class="js no-rgba no-borderradius no-boxshadow no-textshadow no-opacity no-cssanimations no-cssgradients no-csstransforms no-csstransforms3d no-csstransitions fontface generatedcontent skrollr skrollr-desktop wf-camingodosweb-n7-inactive wf-camingodoswebn7-n7-inactive wf-quatro-n9-inactive wf-quatron9-n9-inactive wf-rooneyweb-i4-inactive wf-rooneyweb-i7-inactive wf-rooneyweb-n4-inactive wf-rooneyweb-n7-inactive wf-rooneywebi4-i4-inactive wf-rooneywebi7-i7-inactive wf-rooneywebn4-n4-inactive wf-rooneywebn7-n7-inactive wf-inactive">

PIE and ie7.js

Respond.js

### YSlow


### Images

http://www.smushit.com/ysmush.it/


#### Sprites

When you come to the end of your design and development, run YSlow. Checkout how many images are being called separately and combine as many as you can into a sprite.

Here's my sprite:

### Icon Fonts

Remove unnecessary icon fonts.



Feedback and Testing
--------------------

One very important thing to practice when designing interfaces is do nothing in isolation, and consider everything you think as intuitive,, to be wrong! (until proven otherwise) Iterating is key. Get feedback from your end users and refine. If you can't get to them, then ask your neighbor, a friend, or try one of the services listed in the [Feedback Services][Appendix 3] appendix.

> Test across major browsers, devices, and in front of "real-life" users.
\- [Manifesto][]

Testing on actual devices is also very important. Resizing a browser window and/or using device simulators cannot substitute for an actual device. The "[Device Testing][Appendix 3]" section in of the Appendices lists several useful articles to get you started on testing or building your own testing lab. As a rule of thumb, test on at least four different devices: desktop, tablet, small tablet, and a smartphone. Walk into the Mac store, or Verizon, or AT&T if you have to and test away.

[Manifesto]:            https://github.com/maxxiimo/the-front-end-manifesto/blob/master/MANIFESTO.md#the-manifesto
