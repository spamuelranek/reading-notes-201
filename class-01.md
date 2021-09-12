# HYPER TEXT MARKUP LANGUAGE AND Structure

## Why **Structure**? (pp.12-39)
Nave: Don't all words of power(WOP) work equally well?
Sage: WOP work well when constructed correctly. Often they are built on top of each other and it makes them even more powerful.
Nave: Where do I start then?
Sage: The **structure** of a single spell(web page). You need to understand each piece of structure is a bin that holds things in it. 
- ``` html
    <html>
        <head>
        </head>
        <body>
        <header>
        </header>
        <main>
        </main>
        </body>
    </html>  ```
    You can see how the bin has two handles(tags). The opening one and the closing one (one with the /). The whole bin is the binding of *Element* s. These handles are also interesting.
- Most come in pairs as described:
 - '<p></p>' the handles have small alligators called into existence to hold each handle. They are always eating toward the handle. 
 - '<p lang = "en-us"></p>' the handles also come in different flavors for the alligators. The 'lang' tells us what change in flavor *(Attribute Name)* and the '"en-us"' tells us by how much *(Attribute Value)*. 
- The Structure shown above has specific parts
    - '<html></html>' helps everyone know what language you will be conjuring in
    - '<head></head>' is a bin that holds meta-spell information. Title of the spell as seen by the demons that it summons. It may hold other information that is pertinent but not for the performance of the spell.
    - '<body></body>' is the bin that contains every thing you want to yell, whisper, swirl, or boil.
    - '<header></header> a bin to help set a mood. Good place for calling attention to the gods above or below

#### Extra Markup (pp.176-199)
Nave: This seems basically a skeleton. Like a animal. It seems there is still much I need to know. Is there ways to identify like an individual rib. Like they are all ribs but maybe the spell calls for specifically the top right one.
Sage: A wise investitgation. Yes. One of the flavor changes (Attribute Name) you can do to the handles is give it an unique scent( id ).
 - '<p id = "salamanderToeright"></p>' 
 - This is for truly unique items in the spell, but if you would like to group either specific items or parts together use sparlke dust( class ).
 - '<p class = "catStuff"></p>'
 Nave: For the presentation of these bins are there any visual things I need to keep in mind?
 Sage: Yes.
 |Type of Element|Specifics of type| Examples| Tag to set items as element|
 |Block Level | Element will always start on a new line| '<h1>,<p>,<ul>,<li>'| '<div>' |
 |Inline | Element will always contnue on the same line as neighboring elements| '<a>,<b>,<em>,<img>| '<span>'|
 Nave: That is impressive that you can just speak a table of information in to being right in front of me. WOPs are increadible. Is there a way to punch a hole in this table to have another spell work with in it?
 Sage: Aye, It be the Wayof the Eye('<iframe>'). This one requires knowing the other spell( *src* ) and how much space you want to have it take up on your spell( *height, width* ).
 Nave: Inside the '<head>' bin, what other can I store in there?
 Sage: Inside the '<meta>' bin fits well. The flavors are:
- description
  - small explainer of page used by search imps(search engines)
- keywords
 - words people will tell teh search imp to look for
- robots
 - helps describes how and if search imps should look at your spell
- author
 - talks about you
- pragma
 - prevents owner of the return imp making a local copy of the spell
- expires
 - can set time for the spell to self-destruct

#### Layout (pp.428-451)
Nave: Has the structure of the WOP always been the same?
Sage: No. They continue to grow and adapt and work to be more inclusive of the people that can practice the arcane arts. Previously '<div>' handle was used for all block separations in a spell. But the ones we spoke of ('<header>, <body>, <section>, <article>,<nav>,<footer>') are part of those changes.

#### Process and Design (pp.452-475)
Nave: I think I have the basics. I am ready to make my first spell
Sage: Good. There is a suggested process to take you from your idea to a final project.
1. Start with questions
 - who is coming to my site?
 - what information are they looking for?
2. Build a site map
 - make each page a location on a flowchart relative to each other
 - make sure the groupings make sense for a user
3. Wireframe a set up
 - build a visual repersentation of each page
 - does not need to be pretty
 - needs to be able to convey visual structure of each page
4. Use Visual Heirarchy structures
 - use color, font, size to differentiate information
 - use these same things to highlight information
 - group things in ways that general information can be pulled the collective

 #### The ABC of Programming (pp.11-52) A/B
 Nave: I have built the structure but how do i get it to do something?
 Sage: mmm...A much more complex question. What do you mean?
 Nave: I want to have my spell steal names of those that cast it.
 Sage: I will have to give you the ground up for Actovatrix( javascript ).
 Nave: What bin (html) do i need to fill up to make it go?
 Sage: These are not bins. These are the whispers we say to manipulate the bins. Actovatrix uses specific descriptions of these bins. The spell can only look to what is containted with in it. It knows not of the world as we see it.
 Nave: It only knows the bins I have created for it?
 Sage: Precisely. It knows these bins and the flavors of those bins. The spell can be written in such a way that when parts of those bins are "full" in certain ways it will say a whisper.
 Nave: What if this is on someone's scrying glass(Web Broswer) or a report from a retrun imp?
 Sage: Worry not, most spells are already desigined to be effective on the scrying glass by using a Shifter( HTML Mark up). It helps the the scrying glass to see each bin in a way that it understands. Then your whispers work best on the bins of the end user.

 #### C
 Nave: How do I put it all together?
 Sage: Take your full built skeleton(HTML), your creations skin(CSS), and all the organs(JavaScript) and link them. People should not see the working parts. That would be bad. It would mean something is sticking out from the inside. Even if they look at the just below the skin.  

[Knowledge Base](README.md)
