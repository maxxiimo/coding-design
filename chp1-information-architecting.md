Information Architecting
========================

In [The Front End Manifesto][Manifesto Book] we laid down the foundation of our application by:

1. Defining our base [markup][Chapter 1 - Manifesto] and [styles][Chapter 3 - Manifesto].
2. Choosing a [mobile][Chapter 5 - Manifesto] content delivery strategy.

NOTE: You do not need to read *The Front End Manifesto* to follow along with this book, although if you are setting up a Ruby on Rails application it wouldn't be a bad idea to do so.

Now it's time to build a user experience on this foundation: how your users will understand your [whatever you're building] and how they will [whatever they will do]. The key to being successful in building your applications user experience can be summed up in one word: **Storytelling**.
<br>
<br>
![][Storytelling]
<br>
<br>
> The other way to persuade people—and ultimately a much more powerful way—is by uniting an idea with an emotion. The best way to do that is by telling a compelling story. In a story, you not only weave a lot of information into the telling but you also arouse your listener's emotions and energy.

\- [Storytelling That Moves People][Move People] by Robert McKee and Bronwyn Fryer

### Storytelling in Web Design

Back in 2008, at "An Event Apart: Boston," I listened to [Jason Santa Maria][] – then the Creative Director of Happy Cog Studios – give a presentation called "Good Design Ain't Easy." In his presentation he described how stories were being told by design, with the designer in effect becoming the narrator. Another presenter at Fidelity Investments that same year also talked about storytelling and its importance in design. Although I no longer remember his name, I do remember his talks thesis: people understand and remember stories.

These talks have stuck with me over the years, and they have become the way I view information architecting and visual design; as storytelling. What follows is an explanation of how to build a story for your website and translate that into code, and beginning with [Chapter 2][] we will begin to explore creating the sites "look and feel" (visual design) from the same perspective of storytelling.

As a front end developer, without getting super complex or requiring a gazillion dollars, there are three basic ways to go about designing a website:

1. Start from scratch and architect and design everything yourself.
2. Work with a graphic designer from the get-go and implement a design mockup into your foundation work ([Chapter 6 - Slicing and Dicing Mockups][Chapter 6]).
3. Start from scratch and architect yourself, then get help from a graphic designer on the look and feel.

In this chapter we're going to mostly focus on option 1. Hiring a graphic designer from the get-go is not a bad idea, but perhaps there isn't money in the budget, or this responsibility falls on your lap, or maybe you just want to do it yourself. To illustrate how simple option 1 can be take a look at this 2007 website concept:

- http://noonebelongsheremorethanyou.com/00025

Jason Santa Maria pointed out this site in in his 2008 presentation I mentioned. What I like about the website is that it demonstrates the simplicity of storytelling: the entire site is written on kitchen appliances! ...and at the same time engages the user and ultimately delivers a message to entice action. We want to do this.

A Mosaic of Information
-----------------------

To build our story we should first explore what it means to organize a websites information and function.

> As a front end person, oftentimes taking the role of Information Architect, when I think about layout I literally think about how a site is laid out on a screen. I don't think in terms of code, but more so in terms of organization of information and function for an end-user's consumption.

\- [Chapter 1 - The Front End Manifesto][Chapter 1 Quote]

How does "organizing information and function" relate to storytelling? I like to think about it in terms of traditional mosaics. What is a mosaic if not a bunch of smaller things coming together to form a meaningful whole:

> Mosaic is the art of creating images with an assemblage of small pieces of colored glass, stone, or other materials.

\- [Wikipedia][]

Individually, the components of a mosaic are meaningless, but together they form a pattern or an image. Take for example this Roman mosaic of Ulysses, from Carthage:

![][Mosaic]

Is it a meaningless conglomeration of colored tiles, or does it tell a story?

A website layout is similar in that it is composed of different blocks of information that together convey a larger whole, a story composed of text, images, color, function, and more.

