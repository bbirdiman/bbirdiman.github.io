# markdown considered harmful

## (or perhaps just a loved but irritating old uncle)

### by bowerbird intelligentleman







## table of contents

<a href="#markdown_considered_harmful"> markdown considered harmful </a>
<a href="#table_of_contents"> table of contents </a>
<a href="#preface"> preface </a>
<a href="#the_screed"> the screed </a>
<a href="#the_ugly"> the ugly </a>
<a href="#the_bad"> the bad </a>
<a href="#the_good"> the good </a>
<a href="#john_macfarlane"> john macfarlane </a>
<a href="#fletcher_penney"> fletcher penney </a>
<a href="#brett_terpstra"> brett terpstra </a>
<a href="#markdown’s_future"> markdown’s future </a>
<a href="#a_few_more_things"> a few more things </a>
<a href="#light-markup"> light-markup </a>
<a href="#restructured-text"> restructured-text </a>
<a href="#ascii-doc"> ascii-doc </a>
<a href="#textile"> textile </a>
<a href="#markdown’s_arrival"> markdown’s arrival </a>
<a href="#markdown_in_public"> markdown in public </a>
<a href="#i.o.s._apps"> i.o.s. apps </a>
<a href="#draftin_dot_com"> draftin dot com </a>
<a href="#editorially"> editorially </a>
<a href="#ghost"> ghost </a>
<a href="#wordpress"> wordpress </a>
<a href="#dillinger"> dillinger </a>
<a href="#simplenote"> simplenote </a>
<a href="#long-form_light-markup"> long-form light-markup </a>
<a href="#leanpub"> leanpub </a>
<a href="#scrivener"> scrivener </a>
<a href="#texts_dot_app"> texts dot app </a>
<a href="#textastic"> textastic </a>
<a href="#zen_markup_language"> zen markup language </a>
<a href="#summary"> summary </a>














## preface


ok, first of all, you know that the “considered harmful” expression is an exercise in silly titles, right?, just a bit of humorous hyperbole.

and, as i have just demonstrated -- right in my opening paragraph -- i am a person who is quite willing -- eager? -- to state the obvious.

so bear with me.

because though i will be discussing a raft of very real problems with it, i still do not really think markdown could ever be “considered harmful”.

yes, there are lots of problems with it, and its development _is_ troubled. and i’m gonna be frank about that.

but still, i _love_ markdown. a lot! and if you don’t, we’ll have to fight.

in particular, if you are one of those meatheads saying “markdown sucks, and i don’t understand why people can’t just write in .html, like i do”, and you came for a spiel which you expected would validate your opinion, then you’ll want to stop reading now, as i have no tolerance for such idiocy.

any writer worth his or her salt knows that writing is hard enough, _without_ dodging all that tag-bracket crap in your text, disrupting your thoughts, every quote-mark and contraction creating an endless parade of needless ampersand distractions.

so if you’ve somehow learned to ignore garbage strewn about your living-room, well, good for you, meathead, but that doesn’t mean that now everyone else has to tolerate it in our living-rooms.

so just walk away now, while you can, so i don’t have to ridicule you further.

 _#i/mean/it/just/walk/away/and/do/it/now_

because i love markdown.

and, later, i will explain why, in detail, with some history and some analysis.

but hey, i know you internet kids. i used a “considered harmful” title, and you jumped on that link-bait, so the last thing i can do now is to bait-and-switch by making you first sit through some history lesson or wallow through reasoned discourse.

no sir, you came for a screed, and if i do not give it to you, _now,_ you might take it out on me, i know.

indeed, you probably already think that this is getting too long-winded. (assuming you even made it this far.)

so, if you’re one of _those_ people, here’s your meaty list of shit, quick!, for your tl;dr attention-deficit mindset.







## the screed


here’s “the good, the bad, and the ugly”, in _reverse_ order, to end on a positive, where i can continue on from that point to embark on a more thoughtful review.

the reflective readers can stick around for the whole thing, and think.

while the accident-lurkers among you can speed off to seek your next thrill.







## the ugly


for the truly ugly parts of markdown, we’ll need to start at the very outset.

gruber’s original spec for markdown is _too_ _primitive_ for today’s .html needs.

to give just one little example of that, it doesn’t automatically formulate the id tags needed on headers in order to have internal links in a document _or_ to allow deep-linking from the outside.

