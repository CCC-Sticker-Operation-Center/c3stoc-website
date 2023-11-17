+++
title = "How to make your own stickers: A c3stoc guide"
linkTitle = "Sticker Howto"
menu = "sidebar"
weight = 500
+++

As promised during [our talk at Camp](https://media.ccc.de/v/camp2023-57194-from_c3stoc_with_love_3) we are finally releasing our tips and tricks for people who want to start making stickers!

Before we get started:
- we’ve tried to find the right balance between telling you everything you need to know and not drowning you in too much information – if you think we have missed something essential, please [get in touch with us](mailto:exchange@stickeroperation.center)!
- there are more nice tools, good printers and resources than the one we list here – it is always a great idea to ask communities and people around you for advice. Or do some additional research!
- if you have any specific questions, we’re always happy to help you point to an answer :)

## What’s a good sticker motive?

What makes a good sticker design really depends on the message you would like to send, the community it addresses, and where you would like to see it generally. 

### The basics

Usually for Chaos events, stickers are meant to be put on devices like smartphones, laptops, routers, or machines in your hackspace of choice. For those uses, **we have learned a few things that usually *don’t* work well**. They are not absolute rules, we ourselves make exceptions to them:

#### Suff that is just logos

In most cases this is very boring, and makes whatever you stick it on to feel a little more like a billboard. If you would like to promote a project, like git for example, just adding a silly slogan like “just do git” makes the design much more fun, effective and memorable.

#### Plain white backgrounds

This also can make sticker designs look boring, altough there are exceptions to this rule, too. In general, large white areas on stickers tend to look dirty quite quickly.
Another type of stickers that doesn’t always look good is anything printed on transparent background: Most laptops and smartphones these days have a dark surface and the colors of your designs will look grey-ish and dull, except if you can afford a very expensive print with a good white base layer under the motive.

#### Oversized dimensions

People generally want to put stickers on their laptops, smartphones and other devices, and they  usually like to display as many cool stickers as possible. If someone has to decide between one large sticker or ten smaller ones, they’ll usually go with the smaller ones. If your sticker design is too large, it won’t get used that often.

### Inspiration

In order to find out what works, look out for what people often have on their laptops. Here are some examples of what kind of stickers we personally enjoy:

**TODO: insert examples from talk slides here**

If you need more inspiration, consider checking out one of those projects:

