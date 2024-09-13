# The Mission X Brief

is enormous, but we need to pick our sections to help us organise and create a scaffold around.

Before anything else, please open up the directory:
<img src="assets/images/directory.png">

OK so here's some things to remember:

## A. General stuff

### Don't worry too much about the CSS.

... because the CSS we'll need is already outlined in the Adobe XD document:

https://xd.adobe.com/view/6f52b708-fde0-4967-bdea-98a46169b9b1-3a01/specs/

<img src="/assets/images/adobe-xd-screencap.png">

To have a look for yourself:

1. click any element on any slide (even the text bits)
2. hit the </> button on the right edge sidebar
3. behold the pre-done CSS and other bits and bobs on the right side.

### Pick a colour, then focus only on the stuff in that colour.

Don't get caught up in the size of the project or the pieces that you can't 'see'. Either it's _nobody's section_ (which are uncoloured bits in the miro board), or it's _somebody else's section_.

## B. Key take-aways for each colour - quick skim if you want to see what you might be interested in (the colours are not in the design brief, but they're used to represent each section on the miro board)

### 1. <span color="#FAC710">Yellow<span> - Home & Log-in/Sign-up (Brief page 5, near the bottom)

1. _Home_ is our ground floor webpage. There's some buttons that cycle through what's displayed near the bottom of the page&mdash;

<img src="/assets/images/main-buttons.png">

&mdash;and some RWD work to be done:

<img src="/assets/images/main-page-icons.png">

These icons need to go from horizontal on desk devices to vertical on mobile.

2. _Log-in/Sign-up_ is neat. So yeah, click this link:

https://xd.adobe.com/view/6f52b708-fde0-4967-bdea-98a46169b9b1-3a01/?fullscreen

and click the magenta (pink? rose? idk) 'Sign Up' button. Container that renders over the main page, blurs everything else, and changes content depending on if you click 'LOG IN' or 'SIGN UP', either in the student or teacher section. Very spiffy, you will feel so much satisfaction coding that.

### 2. <span color="#6DE833">Green<span> - Project Library & Student Profile (Brief page 10)

1. _Project Library_ has two major parts. Apparently, the content filters 'can be created using SQL queries in the backend'. Those filters have three tiers: difficulty; 'free' & 'subscription' content; and this thing:

<img src="assets/images/project-library-filter.png>

At first blush it'll be a lot of lining classes up. The 'Introduction' slide is actually just a big link to _Student Dashboard_ (more on that later, or skip to it using the directory). The other big part would be the project slides themselves. Nice chunky flex-box stuff for you. Fun part is, we get to decide which projects are free, sub-only, their difficulty levels, all those other filter categories. The brief doesn't specify which is which, and we need at least 3 to display & filter correctly.

Finally, _Project Library_ looks slightly different if user = student vs if user = teacher, but that part's not a big deal. That and everything else is just buttons and anchor tags.

2. _Student Profile_ a mostly static webpage. If you're working <span color="#6DE833">Green<span>, wait for whoever's working on the Home page to finish their header and footer, because you can just copy that part of their homework. However, looks like it will need to draw information from a database, so dynamic code is a must. Otherwise, just a bunch of buttons.

### 3. <span color="#F0CACA">Pink<span> - The Project Builder aka 'Learning Objectives', 'Instructions', 'Video Tutorial', and'Make Project' (Brief page 11, but the "Submit Project" section on page 12 is not part of this category. See Orange section below)

'The Project Builder page is the main workbench for students.' It looks chunky, but sink your teeth in and it's not too substantial. Kinda like pavlova, you know? Mmmm, pavlova. Also, the "Submit Project" part is somebody else's job, so say hi to them once your work's done so you can embed their work into yours.

1. _Learning Objectives_ has this neat sidebar: it's collapsible!

<img src="assets/images/workbench-sidebar.png>

It also has these buttons, one of which has conditional statement requirements:

<img src="assets/images/workbench-ribbon.png>

2. _Instructions, Video Tutorial, & Make Project_ has large portions of the page just grabbing pre-existing content (HTML, pics, video) from a database and rendering it onto the screen. Easy (like eating a pavlova). Looks like once you've got the UI sorted and your code is capable of pulling correctly from a database, you're golden. Beyond that, it's a bunch of buttons.

### 4. <span color="#D99239">Orange<span> - Submit Project (Brief page 12) & Project Submissions (not explicity detailed on brief\*)

1. _Submit Project_ can be treated as a container nested within the wider Pink section detailed above, so once you're done with this part be sure to say hi to whoever's working on Pink so they can pop your container in there.

Main focus is a big button that, when clicked, calls a function that grabs a screenshot, attaches a bunch of information to it about when it was taken, then saves it as a URL in the backend. Looks like you'll need to study this as an example component of how that can work: https://github.com/Mission-Ready/MissionX-Screenshot-Upload. Look, I've done my best to be mostly neutral, but this part looks complicated. Hopefully someone can correct me if I'm wrong, but this is what the experts call a 'big learning opportunity'.

2. _Project Submissions_ is the other side. Grabs those URLs from the database then presents them to the teacher as a list on the page with thumbnails which the teacher can enlarge into the full photo. Each submission gets a checkbox to allow the teacher to affect more than one submission with the pièce de résistance, a '✔️MARK AS COMPLETED PROJECT' button. There is no 'DELETE ALL'. That would be just mean.

### 5. <span color="#12CDD4">Cyan<span>
