Title: This Week in Rust 194
Number: 194
Date: 2017-08-08
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

* [Revisiting Rust’s modules, part 2](https://internals.rust-lang.org/t/revisiting-rust-s-modules-part-2/5700).
* [RustFest 2017: Supporter tickets on-sale, diversity ticket applications open](http://blog.rustfest.eu/this-week-in-rustfest-5-tickets-diversity).
* [JetBrains announces official support for Rust plugin for IntelliJ IDEA, CLion, and other JetBrains IDEs](https://blog.jetbrains.com/blog/2017/08/04/official-support-for-open-source-rust-plugin-for-intellij-idea-clion-and-other-jetbrains-ides/).
* [Building a mobile app in Rust and React Native - part 1](https://medium.com/@marekkotewicz/building-a-mobile-app-in-rust-and-react-native-part-1-project-setup-b8dbcf3f539f).
* [Asynchronous Rust: complaints & suggestions](https://pro.theta.eu.org/2017/08/04/async-rust.html).
* [A Stratego interpreter in Rust](http://blog.jeffsmits.net/compsci/2017/08/06/a-stratego-interpreter-in-rust/). Building a faster interpreter for an old language in Rust.
* [Evolution of a simple `du -s` clone](https://durka.github.io/blog/2017/08/06/du-evolution.html).
* [Compile-time safety is for everybody](https://www.tockos.org/blog/2017/apsys-paper/). Follow-up to [Ownership is theft](http://amitlevy.com/papers/tock-plos2015.pdf).
* [Fearless concurrency with hazard pointers](https://ticki.github.io/blog/fearless-concurrency-with-hazard-pointers/).
* [Scrapmetal — Scrap your Rust boilerplate](http://fitzgeraldnick.com/2017/08/03/scrapmetal.html).
* [Rust: Optimising decoder experience](https://codecs.multimedia.cx/2017/08/rust-optimising-decoder-experience/). Follow-up to [Rust: Not so great for codec implementing](https://codecs.multimedia.cx/?p=1246).
* [This week in Rust docs 67](https://guillaumegomez.github.io/this-week-in-rust-docs/blog/this-week-in-rust-docs-67).

# Crate of the Week

This week's crate is [aesni](https://crates.io/crates/aesni), a crate providing a Rust AES (Rijndael) block ciphers
implementation using AES-NI. Thanks to [newpavlov](https://users.rust-lang.org/u/newpavlov) for the suggestion.

[Submit your suggestions and votes for next week][submit_crate]!

[submit_crate]: https://users.rust-lang.org/t/crate-of-the-week/2704

# Call for Participation

Always wanted to contribute to open-source projects but didn't know where to start?
Every week we highlight some tasks from the Rust community for you to pick and get started!

Some of these tasks may also have mentors available, visit the task page for more information.

* [PumpkinDB: Rust nightly after 2017-06-20 affects benchmarks negatively](https://github.com/PumpkinDB/PumpkinDB/issues/345). ([Discuss here](https://gitter.im/PumpkinDB/Lobby)).
* [easy] [gimli: Improve error handling in dwarfdump](https://github.com/gimli-rs/gimli/issues/231). gimli is a lazy, zero-copy parser for the DWARF debugging format.
* [wayland-window: Add control buttons](https://github.com/Smithay/wayland-window/issues/4).
* [wayland-window: Make borders prettier](https://github.com/Smithay/wayland-window/issues/19).
* [doc] [lyon: API guidelines: methods on collections that produce iterators follow the iter, iter_mut, into_iter conventions](https://github.com/nical/lyon/issues/86). Lyon is a GPU-based 2D graphics rendering engine in Rust.
* [doc] [lyon: API guidelines: ad-hoc conversions follow as_, to_, into_ conventions](https://github.com/nical/lyon/issues/85).
* [doc] [lyon: API guidelines: iterator type names should match the methods that produce them](https://github.com/nical/lyon/issues/87).
* [doc] [lyon: API guidelines: return error type from functions instead of empty struct](https://github.com/nical/lyon/issues/88).
* [medium] [lyon: Implement clipping line joins at the miter limit](https://github.com/nical/lyon/issues/35).
* [less easy] [bindgen: Emitting or deriving trait implementations](https://github.com/rust-lang-nursery/rust-bindgen/issues/886).
* [less easy] [bindgen: Emit a "manual" implementation of Debug when it cannot be derived](https://github.com/rust-lang-nursery/rust-bindgen/issues/875).
* [less easy] [bindgen: "manually" implement Hash when it cannot be derived](https://github.com/rust-lang-nursery/rust-bindgen/issues/877).
* [less easy] [bindgen: "manually" implement PartialEq when it cannot be derived](https://github.com/rust-lang-nursery/rust-bindgen/issues/879).
* [less easy] [bindgen: Derive `Eq` when possible](https://github.com/rust-lang-nursery/rust-bindgen/issues/880).
* [less easy] [bindgen: "manually" implement Eq when we cannot derive it](https://github.com/rust-lang-nursery/rust-bindgen/issues/881).
* [less easy] [bindgen: Derive PartialOrd when possible](https://github.com/rust-lang-nursery/rust-bindgen/issues/882).
* [less easy] [bindgen: "manually" implement PartialOrd when we cannot derive it](https://github.com/rust-lang-nursery/rust-bindgen/issues/883).
* [less easy] [bindgen: Derive Ord when possible](https://github.com/rust-lang-nursery/rust-bindgen/issues/884).
* [less easy] [bindgen: "manually" implement Ord when we cannot derive it](https://github.com/rust-lang-nursery/rust-bindgen/issues/885).
* [doc] [rust-ffi-guide: Make the book more consistent](https://github.com/Michael-F-Bryan/rust-ffi-guide/issues/8).
* [easy] [ggez: Input doesn't work on mac using tmux and iterm2](https://github.com/ggez/ggez/issues/30). ggez is a Rust library to create good games easily.
* [easy] [ggez: SDL controller input doesn't work](https://github.com/ggez/ggez/issues/35).
* [doc] [ggez: Finish full building-and-install docs for each platform](https://github.com/ggez/ggez/issues/118).

If you are a Rust project owner and are looking for contributors, please submit tasks [here][guidelines].

[guidelines]: https://users.rust-lang.org/t/twir-call-for-participation/4821

# Updates from Rust Core

105 pull requests were [merged in the last week][merged]

[merged]: https://github.com/search?q=is%3Apr+org%3Arust-lang+is%3Amerged+merged%3A2017-07-31..2017-08-07

* [rewrite large float math in Rust and use it for stable compile-time evaluation](https://github.com/rust-lang/rust/pull/43554)
* [borrowck: skip CFG construction when there is nothing to propagate](https://github.com/rust-lang/rust/pull/43547) (awesome memory savings)
* [cycle-free dependency graph](https://github.com/rust-lang/rust/pull/43590)
* [fix instability in import suggestions](https://github.com/rust-lang/rust/pull/43552) (alas, re-exports still aren't correctly filtered)
* [fix quadratic performance on `use` statements](https://github.com/rust-lang/rust/pull/43584)
* [save-analysis fixes](https://github.com/rust-lang/rust/pull/43533)
* [save subobligations in the projection cache](https://github.com/rust-lang/rust/pull/43546)
* [don't warn on unused `union` fields](https://github.com/rust-lang/rust/pull/43397)
* [error code & explanation for calling private methods from outside](https://github.com/rust-lang/rust/pull/43699)
* [improve error message for trying static dispatch on trait object](https://github.com/rust-lang/rust/pull/43600)
* [the case of the missing error codes](https://github.com/rust-lang/rust/pull/43709)
* [{`StdIn`, `StdOut`, `StdErr`}`.as_raw_fd()`](https://github.com/rust-lang/rust/pull/43459)
* [MIR Validate statement](https://github.com/rust-lang/rust/pull/43403) (hook for unsafe code guidelines validation via miri)
* [MIR don't build unused unwind cleanup blocks](https://github.com/rust-lang/rust/pull/43576)
* [MIR trans no longer ICEs on assignment errors](https://github.com/rust-lang/rust/pull/43568)
* [more parallelization between trans and LLVM](https://github.com/rust-lang/rust/pull/43506)
* [inline bitwise modification ops](https://github.com/rust-lang/rust/pull/43581)

## New Contributors

* Eric Daniels
* Mario Idival
* Ryan Leckey
* scalexm
* Tobias Schaffner
* Tymoteusz Jankowski

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

* [disposition: merge] [Allow an optional vert at the beginning of a match branch](https://github.com/rust-lang/rfcs/pull/1925).
* [disposition: merge] [Unsafe pointer methods](https://github.com/rust-lang/rfcs/pull/1966).
* [disposition: merge] [Amend RFC 1242 to require an RFC for deprecation of crates from the nursery](https://github.com/rust-lang/rfcs/pull/1983).
* [disposition: close] [Match branch semicolon](https://github.com/rust-lang/rfcs/pull/1994).
* [disposition: merge] [Future-proofing enums/structs with `#[non_exhaustive]` attribute](https://github.com/rust-lang/rfcs/pull/2008).
* [disposition: merge] [Enable nested method calls](https://github.com/rust-lang/rfcs/pull/2025).
* [disposition: close] [Zero-Sized References](https://github.com/rust-lang/rfcs/pull/2040).
* [disposition: merge] [Evolving Rust through checkpoints](https://github.com/rust-lang/rfcs/pull/2052).
* [disposition: close] [Allow use of pipe operator in patterns](https://github.com/rust-lang/rfcs/pull/1882).
* [disposition: merge] [Generic associated types (associated type constructors)](https://github.com/rust-lang/rfcs/pull/1598).

## New RFCs

* [Non-lexical lifetimes](https://github.com/rust-lang/rfcs/pull/2094).
* [Infer `T: 'x` outlives requirements on structs](https://github.com/rust-lang/rfcs/pull/2093).

## Style RFCs

[Style RFCs](https://github.com/rust-lang-nursery/fmt-rfcs) are part of the process for deciding on style guidelines for the Rust community and defaults for [Rustfmt](https://github.com/rust-lang-nursery/rustfmt). The process is similar to the RFC process, but we try to reach rough consensus on issues (including a final comment period) before progressing to PRs. Just like the RFC process, all users are welcome to comment and submit RFCs. If you want to help decide what Rust code should look like, come get involved!

The RFC style is now the default style in Rustfmt - try it out and let us know what you think!

Currently being discussed:

* [Define short](https://github.com/rust-lang-nursery/fmt-rfcs/issues/47)
* [Special casing some macros](https://github.com/rust-lang-nursery/fmt-rfcs/issues/86)

# Upcoming Events

* [Aug 10. Rust release triage](https://internals.rust-lang.org/t/release-cycle-triage-proposal/3544).
* [Aug 10. Columbus Rust Society - Monthly meetup](https://www.meetup.com/columbus-rs/events/czcwhlywlbnb/).
* [Aug 14. Seattle Rust Meetup](https://www.meetup.com/Seattle-Rust-Meetup/events/241535500/).
* [Aug 16. Rust Community Team Meeting at #rust-community on irc.mozilla.org](https://chat.mibbit.com/?server=irc.mozilla.org&channel=%23rust-community).
* [Aug 16. Rust Documentation Team Meeting at #rust-docs on irc.mozilla.org](https://chat.mibbit.com/?server=irc.mozilla.org&channel=%23rust-docs).
* **[Aug 18-19. RustConf 2017](http://rustconf.com/)**.
* [Aug 23. GOTO Night Berlin: Modern low level - Rust in 2017](https://www.meetup.com/GOTO-Nights-Berlin/events/241544422/).
* [Aug 23. OpenTechSchool Berlin: Rust Hack and Learn](https://www.meetup.com/opentechschool-berlin/events/242277432/).
* [Aug 23. Rust Community Team Meeting at #rust-community on irc.mozilla.org](https://chat.mibbit.com/?server=irc.mozilla.org&channel=%23rust-community).
* [Aug 23. Rust Documentation Team Meeting at #rust-docs on irc.mozilla.org](https://chat.mibbit.com/?server=irc.mozilla.org&channel=%23rust-docs).
* [Aug 24. Rust release triage](https://internals.rust-lang.org/t/release-cycle-triage-proposal/3544).

If you are running a Rust event please add it to the [calendar] to get
it mentioned here. Email the [Rust Community Team][community] for access.

[calendar]: https://www.google.com/calendar/embed?src=apd9vmbc22egenmtu5l6c5jbfc%40group.calendar.google.com
[community]: mailto:community-team@rust-lang.org

# Rust Jobs

*No jobs listed for this week.*

*Tweet us at [@ThisWeekInRust](https://twitter.com/ThisWeekInRust) to get your job offers listed here!*

# Quote of the Week

> Nah, it's not you, it's the borrow checker.
>> Honey, it's not you, it's &mut me.
>>> You can borrow me, and you can change me, but you can't own me.

— [/u/staticassert, /u/ybx, and /u/paholg on reddit](https://www.reddit.com/r/rust/comments/6s8vhg/how_do_i_do_if_let_somex_selfbla_selfdobla/dlazidp/).

Thanks to [Matt Ickstadt](https://users.rust-lang.org/t/twir-quote-of-the-week/328/428) and [QuadDamaged](https://users.rust-lang.org/t/twir-quote-of-the-week/328/429) for the suggestion.

[Submit your quotes for next week][submit]!

[submit]: http://users.rust-lang.org/t/twir-quote-of-the-week/328

*This Week in Rust is edited by: [nasa42](https://github.com/nasa42), [llogiq](https://github.com/llogiq), and [brson](https://github.com/brson).*
