---
author: "Ryan Williams"
title: "'Online-only' post-mortem"
layout: "post"
permalink: /post-mortem/
---

# NE Scala 2020: "online-only" post-mortem
*2020-03-20*
 
On Saturday [we](https://github.com/orgs/nescalas/people) wrapped up the [Northeast Scala Symposium](https://nescala.io/): a community-run conference related to [the Scala programming language](https://www.scala-lang.org/).

## Going "online-only" at the last minute
On Tuesday, having sold 170 tickets to a conference starting Thursday at [a venue in DUMBO](https://www.26bridge.com/), [we decided to go "online only"](https://twitter.com/nescalas/status/1237485050234617856).

It's possible we should have made the call earlier. As is, some ppl were able to cancel their travel plans, others had already traveled, and (seemingly most) others had canceled on their own (or their employers had done it on their behalf).

We watched closely what other events were doing; we were much smaller than many of the big-name cancellations, and thought we might still be able to offer a remote option while meeting in-person with whoever was comfortable doing so.

When confirmed cases and lockdowns came to the NYC area, we quickly decided to cancel the physical event.

## Cancel all the things 😔
That required canceling our {[venue](https://www.26bridge.com/), [A/V](https://ulsnyc.com/), [internet](https://events.gtt.net/), [security](http://theoutfitgroup.com/security/), [catering](https://www.dostoros.com/catering), [videographer](http://acavideo.com/)} about 36hrs before the event.

All of those sectors are having a very bad time right now, of course, and we're basically following their lead about whether we should be refunded for any, some, or all of what we paid. In at least one case, we've been offered a full refund but are planning to insist they take some partial payment.

Elsewhere, things are presumably more contentious; one of our vendors shared an anecdote about a negotiation involving [a much bigger, more expensive event] and [a big, canceled hotel-room block] that has already turned litigious.

We're a small event with a lot of good-will between sponsors, attendees, and vendors, so I'm optimistic everyone will feel reasonably whole.

## Running the conference

We primarily relied on [Zoom](#zoom) (videoconferencing) and [Slack](#slack) (group chat):

### [Zoom](https://zoom.us/)
To run the conference, we bought [a $500/mo Zoom plan](https://zoom.us/pricing) including a ≤500-person "webinar" room.

We had ≈100 ppl in the "webinar" room for most of two 8-hr days:

![speaker view: live video feed, attendee+panelist list, and Q&A modal](/assets/imgs/speaker-view.gif)

*(speaker view: live video feed, attendee+panelist list, and Q&A modal)*

#### "Breakout rooms"

There were also been 5 "breakout rooms" anyone could join and talk in. After the conference on day 2, ppl gathered in one of those for an e-"happy hour" (I was tired and didn't stick around to see how it went, though).

![NE Scala organizers chatting in the "webinar", complete with fancy "virtual backgrounds"; Zoom mirrors your view of your own background, to facilitate any interacting with it you may like to do 😂](/assets/imgs/zoom-hosts.png)

*(NE Scala organizers chatting in the "webinar", complete with fancy "virtual backgrounds"; Zoom mirrors your view of your own background, to facilitate any interacting with it you may like to do 😂)*

#### Videos
Zoom recorded 8hrs/day of the main room ("to the cloud"):

![8hrs of video for ≈1.5GB; video codecs are wild](/assets/imgs/recording-sizes.png)

*(8hrs of video for ≈1.5GB; video codecs are wild)*

Each evening I got a link to the raw footage, that I shared with the entire conference in Slack:
* [day 1](https://zoom.us/rec/share/x8kkKLzsz1NLU6fu0xDHV6cKAoTIeaa8hHAW-fJeyhuEnHpDD2Mo_-gItYzXZAQV)
* [day 2](https://zoom.us/rec/share/vMx5FLHu5FxLTp3G5WXNVJMlT4jraaa8gyZPq_Vc-YHrRtAjo7ashE3PhaogNw)

We'll probably stick with [our videographer](http://acavideo.com/) for post-processing the videos and getting them on YouTube (as originally planned), but it's pretty cool to have the footage available immediately as well (some speakers can probably just slice out their talks and share them as they see fit).

#### Group Chat, Q&A
Zoom rooms always have a "chat" feature (with fine-grained visibility permissions, per-message); in addition, "webinars" have a structure "Q&A" window:

![Various Zoom "webinar" windows: "Participants", "Chat", and "Q&A" (also Slack in the background)](/assets/imgs/chat.png)

*(Various Zoom "webinar" windows: "Participants", "Chat", and "Q&A" (also Slack in the background))*

Questions and discussion about each talk were split between Zoom chat, Zoom Q&A, and our Slack "#talks" channel. This was all new enough that we decided not to push people too hard to any single channel. Some reflections:
- I expected the "Q&A" flow to be best, but it was almost never used
- Zoom chat was most frequently used, but had rough edges:
  - Attendees' chats defaulted to only being visible to "panelists" (presenters and hosts) when they more commonly meant to address everyone
  - Speakers often had trouble finding+viewing the chat window while presenting
  - General lack of functionality (vs. Slack's rich text, threading, and search)
  - Chat history was generally not kept available to people:
    - when speakers were changed back to being "attendees" (at the end of their talks)
    - when people left and rejoined the room
    - (we did enable a setting to save chat history alongside our recordings, and accordingly seem to have received `.txt` files next to our `.mp4`s/`.m4a`s)
- Speakers mostly followed 0 or 1 of the 3 channels; usually moderators just read out loud from whichever of the 3 questions appeared in

#### Settings, UX
Zoom has a huge number of settings available:

![Scrolling down many folds of a Zoom settings page](/assets/imgs/zoom-settings.gif)

Many are available at both user- and account-level granularities. My programmer-brain respects the extensive customizability, but something about the UX was off; some settings depend on others in unclear ways, and some things appear in two different places (e.g. recordings "to the cloud").

### [Slack](https://slack.com/)
We also leaned heavily on Slack for group chat.

We've used it to communicate with attendees, and among organizers, for years, but this year attendees and organizers alike brought some extra energy to make it feel like a real community:

![example messages and "applause" in the #talks channel during a particularly interesting talk](/assets/imgs/talks-channel.gif)

*(example messages and "applause" in the #talks channel during a particularly interesting talk)*

Various channels have focused on live discussions about the talks (`#talks`), conference logistics/q's (`#feedback`), job-seeking and hiring (`#jobs`), and misc other topics (e.g. `#category-theory`).

#### Slack Norms

![Header bar of the #general Slack channel, showing 268 members and a "topic" encouraging use of "threads" and "pinned msgs"](/assets/imgs/general-topic.png)

*("Please 'thread' replies, and check the "pinned" msgs for impt high-level info.")*

A lot people's work-Slacks are much bigger and livelier than ours, but a couple reflections on choices we made and norms that emerged:

##### Threading
We suggested people "thread" discussions, but ended up with a mix of threaded and un-threaded discussion.

I'd guess ≈even splits between people that love threads, hate threads, and [are confused by the UX so don't use them].

A couple features that seem surprisingly absent:
- inability to auto-subscribe to all msgs (even in threads) in a channel
- not being subscribed if you "react" to a post

##### Pinned Messages
We tried to use "pinned msgs" in each channel to make impt high-level info quickly visible (esp. to new members):

![Screenshot showing "Pinned Messages" providing various important info about joining VCs, signing up for unconference talks, etc.](/assets/imgs/pinned-msgs.png)

*(Lots of good "annouce"-y content was available, if you knew where to look)*

It should have been a good system; I'm not sure anyone really noticed or used them though.

I frequently used the pins to refer back to impt info (often to copy+paste a URL for someone who was asking, bc they'd not seen the relevant pinned msg).

The UX around them probably needs to be more prominent; I've used Slack for years and learned about pinned msgs while poking around last week.

##### Rich text
I was grasping at every bit of markup I could deploy to highlight, nest, and group info in "announce"-style msgs:

!["Announcement" message using lots of Slack's rich-text functionality](/assets/imgs/rich-text.png)

*(Inline links, bolding, bold links, bullets, paragraph breaks… my kingdom for a font-size picker and/or nested bullets! or, y'know, markdown 🤞🏻)*

#### "Free" as in "search history"

Slack worked really well, though we're somewhat awkwardly stuck on the "free tier" (capped at 10k msgs across all users+channels);

![NE Scala's Slack workspace is currently using 9k of the 10k messages available on the free plan](/assets/imgs/slack-msg-count.png)

*(those 9k msgs take us back to 2015 or so, when NE Scala started using Slack 🤷🏼‍♂️)*

When we hit 10k msgs, we'll start [losing access to our earliest msgs] or [paying ≈$1700/mo for our ≈250 Slack users](https://app.slack.com/plans/T0FUWP1D3), I guess? We might qualify for Slack's [non-profit](https://slack.com/help/articles/204368833-Slack-for-Nonprofits) or [education](https://slack.com/help/articles/206646877-Slack-for-Education) discounts, but it was all our volunteer corps could do this year to have an LLC and bank account up in time to invoice sponsors, receive ticket payouts, and pay vendors. 

### [Some] hands on deck
During the conference-days, we typically had 2-3ppl focused on running the event, performing 2-3 logical roles:
* emcee (introduce speakers, moderate Q&A)
* tweeter (sometimes same as the emcee; cf. [**nescalas**](https://twitter.com/nescalas))
* Slack "ops" (answering logistical q's, announcing talks, corraling speakers, getting/linking slides, updating [website](https://nescala.io/), etc.)

We planned to have more folks available, but several ended up being sick and/or taking care of kids who were unexpectedly home. Some attendees really stepped up to help with duties, which was much appreciated.

### T-shirts
No sooner had we announced our move to "digital only" than I took delivery of 230 NE Scala 2020 t-shirts:

![Ryan standing next to a large stack of boxes full of t-shirts](/assets/imgs/t-shirts.jpg)

*(it seemed like a good idea at the time)*

#### [customink.com](https://www.customink.com/)
We got the shirts from [customink.com](https://www.customink.com/). They were good to work with; the shirts ended up being $7.92ea ($8.71 w/ "rush" 1-wk shipping) after they fixed up our design, post-order (simplifying and removing some colors to bring the price down).

![action shot: NE Scala 2020 "slack ops", in uniform](/assets/imgs/ryan-desk.jpg)
![posing in "mission control"](/assets/imgs/ryan-mission-control.jpg)

*(confirmed: the shirts are good 👍🏻)*

Maybe I can get my co-organizers over for a t-shirt-mailing party next wknd 🤞🏻.

### Day 3: "Unconference"
On the third and final day of the conference, we hold an "unconference": a collaboratively-edited google-sheet is opened to everyone in the morning, and they fill in {room x time-slot} cells with talks or topics they want to give or discuss.

Our 5 Zoom "[breakout rooms](#breakout-rooms)" hosted those various smaller/less-formal talks all day (and most or all of them were recorded, for the first time!).
 
## Conclusion
Working on this conference for months, and then moving the whole thing online at the last minute, was a wild experience.

People (including me) seemed mostly pleasantly surprised about how it went. It definitely missed some of the serendipitous networking interactions people love about physical conferences, though some of that was recouped thanks to a community effort to interact meaningfully online.

Online-only also fostered dynamics that don't have a direct analogues in physical space. For example, several dozen people could participate in (or just read and give a drive-by emoji-reaction to) a particularly funny or lively Slack conversation (while real-life conversations cap out at much smaller sizes):

![Slack msgs from the #general channel with lots of interactions](/assets/imgs/group-slacking.png)

*(keeping everyone on the same page)*

### Looking Forward
We're assuming NE Scala 2021 will be a physical event (it's Boston's turn…).

However, we're also anticipating continued demand for attendees and speakers to participate remotely (there were many discussions around this for 2020 even before COVID19-related concerns really flared up).

Keeping the remote community active online through the year is also a newly-appealing proposition. 

Seeing how possible it may be to run our event remotely – and spread our communing temporally outside the 3d of conference – has been very eye-opening, and we hope you've found this debrief about our experience useful or interesting!

### Thanks
Our sponsors and community have been really generous and wonderful through this whole roller-coaster; thanks again to them and everyone who participated!

![NE Scala sponsors: Bridgewater, Foursquare, Tapad, Inner Product, Spotify, Comcast, dv01, and Lightbend](/assets/imgs/sponsors.png)

---------

## Appendix: useful tools during the lead-up to the conference
Below are experience reports about various other tools we used to run the conference:
- [Eventbrite](#eventbrite) (ticket sales)
- [Papercall](#papercallio) (CFPs)
- [GitHub Pages](#github-pages) (conference website)
- [Google Domains](#google-domains) (conference website, rudimentary email forwarding)

### [Eventbrite](http://eventbrite.com/)
[We sold tickets through Eventbrite](https://www.eventbrite.com/e/northeast-scala-symposium-typelevel-summit-2020-tickets-92788556069) (as well as managing+emailing attendees, creating discount/promo codes, etc.).

![Graph of net sales revenue over the last month of ticket sales](/assets/imgs/tix.png)

*(refund requests were trickling in over the last week, but new ticket sales basically kept pace with them)*

### [papercall.io](https://www.papercall.io/)
We used Papercall to run a CFP for each of the first two days of the conference:
* [Day 1 ("Typelevel Summit")](https://www.papercall.io/typelevel-summit-nyc-2020)
* [Day 2 ("NE Scala")](https://www.papercall.io/nescala-2020)

(historically, the conference is two separate events, that now always co-locate; we still "ship our org chart" in some ways)

Papercall worked pretty well, though I ended up writing [a scraper](https://gist.github.com/ryan-williams/65c6143d3a027cd2532785565d740ca8#file-01-scrape-papercall-ipynb) to get the talk details out, followed by [some pandas](https://gist.github.com/ryan-williams/65c6143d3a027cd2532785565d740ca8#file-02-generate-proposed-talks-page-ipynb) to munge them and dump out [a "Proposed Talks" HTML page](https://nescala.io/proposed-talks) and "[ballot](https://docs.google.com/forms/d/e/1FAIpQLSdr9YTEvJcvcYOeSx3ddiWp0AuvW1PlumaNOzt2r8E9KtXGWA/viewform)" (a Google Form; attendees vote on talks).

At the time, I needed to get the ballot out quickly, and scraping seemed faster than:
* paying for API access
* trying to sort through what looked like a long-tail of potentially-half-baked clients

#### Randomizing order of proposed talks (on static site and official ballot)
For the first time, we randomized the order in which "proposed talks" were displayed, wherever possible:
* [this JS](https://github.com/nescalas/nescalas.github.io/blob/b349bf2a57d02b1428060796959a9f78e81ca70a/proposed-talks.html#L629-L654) did the trick on [the "Proposed Talks" page](https://nescala.io/proposed-talks)
* Google Forms gives you this option automatically:
  ![](/assets/imgs/gform-shuffle.png)  

It was nice to remove a potential source of bias in that way, with relatively little effort.

### [GitHub Pages](https://pages.github.com/)
[The conference site](https://nescala.io/) is a static site hosted on [GitHub Pages](https://pages.github.com/), and [its source is public](https://github.com/nescalas/nescalas.github.io).

#### Live previewing
Most changes went through a PR/review flow, and I came up with a good system for publishing a "live preview" of a PR's changes:
* I added [nescalas.github.io](https://github.com/nescalas/nescalas.github.io) as a git submodule (named e.g. `nescala`) of another GitHub Pages site I control
* push my NE Scala changes to a branch on [nescalas.github.io](https://github.com/nescalas/nescalas.github.io) (this was a natural part of creating a PR anyway; we weren't bothering with PR'ing from forks) so that they are publicly accessible (and clone-able!)
* set the [nescalas.github.io](https://github.com/nescalas/nescalas.github.io) submodule in my other site to the git commit of the PR'd branch
* push the other site 

Example: [nescalas.github.io#9](https://github.com/nescalas/nescalas.github.io/pull/9)

#### Jekyll Opacity
GitHub Pages is generally an amazing service, though it could be more helpful when Jekyll builds fail for some reason. On one occasion, I pushed a few updates to some image assets ([sponsor logos](https://nescala.io/#sponsors)) and got a cryptic, non-actionable email that the site build failed:

![screenshot of "Build failed" email from github-pages about a failed Jekyll build](/assets/imgs/jekyll.png)

Re-pushing the images one at a time (was one of them corrupt in some way that was giving Jekyll problems?) resulted in only successful builds 🤔.

### [Google Domains](https://domains.google.com/)
For some reason, we used our [ny-scala.org](http://ny-scala.org/) (administered by Google Domains for a whopping $12/yr) to do email-forwarding, to give some veneer of formality to our emails with sponsors and vendors (and help us manage our personal inboxes). 

This part was really clumsy:
* we used ny-scala.org instead of nescala.io for reasons that escape me now (I think we didn't have admin access to the latter when we started organizing this year?)
* we didn't pay for actual GSuite accounts under ny-scala.org, but just set up email fwds for organizers (e.g. from `<name>@ny-scala.org` to `<name>`'s personal email)
  * that was ok e.g. for telling ppl **to** "email `<name>@ny-scala.org` for access to the Slack workspace"
  * it was awkward in threads with vendors and sponsors (where we were ultimately emailing **from** our personal email addresses)

#### Minimizing telephone game
It was also clumsy to not have a single email address, that all organizers had read+write access to, that we could cc or bcc on all relevant emails.

By the later stages, I was intent on there not being pertinent emails, on any topic related to the conference, that only one person was privy to (as it was, we had separate people email the same sponsor, confusion/misplacing of important details about vendors, etc).  I ended up just cc'ing 4 organizers' personal gmail addresses onto every email I sent, which was not ideal.

#### GSuite accounts?
We are a low-budget affair and have a very dispersed base of organizers (≈5, ≈10, or ≈30, depending how you count); I don't know if it would have made sense to make a GSuite account ($6/user/mo?) for organizers to use. Since there is little organizing or conferencing happening for at least half the year, I don't know if it makes sense to pay for any or many GSuite accounts year-round (and I don't know if there's a graceful way to only pay for them some of the time, but leave them dormant for part of the year?)

It could be that we should think of this as the cost of doing business. It's also possible that there is a better deal for non-profits, if we officially went this route (hopefully we will, later this year).   

## TODO
- D&I
- LLC, bank acct
- anon Q&A (enabling, moderating, etc.)
- validating email addresses/users
- better visibility about breakout rooms, facilitating casual interactions that ppl love from IRL confs.
- online-only vs. mixed IRL/digital
- speaker prep for webinar presenting, etc., test webinars
- sponsors: reaching out, paperwork, accepting payments
- CoC, supporting anonymous reporting to organizers