given the web of today, that would be something that made it a non-starter. heck, even in the web of 2003, that _should_ have made it a non-starter.

there are other omissions like that too.

moreover, extensive usage showed us “classic” markdown is plagued by more than its fair share of “ambiguities” in the features which _are_ included, because it’s insufficiently complete.

and last but not least, there are even inconsistent “edge-cases”, where gruber’s descriptions of the “spec” contradict themselves.

of course, what can you expect from a perl script filled with reg-ex crap, which has seen one (count ‘em -- 1!) update in 10 years? yep, exactly that.

so first, classic markdown doesn’t do _enough_ stuff.

second, it’s too silent on stuff it _does_ do, when it should be explaining it clearly.

and third, even when it does explain, inconsistent edge-cases pop up.

putting it starkly, gruber-markdown simply ain’t sufficient for prime-time. it has just got too many shortcomings and problems.

i mean, fine, if all you’re using it for is the comments on your web-site, or to write your 4-paragraph blog posts; these shortcomings will not bother you.

but once you are doing real documents, you will experience the burn, you will.

because the gruber-classic-markdown is _lame._

to realize this is what people _mean_ with generic references to “markdown” -- nearly every “help” link goes to gruber’s page -- is enough to make you cry in despair.

whenever i hear someone say “markdown” to describe what they used for a text, and they don’t name a specific flavor, when i know they’ve clearly used one, because generic markdown just cannot do the type of stuff they have done, it reminds me of relatives having web problems, so i ask them which browser they’re in, and they say “the internet”.

the fact that few people know about the gruber-markdown shortcomings, or the wide variety of extensions, is because they use markdown only in the most superficial of ways.

(this is also why you hear them repeat the lie that “it only takes 5 minutes to learn all about markdown”; yeah, right.)

and gruber has reinforced this notion that “markdown” is a superficial tool, insisting that, as far as he’s concerned, his version of it is a finished product.

um, gee, ok, it might well be “finished”, but it’s nonetheless _badly_ _incomplete._ far too primitive for what we need today.

and that’s the ugliest thing about markdown. the guy that gets all the credit for “inventing” it doesn’t even mind that it’s so damn primitive. it’s as if he cannot even hear himself praising apple for its “constant iteration toward an even better product.” which is terribly ironic.







## the bad


even if it’s “good enough for gruber”, the rest of the world has needs which often go beyond the mere superficial, so classic-markdown is _not_ “enough”.

plus it’s only natural that people will improve any tool to get what they need.

the first wave of people to embrace markdown use was comprised by coders who simply ported gruber’s perl script to their particular language compiler, be it php, python, ruby, or whatever.

but these individual developers also “extended” markdown, to improve on it -- for their own use and viewpoint -- by addressing its shortcomings, and were usually fairly successful at that.

it’s typically quite easy enough to invent a light-markup rule that will accomplish the outcome that you want, whatever that outcome might be. and the shortcut is pretty easy for you to remember, and use consistently. so people threw in whatever they needed.

some of them added just a couple things. others put in a full range of new stuff.

each person invented their own “flavor”.

every developer solved a different set of problems, and did it a different way.

well, of course, as you’d expect, soon the various reformulations grew terribly out-of-sync with one another.

the flavors clashed. they clashed badly.

not only did they do different things in different ways, they often did the same thing different ways, and different things in the same way. so, total chaos.

for a long time, few people noticed it, and even fewer minded. but as needs to transport markdown files from one system into another started to become common, these incompatibilities grew bothersome.

so they became difficult to ignore, and thus began to be grudgingly acknowledged, then recognized as serious, until finally, they were finally noted across the board by everybody with extensive experience.

so while developers plugged big holes in gruber’s too-primitive classic-markdown, they have also exacerbated problems with the inconsistencies, to the degree that nobody is certain what “markdown” does now.

so, if you feel that you have a certainty, you should prepare yourself for the shock -- if you need to use some other flavor -- when it doesn’t act like you think it will.

further, because of the markdown flavors doing different things, and differently, the underlying “mental model” has grown to be badly fragmented, so any reliance on “what seems intuitive” is no longer a dependable guide on what will happen.

this shattering of the “intuitive” asset might prove -- in the long run -- to be the most serious problem of all of them.

moreover, despite continuous calls for a “standardization” of markdown, the various developers all have a stake in their own personal vision and product, therefore, none wants to “standardize” his flavor out of its very existence by making it “redundant” with another one.