As front end developers we choose and arrange what blocks belong together, and through our code create a digital mosaic, a website, that ultimately is viewed and interpreted by our audience. As such we should think of what we create, it's meaning and purpose, as storytelling and ourselves as narrators. It's not as far-fetched as it might sound when you consider that most websites are probably designed to invite/entice/cause the user to take a next step or action, i.e. turn the page in the story.

The Storyline
-------------

The unifying message behind this mosaic of information is the storyline or theme. Before content can be discovered, grouped, and placed in a layout, the narrator, in this case you, has to have the stories general theme in mind. For example, the storyline might be:

> I'm a great Web site for finding a job...a job that is perfect for you, you should join me, if you do you will have access to tons of perfect jobs and your life will change for the better forever!

In this storyline example – with my Information Architect (IA) hat on – I immediately see several major blocks of information:

1.  What is the site in 10 words or less – possibly a summary box.
2.  How do I join – a sign-up section.
3.  An area that describes the benefits of the site – maybe user testimonials.
4.  The obvious table stakes to this story:
    - A logo
    - Legalese (Copyright, ToS, Privacy)
    - Non-legal footer type info (Feedback, About, Contact, Site Map)

...and as the front end developer I'm already beginning to imagine how these blocks of information will be organized and coded into our application and used by our backend development team.

This is exactly what you will need to do: think of an overriding storyline, organize it into blocks of information, then begin to imagine how it will be conveyed and coded. Just remember to keep the following tenant of [The Front End Manifesto][Manifesto] in mind:

> Architect and design for the end user, not developers.

TIP: Although I enter projects with a good idea of how the website might be laid out, following the processes laid out in this book the end result might be completely different from what I first envisioned. The bottom line is being flexible is a good idea. Don't invest too much ego into your work.

Gathering and Organizing Information
------------------------------------

Before you begin coding it's important to take a few preliminary steps. What follows are two techniques for gathering all the blocks of information that will ultimately make up the sites story, help define the user experience, and establish a layout:

1. Index Card Exercise
2. Prototyping on Paper

NOTE: I'm going to make the assumption that you have conducted basic client discovery and subject research for your project. Also, throughout this process I highly recommend keeping the book "[Don't Make Me Think][]" by Steve Krug nearby as a reference. It’s a good read and everything he says is so darn obvious you just might miss it, but thankfully Steve Krug puts it all there in one place for you.

Index Card Exercise
-------------------

The first technique involves the use of index cards to create a physical inventory of possible information components. It's best to do this exercise with others, especially stakeholders in the project. Here are the steps I follow:

*Step 1:* Write down in a word or two on an index card what the card represents: content, function, a navigational element, an image, video, whatever.

Think of as many components to the page or application as you can - I prefer dealing with a single view at a time, like the homepage.

NOTE: Color coding is helpful.

*Step 2:* Lay out the index cards on a table, organize them into logical groups like navigational or footer areas.

*Step 3:* Review the cards on the table and start eliminating the cards that you don't want to include. Don't be conservative in eliminating.

> KISS (keep it simple stupid)

\- [The Front End Manifesto][Manifesto]

### Introducing the ViewThought Case Study

Here's a practical example and a proof of concept. I need a new website for my practice "View Thought" I would like to launch at the end of writing this book. My storyline goes something like this:

> We are a great website design, development and user experience shop. We have tons of experience, have worked with a bunch of different clients who are all happy with our work, and we really care about what we do. We specialize in Ruby on Rails, and we pay special attention to what your users will see. You should hire us! ...or give us a call and learn more.

I immediately can see a few index card entries in my storyline and start indexing everything I can think of. Beside my own ideas though, it's a good practice to do some basic research and see what competitors or similar services are doing with their websites.

TIP: It's a good idea to bookmark a bunch of sites to review and reference throughout the process. It's sometimes helpful to add a simple tally on the bottom of index cards to see how many sites referenced used that particular element:

![][Index Card Reference]

After completing Step 2 here is what my entries look like laid out on a table:

![][Index Before]

I have 200 index cards laid out and grouped as navigation, content, or footer information. As I review I begin to remove components I don't plan to use. I also start to think about where information will be placed. I want to call attention to different parts of the story depending on its relevance and importance to the story. These components I move higher up on the table. Basically I think like a newspaper layout editor.

After evaluating and reorganizing here is what I'm left with:

![][Index After]

Quite a bit less and through the process I really have a great grasp on what my site will look like and how I'm going to start coding, but I need to whittle it down even further since we're going to use the mobile first approach.

> Provide for the mobile experience as a forethought.

\- [The Front End Manifesto][Manifesto]

We need to shed even more, and here's what I'm left with after further elimination:

![][Index Mobile]

And there you have it, the application in its absolute simplest form doing only the things that are most important. From here we can build up to the desktop.

Before we move on there is one thing I noticed myself doing in the exercise that I'm not too crazy about: assuming that there would be a traditional header, body, and footer. Chances are there will be, but I don't like the idea of boxing myself in so early on in the project. My thoughts on this are, "you have to start somewhere," and when I do start coding I can always break free–if it makes better sense.

NOTE: You can use a digital equivalent to index cards like PowerPoint, or even a single sheet of paper (as a list of items), but index cards are best. A pack of 200 index cards sell for under a dollar so don't be afraid to get nitty-gritty with what you define as an information component.

### Alternative Approaches

I find that the process I just described works best for me, but there are other ways to go about the index card exercise. Check out how this design group uses index cards:

- [Responsive Design Case Study][Case Study]

### The Importance of This Exercise

On a final note on index carding, as a front end developer with years of practice, a huge part of me just wants to bypass this exercise aaltogether and start coding (and change things on the fly as I move along). So why don't I?

Experience has shown me that the manual process of labeling index cards and laying them out forces me to reflect and think outside of my coding box. It helps me discover new ideas, visualize and refine the information architecture, and not work in isolation (i.e. include others in the process). I find that by doing the exercise there's just enough chance of a better outcome that it's worth trying.

Prototyping on Paper
--------------------

So with the index card exercise done, the next step in the process is to take the resulting information architecture and create a paper prototype ([sketching][]).

Doing so will help you better define the layout, visualize what the site will look like on a screen, visualize how pages interconnect, and give you plenty of room for trial and error. It also provides you with some additional and inexpensive opportunities for stakeholder input, and further reflection and brainstorming before you begin coding.

There are a number of applications out there that can help you prototype, but I prefer to go old-school with pencil and paper. For presentational purposes you can transfer this exercise to PowerPoint or some other application for prototyping, but don't get bogged down and waste time doing so. Paper is highly portable, can be digitized (scan), requires no electricity or Internet connectivity, can easily be shared with others, and its use is a skill that is common between all stakeholders.

Here are some device mockup resources that will help you sketch:

- [Generated Paper][]
- [Interface Sketch][]
- [UX Sketching And Wireframing Templates For Mobile Projects][Mobile Sketching]

**Step 1**: To begin just simply translate what you indexed in the previous section into what it might look like on a scree, and that's it. There is no Step 2, just a lot of erasing between when you begin and when you end.

Here's what my paper prototype process looks like starting with a blank sheet of paper next to my index cards and ending with a paper prototype:

![][Prototype]

...a well-defined user interface layout for my entire application.

TIP: As you prototype always have an eye on your bookmarked reference websites, and/or some of the [inspirational sites][Appendix 1] listed in the Appendices.

NOTE: For some great examples of how others use paper to prototype checkout:

- [UI & Wireframe Sketches for your Inspiration][Prototyping Examples]

Content
-------

I highly recommend getting real content early on in the development process, preferably before you create wireframes. Nothing can substitute for real content, but unfortunately more times than not you will have to make do without, perhaps a client has not yet delivered it.

### Content Blocks

If you do not have a website's content while architecting, the following article gives a nice overview of how content blocks can be used in situations where content is not known:

- [Content, First?][Content First]

#### Getting Content

Still, it's best to get your content right off the bat, and the following articles will help you do just that:

- [Using Content Templates to Get Your Clients Thinking Content-First][Client Content]
- [Content Templates to the Rescue][Content Templates]

#### Placeholders

As a last resort you can use Lorem Ipsum or dummy images as content placeholders. I've put together a pretty comprehensive list of [placeholder services][Appendix 2] for your benefit in the Appendices. It includes text and image placeholder services.

Although I like to use [Dummy Image][]'s as placeholders, I also keep a 1px x 1px transparent gif, sometimes referred to as a shim, in the `assets/images/fixtures` folder. It can be used to create image placeholders as follows:

    = link_to image_tag('fixtures/shim.gif', :alt => '', :width => '75', :height => '75'), root_path, :title => ''

Don't forget to set the color:

    img
      background-color: gray

Wireframing
-----------

From the exercises above you have absolutely everything you need to start coding with confidence: content, and the site's information architecture and prototype layout are pretty far along at this point.

If your paper prototype is the blueprint, what you code moving forward is a living wireframe. A living wireframe in that when clients, teammates, and/or stakeholders need to review beyond the early exercises, you can send them to a live URL where they can click away and resize all they want.

The wireframe will simulate the actual application, in fact the wireframe will become the application. For you, everything from this point forward is just an iteration in the development process so **revise and release often!**

TIP: Since we are using git, it's a good idea to always use topic branches as you move along the development process. For example:

    C:\Projects\viewthought>git branch
      design-header-blue
      design-header-pic
    * master
      mobile-nav-experiment
      thoughtful-reduction
      viewthought-1
      viewthought-2
      viewthought-3
      wireframe

### From Paper to Browser

**No More Exercises!** At this point it's time to start coding, and after coding my prototypes here is what I have:

![][Wireframe]

![][Laptop]

Pretty bare-bones, but that will soon change.

NOTE: An assumption I make is that you are a proficient enough front end coder that writing basic markup for your wireframe based on the prototypes we just developed is a no-brainer for you. I hope so!

### Wireframing with Susy

In *The Front End Manifesto* we learned how to [install and implement Susy][Chapter 7 - Manifesto]. It's a powerful tool which I strongly recommend you use. Using it will allow you to quickly lay out the content of your application, set breakpoints, and test across different devices until you zero in on the perfect layout for your project.

One feature that will help you wireframe is the grid background tool:

![][Laptop Grid]

These grid guides are very similar to what [Compass offers][], and can be activated by simply adding the following line to your `.container`'s CSS properties:

    .container
      +container
      +susy-grid-background

Using Susy to wireframe, at the end of our information architecting cycle, with our basic content and layouts in place, here's what we're left with across several different devices:

![][Multidevice]

A complete wireframe, that is also responsive across multiple devices through [Susy breakpoints][]. Test it out here:

- http://viewthought-0.herokuapp.com/

Now all that we need to do is make our wireframes look pretty! We will tackle this head beginning with Chapter 2, "[Visual Design for the Nondesigner][Chapter 2]".

NOTE: As front end developers we oftentimes think in terms of boxes. Notice our wireframe is essentially a layout of different content boxes. As we move into design mode [in the next chapter][Chapter 2] we need to completely change how we use our brains.

Just remember, less is more and KISS (Keep It Simple Stupid).

[Manifesto Book]:      https://github.com/maxxiimo/the-front-end-manifesto/blob/master/TOC.md
[Manifesto]:            https://github.com/maxxiimo/the-front-end-manifesto/blob/master/MANIFESTO.md#the-manifesto

[Chapter 2]:           https://github.com/maxxiimo/coding-design/blob/master/chp2-visual-design-for-the-nondesigner.md#visual-design-for-the-nondesigner
[Chapter 6]:           https://github.com/maxxiimo/coding-design/blob/master/chp6-slicing-and-dicing-mockups.md#slicing-and-dicing-mockups

