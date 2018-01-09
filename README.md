
 # Zach and Andrew's blog collab
 
 ## What we *absolutely* need to do:
 
 ### Making the submodules work
 
 At this point, we pretty much *have* to make both `_post`s and `figures` git submodules.  
 
 **Problem**, this means we can't have blog posts use the images in `images`.
 
 **Solution?**: we move the static images used for the blog posts into a subfolder in `figures` called `figures/static_images`. Pretty sure the `knitr` stuff won't delete anything in that subfolder and that putting a subfolder there won't hurt anything, but who knows. Reading a bit more about Jekyll stuff, I'm actually not so sure.
 
 ### Adding double burchill nav bar
 
 We need to get a navbar for the blog posts that scales with a shrinking window width
 
 ## What we definitely *should* do:
 
 ### Come up with a good way of sharing necessary code
 
 Making anything look good and be robust is going to make sharing code necessary.
 
 Here are things we'd want to share and why we'd want to:
 
 * **Basic CSS code/variables (color schemes, etc.)**: If we want to have the individual posts we make have different color schemes that match our websites, it would be dumb not to have these be in a shared repo. If you ever change your color scheme, etc., it would look super dumb not to have it automatically update the blog posts.  
 * **Links in the shared navbar**: Honestly, we almost absolutely need these to be shared. Preferably as liquid variables.
 * **Jekyll/liquid layouts**: if we want to implement color schemes for different authors, we need to share the markdown layouts that do it
 
 ### Make all the posts use different layouts, as determined by author
 
 We need to do something like this on all the posts (or use a sneakier way) that we make so that Jekyll knows to use different color schemes. At most this will just be changing something in the YAML front matter for each post.
 However, I think getting a good working version of this might actually be trickier than we thought.
 
 # Helpful links
 
 * Read through this first: https://jekyllrb.com/docs/configuration/
 * Variables in Jekyll/liquid: https://jekyllrb.com/docs/variables/
 * Custom data in liquid: https://jekyllrb.com/docs/datafiles/
 
 # Action items:
 
 We should divy up what needs to be done.  Here are some preliminary tasks that I've broken down. When you're done with the task, strikethrough the text.
 
 * Make the double navbar: **Andrew?**
 * Test if making a new `.md` post from a `.Rmd` file will erase static images in the `figures` folder: **Andrew?**
 * Get some way to share Liquid data: **Zach**
 * Come up with a system for managing the CSS/layout differences across sites: **Zach**
 
 
 