their recalcitrance has become so firm that they don’t even bother to debate new proposals in dialog or discussion; they simply fail to respond in any way. which is probably good, in that it saves everyone lots of wasted time and hope; but it won’t, you know, yield a solution.

so we have these problems being caused by this plethora of developers iterating -- separately -- around a shallow core, fragmenting a pathetic entity too weak to stand by itself independent of them, and now they are resisting any solution to this big jigsaw puzzle because each one is holding tightly to his own little piece, reluctant to sacrifice it to another player.

and thus the problems are now intractable.

it’s worth noting that gruber has thus far stared down all attempts to fix this shit. perhaps recognizing the futility of _any_ chance of consensus, he will not even try. he just continues to insist _he_ is happy.

meaning there is nothing on the horizon. no white knight; nix on prince charming.

so, as the uptake for markdown increases, a ton of users will get bit in their butts. and the more that come in, the more that will experience a need to cross flavors, and find themselves bitten in their butts.

so even as the positive affect climbs up, as more and more people stumble upon the appeal of light-markup and come to love it, so too will the negative affect tag along, correlated strongly; and that, my friends, is the state we label “severe ambivalence.”

probably not the zone you want to be in.

but markdown has been tied to the tracks, and the only thing coming now is a train.

it is inevitable. the only way that you can _not_ _see_ _it_ is to close your eyes.

it’s a good thing world peace does not hang in the balance. “just documents.”







## the good


now that we’ve done “ugly” and “bad”, we can move on to “the good”. hooray!

this is where all the people who came for a rant can leave now. see ya later!

when we consider the good news for markdown, we note that it is now showing up _everywhere._ and the signs are that it’ll keep growing, possibly even faster than its current rate.

the cause of light-markup is well-served!

so let’s point our telescope at three stars shining most brightly up in markdown’s sky.







## john macfarlane


“pandoc” -- <http://johnmacfarlane.net/pandoc> -- is a tool that converts between a bunch of text-file-formats and systems, _including_ markdown, so it can be extremely useful, and is one of the few brighter spots in this mix.

one part of the f.a.q. on the “pandoc” site documents the many inconsistencies between _some_ of the many various markdown variants -- but not all, as new implementations are cropping up regularly, with new wrinkles -- while another section over there considers: “what are some big questions that markdown’s specification does not answer?” thus, if you were wondering whether i maybe “exaggerated” all the glitches, as a stunt for the lurkers, you should check out the full array of stuff.

(and you will realize that i _chose_ to _not_ throw meat to all those rambunctious coyotes, or i would have pointed to this page up above, and detailed it all in an excruciating manner.)

> <http://johnmacfarlane.net/babelmark2/faq.html>

the f.a.q. section also has a web-app which lets you input real-life markdown fragments to each of the various flavors to learn what each one actually delivers for that fragment. so much handier than installing all of them.

again, if it’s important in any way for you to know the state of uncertainties in the markdown arena these days, you absolutely must definitely delve into details there, so you’ll grasp the scope of the nightmare.

or if you’re _experiencing_ glitches in a markdown file, this is a great resource to help you debug the crappiness. and if you come up with something new, file a report.

john macfarlane is the berkeley professor who makes the _free_ _and_ _open_ “pandoc”, meaning he has donated a boatload of time to the cause, and that deserves recognition.

so if you need conversions for other formats for markdown to be viable in your workflow, pandoc is the _first_ tool you should review.

“pandoc” has proven itself, over and over, as being a tool that is extremely valuable.







## fletcher penney


likewise with “multimarkdown composer” as a tool that’s proven it is very valuable.

> <http://multimarkdown.com>

“composer” is a text-editor purpose-built for “multimarkdown”, by fletcher penney; he is the creator of “multimarkdown”, so integration of the two is nice and tight.

“multimarkdown” is the markdown variant which is the most powerful of all of ‘em, so it was already the leader of that pack, even before fletcher programmed “composer”.

“composer” is a mac text-editor app that funnels its text through “multimarkdown” to create output, primarily in .html form (the typical output of markdown flavors), but now also as .rtf, and .pdf, and .epub.

“multimarkdown” format is _free,_ but -- to justify all the time spent coding it -- “composer” is a $12 commercial mac product, readily available over at the mac app-store.

because “composer” is geared specifically toward “multimarkdown”, it makes it easy to write and edit your text in that format.