- [DevLids](https://devlids.com/)
- [Chaos Sticker Collection](https://mwarning.github.io/chaos-sticker-collection/)
- [Hacker Archive: The Sticker Archive](https://hacker-archive.org/item-set/6601)
- [The Sticker Archive](https://stickerarchive.org) – currently inactive

Another way to start out with a sticker design can be around an impressive, fun, or just cool photograph you or somebody else took at a Chaos event. The “Bundeslichtagentur” design for example builds upon an impressive shot from Chaos Communication Camp that has been published under a Creative Commons license.

[Flickr](https://www.flickr.com/) can be a good place to start, as its search can be fairly well adjusted using filters, for example for the license pictures are published under, or the date the photos have been shot.

Take a look at these searches:

- [Text search for “36c3” without filters](https://www.flickr.com/search/?text=36c3)
- [Text search for “chaos communication camp”, restricted to photos taken in 2019 and published under any Creative Commons license](https://www.flickr.com/search/?text=chaos%20communication%20camp&license=2%2C3%2C4%2C5%2C6%2C9&min_taken_date=1546297200&max_taken_date=1577833199)

The Creative Commons project provides a search as well, if you’d like to cast a wider net: https://search.creativecommons.org/

In any case, wherever you get your pictures, don’t forget to check the license under which it has been published and whether it is a fit for your sticker!

### Taking notes

Sometimes ideas come up as you’re hanging out with friends or fooling around in your hackspace of choice. It is always a good idea to write them down right then and there, as you might forget about them later. Trust us on this one, there are so many stickers we wanted to print and we have forgotten about ;)

## How to create the design

Once you have a design idea, it needs to be made into a graphics file so the printing company can print it for you. There are different tools that can help you with that.

### Software

We usually make stickers using Free and Open Source software. We know there are proprietary tools around, but we can’t really help you with them.

There are broadly two different kinds of graphic files, and most graphics software specializes on one of those. Those are **vector graphics** on the one hand, and **raster graphics** on the other.

**Raster graphics** (bitmap files) are basically what you get when you take a digital photo, or save one of your MS Paint creations. In a simplified way, it contains information about pixels arranged on a 2-dimensional grid, that can be modified individually. This is also what happens when you increase the contrast of a picture or paint a stroke with a “pencil” tool.  
Such files tend to take up more disk space, but if you need to manipulate pictures or even paint digitally, there’s not really a way around them.

![Scan of the “Laber nich, tuwat!” sticker](./tuwat.jpg)

This [sticker design](https://hacker-archive.org/ark:/45490/bfc5nO) is a good example for one where raster graphics are required, since it makes use of an [existing public domain poster](https://en.wikipedia.org/wiki/We_Can_Do_It!).

**Vector graphics** on the other hand contain information about shapes and lines, possibly editable text and information about their color. This means you can scale them as large in size as you want without losing quality, like you would with bitmap files. Vector graphics are great for logos, warning labels, or depicting less complex objects, and have a smaller footprint. 

![notice sign “cat ears must be worn”](./cat-ears.svg)

[This design](https://hacker-archive.org/ark:/45490/bu8YxI) is a good example for a typical vector graphic candidate because it only contains text and simple shapes.

#### Inkscape

Available for: Windows, Linux, macOS

Inkscape is a Free and Open Source tool for vector graphics, and most of the time this is our personal tool of choice. It is primarily made for creating graphics used on the computer, and currently has no means to comfortably create CMYK files for printing without external tools (more on that in "Preparing the design for printing").

Website: https://inkscape.org/

Here are a few good resources for working with Inkscape:

- [YouTube: Logos By Nick](https://www.youtube.com/@LogosByNick)

#### Krita

Available for: Windows, Linux, macOS

Krita is a Free and Open Source painting program focusing on illustrations and comics, texture and matte painters as well as concept art.While its focus is primarily on raster graphics, paintings and drawing on graphical tablets, Krita also offers a suite of vector tools.

Krita supports exporting pixel graphics in CMYK profiles out of the box (not as PDF  or other vector files though).

**TODO: we should list a few resources for learning to use this software here**

#### GIMP (Windows, Linux, macOS)

GIMP (GNU Image Manipulation Program) is a Free raster graphics editor. Contrarily to Krita, it is not designed for drawing. Graphics made with GIMP can then be embedded or referenced in Inkscape or other similar tools. In fact, GIMP advertises itself as part of a workflow next to Inkscape and Scribus.

GIMP supports CMYK color profiles via decomposition, e.g. using the plugins [Separate+](https://web.archive.org/web/20070107080439/http://cue.yellowmagic.info/softwares/separate.html) or [Decompose](https://docs.gimp.org/2.6/en/plug-in-decompose-registered.html) ([see here](https://askubuntu.com/questions/114858/how-to-convert-image-to-cmyk-in-gimp/219611#219611) or in the [Arch Wiki](https://wiki.archlinux.org/title/GIMP/CMYK_support)).

Website: https://www.gimp.org/

(we should list a few resources for learning to use this software here)

### Getting Feedback

Asking for feedback before printing your stickers is *always* a good idea. There are plenty of things one could miss when designing a sticker:

- a typo in the text
- not using an obvious reference
- using text that is ambiguous or can offend people if misinterpreted
- maybe others don’t get it
- or maybe a design element looks bad or weirdly aligned to other people

Your friends also just could have good ideas in general how to improve your design. We do this ourselves as well and always ask a few selected people whether we missed something. Just take manu’s “Cyberpunk” sticker for example. [This](https://github.com/manu-cyber/stickers/blob/master/cyberpunk/cyberpunk-draft.png) is what the original draft looked like, and [this](https://github.com/manu-cyber/stickers/blob/master/cyberpunk/cyberpunk-slim_as-paths.svg) is the final design. Quite the difference, right? Which version looks better to you?

![Initial idea and final version next to each other](./cyberpunk-comparison.png)

## Preparing the design for printing

### Tolerances

Stickers are usually cut into single pieces from a larger sheet during production. The cutting machines always have some of tolerance, and even missing your design by half a millimeter could create an ugly slim strip in the sheet’s color next to it.  
To avoid this from happening, print shops will require you to send them a file that is a little bit larger than your actual design, usually a few millimeters in every direction. Use these few milimeters to continue the background color, pattern, or bitmap in the background of your design -  it doesn’t make sense to leave this space blank in your print file.

Most sticker printers provide templates you can use for your stickers, and sheets explaining the distances and tolerances in detail.

**TODO: add an example here**

Be aware that you *can* overdo this! If you leave too much space around the picture you want to show, the end product will have a large border around the actual design, which will then look small and…weird. It’s happened to us before!

### For vector graphics: Convert text to paths

If you have added text to your design, maybe even in some fancy font you downloaded just for that one sticker. The shop printing it for you might not have that font on their computer: If this is the case, their software will replace it with a more basic font. For this reason, it is good practice not to depend on *any* font at all when exporting it for printing.
We **recommend creating a copy of your file** in which you convert any text into paths. This is a common feature in vector graphics tools like Inkscape. Creating a copy is important to avoid accidentally overwriting the design file, because after the conversion the text cannot be edited anymore.

### CMYK

On digital screens and on printed paper, colors are mixed differently. This is important because we usually design graphics on the computer, using a screen, but the end result is to be printed on some adhesive sheet, using ink.

On screens, colors are created by mixing the colors red, green and blue. For that reason, color values in images are usually stored as a combination of those three colors, each color having an own value that tells the screen how to mix them together using [additive color mixing](https://en.wikipedia.org/wiki/Additive_color). That’s what the RGB color schemes do.

In printing, colors are mixed using different colors, namely cyan, magenta, yellow and black, using [subtractive color mixing](https://en.wikipedia.org/wiki/Subtractive_color). A printer doesn’t know how to mix red, green and blue. When trying to print a file stored with a RGB color scheme, usually it is converted automatically. This *works*, but the result can end up *looking very different to the human eye*. Therefore it is important to either create the file with a CMYK color scheme to begin with, or do the conversion manually, so you can check what the result will look like.

If this brief explanation sounds unclear to you, there fortunately are people who explain it much better than us:

- [Vecteezy: RGB vs. CMYK: What’s the Difference and Which is Better?](https://www.vecteezy.com/blog/design-tips/rgb-vs-cmyk)
- [Wikipedia: CMYK color model](https://en.wikipedia.org/wiki/CMYK_color_model)

#### Conversion using Scribus 

Available for: Windows, Linux, macOS, and more

Scribus can help converting color profiles for PDF files, which are accepted by most printing shops as print input format. It is particularly useful for files created with Inkscape.

Website: https://www.scribus.net/

These are a few ways you can use Scribus to convert a PDF to a CMYK color profile:

- [Logos By Nick (YouTube): Create CMYK Files with Inkscape](https://www.youtube.com/watch?v=RNkWXwk_H8o)  
  This explains how to do it manually, with an easy way to adjust colors if they look different after the conversion. This technique has worked best for us.
- [Color-managed PDF export using Scribus](https://wiki.inkscape.org/wiki/index.php/Release_notes/1.0.1#Color-managed_PDF_export_using_Scribus)  
  If you set Inkscape and Scribus up correctly, you can directly export CMYK PDFs from Inkscape (with some restrictions).
- [Scribus Wiki: Convert RGB imported colors to CMYK](https://wiki.scribus.net/canvas/Convert_RGB_imported_colors_to_CMYK)  
  According to this tutorial you can use scripts with Scribus to automate certain actions. We haven’t tried this, but there is a script for the color profile conversion.

#### Managing profiles using SwatchBooker

Available for: Windows (a bit hacky, but possible), Linux, macOS (if you compile it yourself)

SwatchBooker does not help you with converting image files per se, but it it can be helpful when your design uses a proprietary color profile, which this tool can convert into a format that Scribus or GIMP can use.

Website: http://www.selapa.net/swatchbooker/

Other resources:

- [Scribus Help: Swatchbooker](https://wiki.scribus.net/canvas/Help:Manual_Toolsswatchbooker)

#### Pro-Tip: Official Style Guides

Most official bodies, institutions, political parties, etc. provide style guides for their local branches. These usually also contain font names and exact color codes for both RGB and CMYK. This can come in handy if you’d like to re-use some of those properties.

#### Other solutions or resources

- [Logos By Nick (YouTube): Solving Inkscape's Biggest Problem: CMYK](https://www.youtube.com/watch?v=B_lFwSJePcI)

## Printing

### Quality

 “Indoor stickers” are usually not the right option if you’d like people to put your sickers on their devices. They usually are made of sticky paper that rubs off pretty easily, which is bad for use on laptops. They are also a pain to remove because they rip apart.  
We usually advise to print “outdoor stickers”, which are usually vinyl coated stickers. 90µ is a good thickness if you don’t want your sticker to look very cheap (and break in sticker boxes).

Finding the right printing quality for your stickers takes a bit of trial and error to figure out. Most print shops offer samples for free (or really cheap), so make use of that to check the quality.

If you have the budget or want to make a small but special batch, many print shops offer special prints, for example on glitter, metallic or holographic foil, or with free form “die” or ”kiss” cut, among many other fun options.

### Quantity

How many is a good number to get? Well, that varies.

Generally a larger amount gets a better price per piece. If your design is a project sticker for example, which will not go obsolete quickly, or a joke that has been around for years in your community, it makes sense to make use of that. For specific, time limited campaigns or stickers that feature reactions to current events, you will probably not need as many.

If you’re going to a larger event like Camp or Congress, less than a thousand is not a lot of stickers – just think about how many people attend the event(s) you want to distribute your designs at!

### Where to order prints

We try to avoid advertising print shops for sticker printing, simply because that’s a very individual thing. Also, we are based in Germany and lack knowledge about options available in other countries. A quick web search reveals plenty of options, and we encourage you to ask around in your community for experiences.

That said, there are two options (in Germany) we can’t say anything bad about:

- [stickma.de](https://www.stickma.de/)
- [wir-machen-druck.de](https://www.wir-machen-druck.de/)

Also, we’ve never worked with them, but as we know a lot of people like the Github-Style prints: If that’s what you’re looking for, have a look at Stickermule!

## Sticker distribution

### In person

Take your stickers with you to events or when you visit locations like hackspaces and other cultural establishments. No location or event is to small to share stickers, and especially hackspaces usually curate a sticker box for such occasions. So do most Chaos and other nerd events.

If no sticker box is to be found, you can ask the organizers whether you can set one up. Large flat boxes are the best ones to use. Maybe you can improvise from some box that would otherwise been throw away. If the event does have catering of some sort, you could ask in the kitchen. If you can find a flat plastic box, that is the best option we can recommend, as stickers tend to get stuck in the folds at the bottom of paper boxes. 

At larger events, like Camp or Congress we try to help by organizing infrastructure for distribution, so you don’t have to run all over the place to regularly put your stickers into different boxes. Although you can do that if you have the time—it can be quite fun.  
The infrastructure we set up depends on the event, our capacities and those of other volunteers. At  the last Congress [Chaos Post](https://chaospost.de/) helped us with distribution, which was great. When this is possible we can have one central drop-off-point for you, from which multiple boxes will be filled. We recommend checking our website and/or our Mastodon account in the weeks before Chaos events to see if we’re planning anything!

Last but not least, some of your friends are probably happy to help you with distribution as well, so we recommend giving them more than one ;)

#### Sticker box etiquette

**Do not flood sticker boxes with masses of stickers with the same design!** Add them in appropriate amounts and take the rest with you for later. Note that different people might have different ideas of what an appropriate amount is.

It is generally a good idea to see what the sticker box looks like, and adapt the amount of stickers you add to what’s already there.  
Are people actively sorting it, or are there stacks with different designs around it? Then add a stack of yours there instead of throwing them in the box.  
Is it a really large box that contains lots of stickers with the same 4-5 designs, and nobody is sorting it? It’s probably okay to add a bunch of yours to the mix then, but please make sure it is still in a reasonable amount.

### Digital

After getting your design printed on a sticker, consider publishing the source file (the SVG for instance, not only the file you sent to the print shop), so others can re-print, remix, or improve on the design. Or just so it doesn’t get lost.  
You can do that for example by putting it into a public git repository and release it under a license like [Creative Commons](https://creativecommons.org/share-your-work/cclicenses/) for example. You just have to add the license text in a file next to it, and maybe describe it in a readme file. Some git platforms will even do that for you.

Alternatively, you can consider submitting it to one or more of these projects collecting such designs:

- [Chaos Sticker Collection](https://mwarning.github.io/chaos-sticker-collection/) (make sure your design uses a free license)
- [Hacker Archive](https://hacker-archive.org/contribute) (also keeps non-free designs)

Oh, and of course: We’d be super happy to see your design! Share it with us on chaos.social, or say hi at Chaos events! We’re looking forward to your creativity :D
