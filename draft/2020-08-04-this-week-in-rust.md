Title: This Week in Rust 350
Number: 350
Date: 2020-08-04
Category: This Week in Rust

Hello and welcome to another issue of *This Week in Rust*!
[Rust](http://rust-lang.org) is a systems language pursuing the trifecta: safety, concurrency, and speed.
This is a weekly summary of its progress and community.
Want something mentioned? Tweet us at [@ThisWeekInRust](https://twitter.com/ThisWeekInRust) or [send us a pull request](https://github.com/cmr/this-week-in-rust).
Want to get involved? [We love contributions](https://github.com/rust-lang/rust/blob/master/CONTRIBUTING.md).

*This Week in Rust* is openly developed [on GitHub](https://github.com/cmr/this-week-in-rust).
If you find any errors in this week's issue, [please submit a PR](https://github.com/cmr/this-week-in-rust/pulls).

Check out [this week's *This Week in Rust Podcast*](https://rustacean-station.org/episode/024-twir-349/)

# Updates from Rust Community

### Official

### Tooling

### Observations/Thoughts

### Learn

### Project Updates

* [meli terminal mail client v0.6.0 alpha release](https://meli.delivery/posts/2020-07-29-v0.6-alpha-release.html)

### Miscellaneous

# Crate of the Week

This week's crate is [polyfuse](https://github.com/ubnt-intrepid/polyfuse), a library for writing FUSE file systems using async code.

Thanks to [Ivan Kozik](https://users.rust-lang.org/t/crate-of-the-week/2704/795) for the suggestion!

[Submit your suggestions and votes for next week][submit_crate]!

[submit_crate]: https://users.rust-lang.org/t/crate-of-the-week/2704

# Call for Participation

Always wanted to contribute to open-source projects but didn't know where to start?
Every week we highlight some tasks from the Rust community for you to pick and get started!

Some of these tasks may also have mentors available, visit the task page for more information.

If you are a Rust project owner and are looking for contributors, please submit tasks [here][guidelines].

[guidelines]: https://users.rust-lang.org/t/twir-call-for-participation/4821

# Updates from Rust Core

347 pull requests were [merged in the last week][merged]

[merged]: https://github.com/search?q=is%3Apr+org%3Arust-lang+is%3Amerged+merged%3A2020-07-20..2020-07-27

* [AVR: correctly set the pointer address space when constructing pointers to functions](https://github.com/rust-lang/rust/pull/73270)
* [detect turbofish missing surrounding angle brackets](https://github.com/rust-lang/rust/pull/74687)
* [serialize span hygiene data](https://github.com/rust-lang/rust/pull/72121)
* [proc_macro: add API for tracked access to environment variables](https://github.com/rust-lang/rust/pull/74653)
* [correctly deal with unsorted generic parameters](https://github.com/rust-lang/rust/pull/74676)
* [normalize bounds fully when checking defaulted types](https://github.com/rust-lang/rust/pull/74670)
* [disallow non-static lifetimes in const generics](https://github.com/rust-lang/rust/pull/74051)
* [forbid generic parameters in anon consts inside of type defaults](https://github.com/rust-lang/rust/pull/74487)
* [add a system for creating diffs across multiple mir optimizations](https://github.com/rust-lang/rust/pull/74715)
* [optimize away `BitAnd` and `BitOr` when possible](https://github.com/rust-lang/rust/pull/74491)
* [make more primitive integer methods const](https://github.com/rust-lang/rust/pull/73858)
* [impl Default for ranges](https://github.com/rust-lang/rust/pull/73197)
* [remove needless unsafety from `BTreeMap::drain_filter`](https://github.com/rust-lang/rust/pull/74677)
* [hashbrown: refactor probing logic into an external iterator](https://github.com/rust-lang/hashbrown/pull/181)
* [rustlings: add ability to run rustlings on repl.it](https://github.com/rust-lang/rustlings/pull/471)

## Rust Compiler Performance Triage

* [2020-07-28](https://github.com/rust-lang/rustc-perf/blob/master/triage/2020-07-28.md).
  2 regressions, 1 improvement, none in rollups.

## Approved RFCs

Changes to Rust follow the Rust [RFC (request for comments) process](https://github.com/rust-lang/rfcs#rust-rfcs). These
are the RFCs that were approved for implementation this week:

* [Inline assembly](https://github.com/rust-lang/rfcs/pull/2873)
* [Add a new `#[instruction_set(...)]` attribute for supporting per-function instruction set changes](https://github.com/rust-lang/rfcs/pull/2867)

## Final Comment Period

Every week [the team](https://www.rust-lang.org/team.html) announces the
'final comment period' for RFCs and key PRs which are reaching a
decision. Express your opinions now.

### [RFCs](https://github.com/rust-lang/rfcs/labels/final-comment-period)

* [RFC: 'C unwind' ABI](https://github.com/rust-lang/rfcs/pull/2945)

### [Tracking Issues & PRs](https://github.com/rust-lang/rust/labels/final-comment-period)

* [disposition: merge] [Stabilize Vec::leak as a method](https://github.com/rust-lang/rust/pull/74605)
* [disposition: merge] [add `slice::array_chunks` to std](https://github.com/rust-lang/rust/pull/74373)

## New RFCs

* [RFC: Add JSON backend to Rustdoc](https://github.com/rust-lang/rfcs/pull/2963)
* [RFC: Named arguments](https://github.com/rust-lang/rfcs/pull/2964)
* [Establish a new error handling project group](https://github.com/rust-lang/rfcs/pull/2965)

# Upcoming Events

### Online
* [July 27 - August 2. Rusty Days Virtual Rust Conference](https://rusty-days.org/)
* [August 5. Johannesburg, ZA - Johannesburg Rust Meetup - Monthly Joburg Rust Chat](https://www.meetup.com/Johannesburg-Rust-Meetup/events/271875886/)
* [August 5. Dublin, IE - Rust Dublin - August Remote Meetup](https://www.meetup.com/Rust-Dublin/events/272162980/)
* [August 5. Buffalo, NY, US - Buffalo Rust Meetup - Rust User Group](https://www.meetup.com/Buffalo-Rust-Meetup/events/271511557/)
* [August 5. Indianapolis, IN, US - Indy Rust - Indy.rs with Social Distancing](https://www.meetup.com/indyrs/events/jhfstrybclbhb/)
* [August 6. Linz, AT - Rust Meetup Linz - Kick Off](https://www.meetup.com/de-DE/Rust-Linz/events/271857182/)
* [August 6. Berlin, DE - Berline.rs - Rust Hack and Learn](https://www.meetup.com/opentechschool-berlin/events/txcprrybclbjb/)
* [August 11. Seattle, WA, US - Seattle Rust Meetup - Monthly meetup](https://www.meetup.com/Seattle-Rust-Meetup/events/gskksrybclbpb/)

### North America
* [July 28. Dallas, TX, US - Dallas Rust - Last Tuesday](https://www.meetup.com/Dallas-Rust/events/nppvrrybckblc/)

### Asia Pacific
* [August 3. Auckland, NZ - Rust ALK - Rust Meetup](https://www.meetup.com/rust-akl/events/266876693/)

If you are running a Rust event please add it to the [calendar] to get
it mentioned here. Please remember to add a link to the event too.
Email the [Rust Community Team][community] for access.

[calendar]: https://www.google.com/calendar/embed?src=apd9vmbc22egenmtu5l6c5jbfc%40group.calendar.google.com
[community]: mailto:community-team@rust-lang.org

# Rust Jobs

*Tweet us at [@ThisWeekInRust](https://twitter.com/ThisWeekInRust) to get your job offers listed here!*

# Quote of the Week

Sadly, we had no quote suggestions this week.

[Please submit quotes and vote for next week!](https://users.rust-lang.org/t/twir-quote-of-the-week/328)

*This Week in Rust is edited by: [nellshamrell](https://github.com/nellshamrell), [llogiq](https://github.com/llogiq), and [cdmistman](https://github.com/cdmistman).*

<small>[Discuss on r/rust](https://www.reddit.com/r/rust/comments/i094wo/this_week_in_rust_349/)</small>