for instance, let’s say that you are making an ordered list, and you have just finished typing an item there. when you hit _enter,_ “composer” automatically inserts the coding to indicate the start of the next list item, so you can just start typing away at that. hit _enter_ at the end of that, and you’re ready for the next item. at the end, press _enter_ twice in a row, and the app knows that the empty item signals that you’re done with the list, so it deletes that empty item. it sounds like a little thing, and, by itself, it is. but when it gets combined with many such little helpers, it all adds up, and you will find you get used to them quite quickly.

as “multimarkdown” is the best variant -- with more power than other flavors -- and holds a slight edge over the others, i once thought that his “composer” would allow fletcher to break clean from the pack of markdown flavors and take a huge lead (since none of those other flavors had the benefit of an editor specialized for them), thus resolving the inconsistency log-jam, by virtue of “multimarkdown” becoming the “de facto default” markdown flavor standard.

but fletcher’s initial updates came slowly; “multimarkdown” is still leading the pack of all the markdown flavors, but it hasn’t broken out to the point that they all quit.

and part of the reason is that the other markdown flavors soon received one of the most significant advantages “composer” briefly had to itself -- a live preview.

and for that development, behold the third star in our markdown firmament.







## brett terpstra


the best thing for markdown at this time -- no doubt about it -- is brett terpstra, who created the markdown-live-preview app for mac desktops that is called “marked”.

> <http://marked2app.com>

“marked” is also a $12 commercial mac app.

it lets you use your favorite text-editor -- any app that saves a plain-text file -- to write your markdown-formatted text-file, and then “marked” will monitor that file being _saved_; when it discerns a new save, “marked” converts the file, in real time, to show you the resultant .html, _live,_ side-by-side next to your text-editor app.

this instant preview -- _while_ you are actively editing -- is quite informative, and the fact that you can pair “marked” with _any_ text-editor makes it special.

“marked” does nothing that will give your text-editor app any special “markdown mojo” (you’ll have to apply things “manually”), so it’s not quite as good as “composer”, but a live-preview is worth $12 by itself. (especially when you’re editing “by hand”.)

i have long held that the side-by-side interface is a vitally-important factor, when using a light-markup system, since it creates a distinct mental separation between the _input_ (plain-ascii text) and the _output_ (nicely-formatted rendering).

input in one window, output in the other.

it keeps everything straight in your head.

this gets at one of the crucial topics in discussing text-editing these days, especially pertaining to the web and a struggle to ditch ms-word, to make text “semantic”, not “presentational”.

since most of our users grew up using word-processors, their modus operandi is to “make it look good”, which doesn’t translate so well to our new web world, where output displays aren’t as fixed as ink put on an 8.5*11-inch sheet of paper.

to emulate the w.y.s.i.w.y.g. approach which our users have fondly embraced, in a decades-long love-affair with the wonderful miracle of word-processors, some coders have strived to develop a “hybrid” light-markup interface which will _combine_ the input and the output -- smooshes both into a single window -- but i firmly believe that will only cause confusion for the users. (not to mention for the designers of such an interface.)

in my strong and longly-held opinion, a “combination model” is the _worst_ possible approach we could be taking, precisely since it confuses the issue.

no, we should do exactly the opposite!

we need users to understand that input and output are fully separate, and also that the only way they’ll get the output they want is to make edits to the input.

this embraces the strong user desire to “make it look right”, while constraining their edits to ones accurately reflecting the text’s underlying structural integrity.

in other words, if the _only_ way you can “make it look right” (on the “output” side) is to tag it correctly, i.e., structurally, (on the “input” side), you’ll tag it right!

the secret answer to that hard question of “how do we get people to stop making it look right?” is “stop trying to make them, and take advantage of their inclination”.

but the only way to invoke that mentality is for us to use a side-by-side interface, so the input and output remain separate; not just on the screen, but in your mind!

the distinction is especially crucial when you are _learning_ markdown, but it’s also still valuable when you are _writing_ it, since using the live preview window while you are working gives immediate feedback whenever you have tagged something wrong.

and i firmly believe that if you experiment with a 2-up live-preview method of working, you will rapidly come to see what i mean.

so i cannot recommend “marked” enough -- especially if you’re _learning_ markdown!

plus brett just came out with version 2, which offers a brand-new slew of tools (e.g., one to highlight word-repetition) that’ll be of good utility to most writers:

> <http://marked2app.com>

nor is “marked” the first trip to the rodeo for brett, either; he is an old hand there.

