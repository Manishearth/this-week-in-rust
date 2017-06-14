Title: This Week in Rust 186
Number: 186
Date: 2017-06-13
Category: This Week in Rust

Hello and welcome to another issue of *This Week in Rust*!
[Rust](http://rust-lang.org) is a systems language pursuing the trifecta: safety, concurrency, and speed.
This is a weekly summary of its progress and community.
Want something mentioned? Tweet us at [@ThisWeekInRust](https://twitter.com/ThisWeekInRust) or [send us a pull request](https://github.com/cmr/this-week-in-rust).
Want to get involved? [We love contributions](https://github.com/rust-lang/rust/blob/master/CONTRIBUTING.md).

*This Week in Rust* is openly developed [on GitHub](https://github.com/cmr/this-week-in-rust).
If you find any errors in this week's issue, [please submit a PR](https://github.com/cmr/this-week-in-rust/pulls).

# Updates from Rust Community

## News & Blog Posts

* [What's coming up in imag (26)](https://imag-pim.org/blog/2017/06/11/whats-coming-up-in-imag-26/) published on [the new website](https://imag-pim.org/blog/2017/06/10/imag-pim.org---the-new-website/)

# Crate of the Week

This week's crate is [structopt](https://crates.io/crates/structopt), a crate that lets your auto-derive your command-line options from a struct to parse them into. Thanks to [m4b](https://users.rust-lang.org/u/m4b) for the suggestion!

[Submit your suggestions and votes for next week][submit_crate]!

[submit_crate]: https://users.rust-lang.org/t/crate-of-the-week/2704

# Call for Participation

Always wanted to contribute to open-source projects but didn't know where to start?
Every week we highlight some tasks from the Rust community for you to pick and get started!

Some of these tasks may also have mentors available, visit the task page for more information.

* [discussion] [What does Rust need today for server workloads](https://users.rust-lang.org/t/what-does-rust-need-today-for-server-workloads/11114)?
* [Rust libz blitz status update 2017-06-02](https://internals.rust-lang.org/t/rust-libz-blitz/5184/53). Contribution opportunities are available.
* [rustup: Create and publish a snap of rustup](https://github.com/rust-lang-nursery/rustup.rs/issues/1144).
* [rust: Create and publish a snap of Rust](https://github.com/rust-lang/rust/issues/42349).
* [rust: Update docker images to share scripts when possible](https://github.com/rust-lang/rust/issues/42201).
* [corrode-but-in-rust: let-defined lambdas aren't combined](https://github.com/tcr/corrode-but-in-rust/issues/65).
* [easy] [rust-url: Explain the term "fragment" in `Url::fragment`](https://github.com/servo/rust-url/issues/318).
* [easy] [rust-url: Modify docs to put error conditions into `Errors` sections](https://github.com/servo/rust-url/issues/314).
* [easy] [rust-url: Implement Debug for many types](https://github.com/servo/rust-url/issues/305).
* [rust-url: Document the percent_encoding module](https://github.com/servo/rust-url/issues/298).
* [easy] [reqwest: Examples for RequestBuilder::body](https://github.com/seanmonstar/reqwest/issues/119).
* [reqwest: Error doc improvements](https://github.com/seanmonstar/reqwest/issues/117).
* [reqwest: Response doc improvements](https://github.com/seanmonstar/reqwest/issues/115).
* [log: Remove env_logger from this repository](https://github.com/rust-lang-nursery/log/issues/145).
* [easy] [log: Expand log! docs for `max_level_*`](https://github.com/rust-lang-nursery/log/issues/125).
* [log: Support construction of `Record`s and `Metadata`](https://github.com/rust-lang-nursery/log/issues/116).

If you are a Rust project owner and are looking for contributors, please submit tasks [here][guidelines].

[guidelines]: https://users.rust-lang.org/t/twir-call-for-participation/4821

# Updates from Rust Core

115 pull requests were [merged in the last week][merged].

[merged]: https://github.com/issues?q=is%3Apr+org%3Arust-lang+is%3Amerged+merged%3A2017-06-06..2017-06-13

* [epic macro expansion speedup](https://github.com/rust-lang/rust/pull/42533)
* [`unimplemented!(..)` now allows message](https://github.com/rust-lang/rust/pull/42155)
* [better suggestions for missing trait impls](https://github.com/rust-lang/rust/pull/42383)
* [disentangle `InferCtxt", "MemCategorizationContext", `ExprUseVisitor`](https://github.com/rust-lang/rust/pull/42563) (plugin-breaking, but clippy already fixed)
* [convert `StdIo` from `File`, `ChildStdout`, `ChildStderr`](https://github.com/rust-lang/rust/pull/42133)
* [disallow "String"_ literals](https://github.com/rust-lang/rust/pull/41990) (No clue why this compiled in the first place?)
* [speed up `mem::swap(..)`](https://github.com/rust-lang/rust/pull/40454)
* [improve codegen for `.next_power_of_two` (and others)](https://github.com/rust-lang/rust/pull/42556)
* [our tests need more jokes!](https://github.com/rust-lang/rust/pull/42247) (look at the change list for some laughs)
* [don't panic, `rust_eh_parsonality()`!](https://github.com/rust-lang/rust/pull/42487)
* [don't store zero-sized pair fields](https://github.com/rust-lang/rust/pull/42486)
* [`#[inline]` `io::Error::from`](https://github.com/rust-lang/rust/pull/42426)
* [`use foo::self;` is now only one error](https://github.com/rust-lang/rust/pull/42580)
* [everything outlives the `'empty` lifetime](https://github.com/rust-lang/rust/pull/42482)
* [doctests skip files without three backticks](https://github.com/rust-lang/rust/pull/42437)
* [speed up cargo](https://github.com/rust-lang/cargo/pull/4118)

## New Contributors

* Edward Yang
* James Cowgill
* Jan Niehusmann
* Tom Prince
* zzhu

## Approved RFCs

Changes to Rust follow the Rust [RFC (request for comments)
process](https://github.com/rust-lang/rfcs#rust-rfcs). These
are the RFCs that were approved for implementation this week:

*No RFCs were approved this week.*

## Final Comment Period

Every week [the team](https://www.rust-lang.org/team.html) announces the
'final comment period' for RFCs and key PRs which are reaching a
decision. Express your opinions now. [This week's FCPs][fcp] are:

[fcp]: https://github.com/rust-lang/rfcs/labels/final-comment-period

* [disposition: merge] [Specify `#[repr(transparent)]`](https://github.com/rust-lang/rfcs/pull/1758).
* [disposition: merge] [Conversions from `&mut T` to `&Cell<T>`](https://github.com/rust-lang/rfcs/pull/1789).
* [disposition: merge] [Match ergonomics using default binding modes](https://github.com/rust-lang/rfcs/pull/2005).
* [disposition: merge] [Tiered browser support policy for Rust's web content](https://github.com/rust-lang/rfcs/pull/1985).
* [disposition: merge] [Prepare global allocators for stabilization](https://github.com/rust-lang/rfcs/pull/1974).

## New RFCs

* [Implement Add for OsString](https://github.com/rust-lang/rfcs/pull/2020).
* [Allow comparisons between integers of different types](https://github.com/rust-lang/rfcs/pull/2021).

## Style RFCs

[Style RFCs](https://github.com/rust-lang-nursery/fmt-rfcs) are part of the process for deciding on style guidelines for the Rust community and defaults for [Rustfmt](https://github.com/rust-lang-nursery/rustfmt). The process is similar to the RFC process, but we try to reach rough consensus on issues (including a final comment period) before progressing to PRs. Just like the RFC process, all users are welcome to comment and submit RFCs. If you want to help decide what Rust code should look like, come get involved!

We're making good progress and the style is coming together. If you want to see the style in practice, check out [our example](https://github.com/rust-lang-nursery/fmt-rfcs/blob/master/example/lists.rs) or use the [Integer32 Playground](https://play.integer32.com/) and select 'Proposed RFC' from the 'Format' menu. Be aware that implementation is work in progress.

Issues in final comment period:

* [[macro_use] on the same line as crate](https://github.com/rust-lang-nursery/fmt-rfcs/issues/83)
* [trait bounds](https://github.com/rust-lang-nursery/fmt-rfcs/issues/80)
* [Specify rules for breaking long `where` conditions](https://github.com/rust-lang-nursery/fmt-rfcs/issues/75)
* [Single-line `where`](https://github.com/rust-lang-nursery/fmt-rfcs/issues/74)

Good first issues:

We're happy to mentor these, please reach out to us in #rust-style if you'd like to get involved

* [paths](https://github.com/rust-lang-nursery/fmt-rfcs/issues/69)
* [simple expressions](https://github.com/rust-lang-nursery/fmt-rfcs/issues/68)
* [assignment and assignment operators](https://github.com/rust-lang-nursery/fmt-rfcs/issues/67)
* [control flow](https://github.com/rust-lang-nursery/fmt-rfcs/issues/62)

# Upcoming Events

* [Jun  7. Rust Cologne - Rust 2nd Anniversary Reloaded](http://rust.cologne/2017/06/07/rust-2nd-aniversary-part-2.html).
* [Jun  7. Rust Atlanta - Grab a beer with fellow Rustaceans](https://www.meetup.com/Rust-ATL/events/240072184/).
* [Jun  7. Rust Community Team Meeting at #rust-community on irc.mozilla.org](https://chat.mibbit.com/?server=irc.mozilla.org&channel=%23rust-community).
* [Jun  7. Rust Documentation Team Meeting at #rust-docs on irc.mozilla.org](https://chat.mibbit.com/?server=irc.mozilla.org&channel=%23rust-docs).
* [Jun  8. Columbus Rust Society - Monthly Meeting](https://www.meetup.com/columbus-rs/events/240198831/).
* [Jun 10. Hong Kong OS Conf 17 - Building Artificial Intelligence Units in Rust](https://hkoscon.org/2017/topics/building-artificial-intelligence-units-in-rust/).
* [Jun 10. RainOfRust Camp Nagpur - I](https://reps.mozilla.org/e/rainofrust-camp-nagpur-i/).
* [Jun 10. RainOfRust Camp Ahmedabad, Gujarat](https://reps.mozilla.org/e/rainofrust-camp-ahmedabad-gujarat-1/).
* [Jun 11. RainOfRust Camp Nagpur - II](https://reps.mozilla.org/e/rainofrust-camp-nagpur-ii/).
* [Jun 12. Seattle Rust Meetup](https://www.meetup.com/Seattle-Rust-Meetup/events/239841907/).
* [Jun 13. Rust Bay Area - Consensus with VMware's Haret and Service Meshes with linkerd-tcp](https://www.meetup.com/Rust-Bay-Area/events/240453207/).
* [Jun 13. RainOfRust Camp Vadodara, Gujarat](https://reps.mozilla.org/e/rainofrust-camp-vadodara-gujarat/).
* [Jun 14. Rust Meetup Vienna](https://www.eventbrite.com/e/rust-meetup-vienna-tickets-34958469724).
* [Jun 14. Rust Community Team Meeting at #rust-community on irc.mozilla.org](https://chat.mibbit.com/?server=irc.mozilla.org&channel=%23rust-community).
* [Jun 14. Rust Documentation Team Meeting at #rust-docs on irc.mozilla.org](https://chat.mibbit.com/?server=irc.mozilla.org&channel=%23rust-docs).
* [Jun 14. OpenTechSchool Berlin - Rust Hack and Learn](https://www.meetup.com/opentechschool-berlin/events/240113597/).
* [Jun 15. Rust DC Learn + Try: Embedded Rust](https://www.meetup.com/RustDC/events/239115658/).
* [Jun 15. Rust release triage](https://internals.rust-lang.org/t/release-cycle-triage-proposal/3544).
* [Jun 16. RainOfRust Camp Nashik - III](https://reps.mozilla.org/e/rainofrust-camp-nashik-iii/).
* [Jun 17. RainOfRust Camp Gandhinagar, Gujarat](https://reps.mozilla.org/e/rainofrust-camp-gandhinagar-gujarat/).
* [Jun 17. Rust Activate - Ciudad de México](https://reps.mozilla.org/e/rust-activate/).
* [Jun 18. #RainOfRust Workshop in Pune](https://reps.mozilla.org/e/rainofrust-workshop-in-pune/).
* [Jun 19. First Belgian Rust meetup](https://users.rust-lang.org/t/first-belgian-rust-meetup/11172).
* [Jun 21. Rust Meetup Dresden](https://www.meetup.com/Mozilla-Community-Dresden/events/240188745/).
* [Jun 21. Rust Community Team Meeting at #rust-community on irc.mozilla.org](https://chat.mibbit.com/?server=irc.mozilla.org&channel=%23rust-community).
* [Jun 21. Rust Documentation Team Meeting at #rust-docs on irc.mozilla.org](https://chat.mibbit.com/?server=irc.mozilla.org&channel=%23rust-docs).

If you are running a Rust event please add it to the [calendar] to get
it mentioned here. Email the [Rust Community Team][community] for access.

[calendar]: https://www.google.com/calendar/embed?src=apd9vmbc22egenmtu5l6c5jbfc%40group.calendar.google.com
[community]: mailto:community-team@rust-lang.org

# Rust Jobs

* [Open Source Rust Engineer at Buoyant](https://rustjobs.rs/jobs/24/buoyant-open-source-rust-engineer).
* [Rust Developer at 1aim](https://rustjobs.rs/jobs/22/1aim-gmbh-rust-developer).
* [Rust Developer at Anixe](https://rustjobs.rs/jobs/21/anixe-rust-developer).
* [Rust Legend at Between Lines](https://rustjobs.rs/jobs/20/between-lines-ltd-rust-legend).
* Student Research Assistant for developing Clippy in Karlsruhe (contact oliver.schneider \at kit.edu)

*Tweet us at [@ThisWeekInRust](https://twitter.com/ThisWeekInRust) to get your job offers listed here!*

# Quote of the Week

> Nothing to worry about, if you ask me. There's no official "Rust ideology".
>
> All you have to do is to accept the message of memory safety and swear allegiance to Our Lord and Savior, Rust programming language, protector of the highly parallel and the most efficient. Avoid the sin of unsafety, respect the lifetimes, mark your path with Send and Sync, and you too can become a member of Rust Evangelism Strike Force.

— [/u/dpc_pw on reddit](https://www.reddit.com/r/rust/comments/6ewjt5/question_about_rusts_odd_code_of_conduct/didok4h/).

Thanks to [/u/caramba2654](https://www.reddit.com/r/rust/comments/6ewjt5/question_about_rusts_odd_code_of_conduct/didqcfz/) for the suggestion.

[Submit your quotes for next week][submit]!

[submit]: http://users.rust-lang.org/t/twir-quote-of-the-week/328

*This Week in Rust is edited by: [nasa42](https://github.com/nasa42), [llogiq](https://github.com/llogiq), and [brson](https://github.com/brson).*