[Chapter 1 - Manifesto]: https://github.com/maxxiimo/the-front-end-manifesto/blob/master/chp1-foundation-markup.md#foundation-markup
[Chapter 3 - Manifesto]: https://github.com/maxxiimo/the-front-end-manifesto/blob/master/chp3-foundation-styles.md#foundation-styles
[Chapter 5 - Manifesto]: https://github.com/maxxiimo/the-front-end-manifesto/blob/master/chp5-mobile-foundation.md#mobile-foundation
[Chapter 7 - Manifesto]: https://github.com/maxxiimo/the-front-end-manifesto/blob/master/chp7-susy.md#susy

[Appendix 1]:           https://github.com/maxxiimo/coding-design/blob/master/appendices.md#appendix-1
[Appendix 2]:           https://github.com/maxxiimo/coding-design/blob/master/appendices.md#appendix-2
[Appendix 3]:           https://github.com/maxxiimo/coding-design/blob/master/appendices.md#appendix-3

[Move People]:          http://hbr.org/web/special-collections/insight/communication/storytelling-that-moves-people
[Jason Santa Maria]:    http://jasonsantamaria.com/

[Chapter 1 Quote]:      https://github.com/maxxiimo/the-front-end-manifesto/blob/master/chp1-foundation-markup.md#foundation-markup
[Wikipedia]:            https://en.wikipedia.org/wiki/Mosaic

[Don't Make Me Think]:  http://www.sensible.com/index.html

[Case Study]:           http://builtbyboon.com/blog/responsive-design-case-study

[sketching]:            http://tympanus.net/codrops/2013/01/29/planning-your-web-design-with-sketches/
[Generated Paper]:      http://generatedpaper.com/en/wireframing
[Interface Sketch]:     http://interfacesketch.tumblr.com/
[Mobile Sketching]:     http://uxdesign.smashingmagazine.com/2012/09/18/free-download-ux-sketching-wireframing-templates-mobile/
[Prototyping Examples]: http://webdesignledger.com/inspiration/ui-wireframe-sketches-for-your-inspiration

[Content First]:        http://alwaystwisted.com/post.php?s=2012-10-13-content-first
[Client Content]:       http://webdesign.tutsplus.com/articles/workflow/using-content-templates-to-get-your-clients-thinking-content-first/
[Content Templates]:    http://alistapart.com/article/content-templates-to-the-rescue
[Dummy Image]:          http://dummyimage.com

[Compass offers]:       http://compass-style.org/reference/compass/layout/grid_background/
[Susy breakpoints]:    https://github.com/maxxiimo/the-front-end-manifesto/blob/master/chp7-susy.md#susy-breakpoints

[Storytelling]:         http://chrismaxwell.com/coding-design/chp-1/storytelling.jpg
[Mosaic]:               http://chrismaxwell.com/coding-design/chp-1/mosaic-800px.gif
[Index Card Reference]: http://chrismaxwell.com/coding-design/chp-1/index-cards/index-card-reference.gif
[Index Before]:         http://chrismaxwell.com/coding-design/chp-1/index-cards/index-cards-before.jpg
[Index After]:          http://chrismaxwell.com/coding-design/chp-1/index-cards/index-cards-after.jpg
[Index Mobile]:         http://chrismaxwell.com/coding-design/chp-1/index-cards/index-cards-mobile.jpg
[Prototype]:            http://chrismaxwell.com/coding-design/chp-1/prototype.jpg
[Wireframe]:            http://chrismaxwell.com/coding-design/chp-1/wireframe/ipad-wireframe.gif
[Laptop]:               http://chrismaxwell.com/coding-design/chp-1/wireframe/laptop-home.gif
[Laptop Grid]:          http://chrismaxwell.com/coding-design/chp-1/wireframe/laptop-home-grid.gif
[Multidevice]:          http://chrismaxwell.com/coding-design/chp-1/wireframe/multidevice.gif