brett has also scripted several mac-os “services” for lots of markdown tasks. matter of fact, go see all his “projects”:

> <http://brettterpstra.com/projects>

but of special interest to markdown, see the section for “markdown-service-tools”.

and, in particular, see this one; brett has a web-app, over at <http://markdownrules.com>, which offers converters that will translate both directions between markdown and .html.

so say there is a web-page and you’d like to have its text in markdown format? easy! just put the u.r.l. into brett’s converter:

> <http://markdownrules.com>

brett also scripted a “bulls-eye” plug-in, where you can select text from a web-page and then have that converted into markdown.

and brett’s projects go on and on and on.

so heck yeah, go see everything from brett. odds are you will find more than one thing that helps you in your particular workflow.

***

so, in this “good” section for markdown, i’ve featured the work of three individuals, all talented, all working very hard, and all contributing great stuff to the community of markdown users. big thanks to all three!

there are, of course, _many_ people who have made contributions, in the past and continuing into the current-day, but these three individuals went far beyond the call.

after the next section, on the future, i’ll talk about some other markdown-related apps that you should be familiar with today, and highlight a couple other things to consider.

but for now, let’s look ahead a little bit.







## markdown’s future


so, next, we look to markdown’s future.

as more and more people start using markdown in more places to accomplish more things, they’re bound to experience the problems that i’ve discussed here, and they will then realize these infrastructural shortcomings.

so -- right along with inevitable growth -- markdown will have an equally-inevitable concurrent dissatisfaction that also grows.

which will be kind of crappy for markdown.

yet still, at the same time, markdown will continue to do the tasks perfectly well on most of those things people use it for now, such as blog pieces, comments, and the like.

when your text has under 11 paragraphs, and doesn’t really need much formatting, like a github read-me, markdown is fine.

and even if you’re doing a long document, with loads of styling, markdown will work well enough for a clear majority of needs.

as living proof of this, many apps now do their manuals in markdown, and handling of these not-all-that-simple documents is done quickly and easily, without problems.

it’s not true of gruber-classic-markdown, but most of the extended flavors can now give whatever you need for many documents. multimarkdown in particular is full-serve.

and you will not experience many problems _provided_ you stay with the same flavor.

but you have to stay with the same flavor.

it’s only when you think you can painlessly switch from one flavor to some other flavor that you might well be in for a big surprise.

so ensure, before you start your document, that the flavor you’re using can handle it.

because you don’t want to have to switch.

but even a switch won’t be insurmountable.

if you do find you have to change flavors, a quality-control pass on the new output should be enough to see incompatibilities, as long as it’s a sharp-eyed close review.

(very sharp-eyed. very close. important.)

but you _should_ be doing quality-control often anyway, as a best-practice workflow.

in other words, as long as you are properly sensitized to a real possibility of glitches, they might cost you some time and energy, yes, but it’s unlikely they’ll bite you in the butt.

it is only if you do not have the wisdom or experience that glitches hide in markdown that you’ll be surprised _when_ they bite. (there’s no _if_ about it; they _will_ bite.)

still, their bite is probably no worse than the “considered harmful” bark i’ve just made, in my title here, so don’t worry, you’ll live.







## a few more things


so let’s talk about a few more things, in terms of how we got to our present-day state with markdown. this will be kind of a history lesson.

first of all, as you can probably tell, no, sincerely, i do not hate markdown.

to the contrary, in _many_ ways, i’m a long-time fan of markdown. and i’ll make sure you know that.







## light-markup


heck, i loved markdown before it _existed._ because markdown is what’s known as “light-markup”.

which, if you consult wikipedia, gets called “lightweight-markup”.

> <http://en.wikipedia.org/wiki/lightweight_markup_language>

but i don’t think it’s “lightweight” at all; i believe it’s a heavy hitter.

i _love_ _love_ _love_ light-markup! i’ve loved it for well over a decade!

so, to repeat, i’m a long-time fan of markdown specifically and also all other types of “light-markup”, going back to “restructured-text”, which was one of the original ones.

(ok, actually “structured-text” was probably _the_ original, but it got re-mixed into “restructured-text”.)







## restructured-text


“restructured-text” is well-known, since the python community has been using it for a long time as its primary format for documentation.

> <http://docutils.sourceforge.net/rst.html>

as that implies, restructured-text has proven itself to be up to the task of doing technically-oriented material for a technically-oriented audience.

so much for the “lightweight” slur.







## ascii-doc


“ascii-doc” is another format which has enjoyed wide implementation, even though it is even less well-known than “restructured-text”.

> <http://asciidoc.org>

ascii-doc can generate output in a large variety of formats, proving itself in an impressive range of situations, even more so than restructured-text.

since “ascii-doc” is also one of the “heaviest” forms of light-markup, it’s not a surprise that it gets most of its attention mainly from a plethora of larger organizations.

> <http://asciidoctor.org>

for instance, ascii-doc was adopted by many in the o’reilly camp nowadays, and is now used as the primary engine for their newest system, called “atlas”, which they steer their authors toward.

> <http://atlas.labs.oreilly.com>

“atlas” also takes markdown as input, but it makes clear that markdown is not really fully up to snuff for the job.

(it must’ve really killed some people over at o’reilly to eat crow and admit that i was right all along when i was lecturing them to favor light-markup, laughing at their docbook bloatware, and heaping scorn upon their blatant x.m.l. promotion at their conventions for the publishing industry, ones which they no longer even bother to conduct, probably because they’re embarrassed to concede that all of their advice was wrong, wrong, wrong, wrong, wrong.)







## textile


among other tech kids, “textile” was often one of their first exposures to any form of light-markup, and thus it initially enjoyed good prominence, especially when it was fairly newish.

while not disappearing entirely, by any stretch of the imagination, it has nonetheless faded in importance, as evidenced by the fact that the best link i can give for it is wikipedia.

> <http://en.wikipedia.org/wiki/Textile_(markup_language)>

in the early days, restructured-text, ascii-doc, and textile were the top three.

despite the numerous other players -- which could also include all of the wiki-markup-oriented derivations -- in the light-markup game, those three were the leading contenders at the top of the light-markup heap.







## markdown’s arrival


but then markdown rode into town.

markdown came from john gruber, who was ascending on the wave of blogging’s big rise, and it benefited from the exposure which he gave it.

and thus markdown’s adoption continued to grow along with gruber’s audience.

true, for a while, that adoption was limited to relatively “minor” places, like the comment sections of blogs.

but in the last few years, markdown has leveraged critical mass for itself.

it is used at <http://stackoverflow.com> and <http://github.com>; considering that these sites have a massive following among techies on the cutting-edge, it was easy to predict a blossoming.

as these techies were exposed to the ease and convenience of light-markup, they were converted to its usefulness.

so, sure enough, now markdown is appearing in all kinds of tech places, including ones of some significance.

among these new appearances was a recent emergence of “static blogs”. tech-minded people found it simple to create a mass of plain-text-files, and then use a markdown script to convert them to the .html-files that can then constitute their static blog.

this movement away from mysql to a flat-file approach is one that might ramify deeply in the future.

and techies have been increasingly using markdown to make manuals and documentation for their apps.

even these people, for whom .html comes “naturally”, seem to want to use a light-markup format instead, both to avoid the tedium of markup and to be able to edit “clean” text.

the fact that the techies now prefer predominately to use light-markup is quite an important demarcation.







## markdown in public


and it wasn’t just techies focused on handling of their own content, either.

developers soon realized that it was a benefit for “unsophisticated users” to let them write in markdown, so as to spare ‘em from the pain of .html. (and to ensure their input was clean!)







## i.o.s. apps


the most stark place for new uses happens to be the ipad and iphone. literally dozens of i.o.s. apps use markdown these days, thanks to its high profile among developers.

this is especially true because many of the apps on those machines are geared towards jotting down notes, not what’s typically called “writing”.

so i won’t focus much on those apps, as that’s an essay of its own, but also because i’m much more interested in the use of light-markup for “writing”, so, for that, we will turn to the web.

if you’re curious about i.o.s. apps, brett terpstra made a review page:

> <http://brettterpstra.com/ios-text-editors>

for the record, brett’s summary table has entries on 99 different i.o.s. apps!

you can also search the app-store for “markdown” for a sense of the breadth.

of course, lots of the i.o.s. apps are hooked up with the web as well, so a person can work on a file _either_ with a mobile device or on the web.

but it sharpens our attention to look at web-sites that focus on _writing._







## draftin dot com


a number of new sites have writing -- and re-writing, version-tracking, editing, collaborative writing, etc. -- as their primary reason for being, and incorporate markdown as well.

one of the best examples is “draft”:

> <http://draftin.com>

“draft” is a site that has gotten lots of praise, from a wide swath of people, and has a healthy base of users, some of them paying the reasonable price of $3-per-month for the service, which hyped easy version-tracking as its primary benefit when it started out, but has since offered a number of other services that are of value to the writer.







## editorially


markdown is also used at “editorially”, a site coming out of a very long beta, targeted on the collaboration process occurring between writers and editors.

> <http://editorially.com>







## ghost


and again, returning to blogs for a bit, one of the most high-profile initiatives in the blogging world today -- “ghost” -- made big noise about using markdown, as one of its marketing messages in a kickstarter campaign that made its goal within a few days, and then went on to raise some $300,000+ by its conclusion.

> <http://ghost.org>

“ghost” has recently begun to be released, and it will be of particular interest to me, since it has made the 2-up input/output user-interface a major jewel in its crown, so many people will be encountering it for the first time in constant heavy use, and i’m curious as to how they’ll react.







## wordpress


and i should mention that “wordpress” just this week announced that it is now supporting markdown in its editor. whether or not this is in response to the “ghost” initiative is not clear; it may, or perhaps it’s a coincidence.







## dillinger


but even long before “ghost”, markdown was being adopted by web-apps which employ a methodology of cloud-storage, where you control where files are saved.

one of my favorites there is “dillinger”, which also has the 2-up user-interface.

> <http://dillinger.io>

“dillinger” can save your files to “dropbox”, “google-drive”, or “github” -- your choice.

like i said, “dillinger” is one of my favorites, of these online editors, but there are _lots_ of them, all basically pretty much the same, so look around until you find your favorite. a recap of them all would be another essay.







## simplenote


but i’ll mention one another important one, however, namely “simplenote”, because it was an early cloud-based note-taking app that used plain-text as its primary format, and it built an excellent _sync_ capability which other similar apps could use as well.

> <http://app.simplenote.com>

“simplenote” sync was known for its speed and for the high quality of its performance. these are both hard problems, which giants (like apple) have stumbled on (often badly), so it was great for a small guy to get it right.

“dropbox” is the gold-standard in this regard, but many developers claim “simplenote” sync is even faster and more accurate, high praise. (although, in fairness, “simplenote” only does plain-text files, while “dropbox” does all types.)

“simplenote” made it very easy for developers to use their service, in the early days, thereby earning the admiration of many early-adopters.

“automattic”, makers of “wordpress”, recently purchased “simplenote” -- mainly because of “simperium”, its sync -- so it’s big-time now. and with editors for i.o.s., the mac, android, and the web, “simplenote” is a shining pointer toward a new reality where all our documents are available to all our machines all the time. (and perhaps this is why “wordpress” itself is now supporting markdown in its own editor.)







## long-form light-markup


now let’s swing back to long-form stuff again, because long-form is my specialized interest.

you might wonder what i mean by “long-form”.

it should be obvious that “long-form” refers to a text that is longer rather than shorter, but other considerations also come to bear.

_books,_ of course, are the prototype of the long-form document, but i define long-form more broadly as “any document that contains easily-differentiated sections and thus benefits by offering a table of contents to the reader”.

in a book, those sections are “chapters”, plus the front-matter and back-matter parts; but under this definition, a scientific article would qualify as well, with sections like “title page”, “abstract”, “introduction”, “method”, “results”, “discussion”, “references”, and “appendices”.

likewise with an annual report, a legal brief, a manual for a gadget or car or appliance, or (as i’ve mentioned) software documentation.

in this respect, a long-form document will often resemble a full _web-site_ -- with each section living on its own web-page -- and not merely one individual _web-page,_ which is the product typically pictured as the output from markdown.







## leanpub


web-sites that help writers create long-form are just starting to pop up, in what appears might be a big trend, but there’s one that has been around for a couple years already, and deserves mention.

it’s called “leanpub”, and it can be found here:

> <http://leanpub.com>

more than just an authoring-tool, leanpub also offers services as a bookstore, and is touting a “release-early-release-often” publishing model, where it makes a book available to purchasers while it is in the process of being written so that the book can (hypothetically) be strengthened by the feedback provided by the early purchasers.

as a publisher/bookstore/whatever, leanpub pays great “royalties” -- in the range of 90% -- and gives its authors/publishers/whatever the ability to offer _variable_ _pricing_ on a book, a flexible touch. (it also lets authors donate royalties to a charity.)

while i sincerely doubt that a “release-often” model is the best one in today’s world, where people are too busy to read a book once, let alone many times just to see what’s been changed between versions, i certainly think that it’s an experiment worth trying, and i’m glad somebody has the balls to do just that.

there are other things i don’t like about leanpub -- like the workflow which forces its users to chop up their books into a separate file for every chapter, which i have found increases consistency errors -- but as they say, “that’s what makes a horse-race”.

and i do commend “leanpub” for creating a platform that concentrates on the long-form book experience.







## scrivener


while we’re on the topic of books, let’s swing back, for just a minute, to the world of offline programs, because a big one in regard to books is scrivener.

scrivener is far more than a markdown text-editor; it’s a smorgasbord of capabilities for writing books (cork-storyboarding, an outlining tool, and so on). it’s probably over-the-top bloated functionality for most markdown users, who generally tend to favor the “distraction-free” side of the “busy” continuum, but it would be a clear omission not to mention it, since scrivener is one of the few book-focused apps. as such, it offers .epub output, not just typical .html.

> <http://www.literatureandlatte.com>

further, it’s a revealing fact that many users who _do_ love “scrivener” love it _very_ _strongly._

so if you think you’d like a book “project manager” -- which is how the “scrivener” hype describes it -- for your writing endeavors, check out “scrivener”. any program that earns this much loyalty is special.







## texts dot app


and as we are talking offline, if only for a brief time, i can mention another few apps that are stand-out, in that they have a considerable book perspective.

one is called “texts”. first of all, it is cross-platform, with programs for both mac and p.c., and i.o.s. too.

further, it outputs .pdf, ms-word.doc, and even tex, in addition to the expected .html and .epub e-books; so that represents a rather complete package of rad. and, for a limited time anyway, it costs less than $15. “texts” is one of the apps that attempts to combine “input” and “output” in the same window, so if you think you would be attracted to that method, try it.

> <http://www.textseditor.com>







## textastic


the other is called “textastic”. there’s no p.c. version, but there are versions for iphone, ipad, and the mac. this is a programmer’s editor, with syntax-coloring -- yes, the colors are applied to markdown syntax -- but it’s handy as it syncs to either dropbox or icloud.

> <http://www.textasticapp.com>

one more section here, and then we’re all done.







## zen markup language


i, too, have developed a system for long-form texts, one that’s firmly grounded in a light-markup format that’s called “zen markup language”, z.m.l. for short.

my light-markup system differs from markdown in that it: 1) is targeted at long-form documents, such as books, 2) avoids the problems which plague markdown, 3) focuses on lightness as an asset that _eases_ _editing_, rather than as something that _fosters_ _readability_ _of_ _the_ _raw_ _format_ (as there’s no reason to read the file in that raw format).

speaking of readability, as well as my focus on long-form, .html is not the only output format supported by my system; it also generates .epub, .mobi, .pdf, and (soon) slide-show presentation modules, and i’m always on the lookout for still-to-come formats. (i’ve also coded my own e-book viewer-apps for the format, of course, which are very powerful.)

z.m.l. was derived from e-texts at project gutenberg -- i have been working on it for over 15 years now -- so it springs from the structures found in actual books, a focus which differs philosophically from markdown’s source (i.e., things that are possible in .html on a web-page). my targeting of the long-form in general, and books in particular, provides a rich field of suggestion about the functionalities that need to be provided.

perhaps most significantly, from the standpoint of this “considered harmful” essay, however, is the fact that with z.m.l., i intend to sidestep some of the problems inherent in markdown, or which have emerged with it.







## summary


in conclusion, let’s review the problems with markdown.

1. gruber’s classic version is far too primitive.

2. gruber’s classic version isn’t detailed enough.

3. gruber’s classic version exhibits edge-cases.

4. gruber continually refuses to acknowledge this.

5. the extensions added capabilities haphazardly.

6. the extensions often conflict with each other.

7. the extensions destroy the “intuitive” asset.

8. the extension developers refuse to collaborate.

9. markdown infrastructure isn’t cross-plat enough.

10. markdown infrastructure is far too piecemeal.

11. there is absolutely no way out of this quagmire.

12. as more users adopt markdown, more trouble will surface.

-bowerbird

p.s. wanna talk about a primitive markup and text-editor? this set-up here at medium takes the cake! and it has received so much hype. oh well…
