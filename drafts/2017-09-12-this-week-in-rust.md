Title: This Week in Rust 199
Number: 199
Date: 2017-09-12
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

* [Implementing the Read trait for strings](https://codingwithglee.blogspot.de/2017/09/a-stringreader-in-rust.html)

# Crate of the Week

This week's crate is [pikkr](https://github.com/pikkr/pikkr), a JSON parser that can extract values without tokenization and is blazingly fast using AVX2 instructions,
Thank you, [bstrie](https://users.rust-lang.org/u/bstrie) for the suggestion!

[Submit your suggestions and votes for next week][submit_crate]!

[submit_crate]: https://users.rust-lang.org/t/crate-of-the-week/2704

# Call for Participation

Always wanted to contribute to open-source projects but didn't know where to start?
Every week we highlight some tasks from the Rust community for you to pick and get started!

Some of these tasks may also have mentors available, visit the task page for more information.

* [Help test async/await/generators/coroutines](https://internals.rust-lang.org/t/help-test-async-await-generators-coroutines/5835).
* [medium] [allocators-rs: mmap-alloc: Support full Alloc API](https://github.com/ezrosent/allocators-rs/issues/9).
* [medium] [allocators-rs: bsalloc: Support allocation failures](https://github.com/ezrosent/allocators-rs/issues/4).
* [easy] [allocators-rs: Add links in documentation](https://github.com/ezrosent/allocators-rs/issues/1).
* [medium] [allocators-rs: Travis: Spurious test failures on Mac](https://github.com/ezrosent/allocators-rs/issues/36).
* [easy] [bindgen: Add `bindgen::Builder::derive_copy` to control whether we emit `derive(Copy)` on type definitions](https://github.com/rust-lang-nursery/rust-bindgen/issues/948).
* [medium] [sysconf: page: Add default hugepage support on Linux](https://github.com/ZeroCostGoods/sysconf.rs/issues/7).
* [rust-machine-id: windows: add implementation](https://github.com/mathstuf/rust-machine-id/pull/2).

If you are a Rust project owner and are looking for contributors, please submit tasks [here][guidelines].

[guidelines]: https://users.rust-lang.org/t/twir-call-for-participation/4821

# Updates from Rust Core

99 pull requests were [merged in the last week][merged]

[merged]: https://github.com/search?q=is%3Apr+org%3Arust-lang+is%3Amerged+merged%3A2017-09-04..2017-09-11

* [improved message on `&str` vs. `&[u8]` literals](https://github.com/rust-lang/rust/pull/44361)
* [hint on overlapping inter-crate ambiguities](https://github.com/rust-lang/rust/pull/43426)
* [`#![feature(drop_types_in_const)]`](https://github.com/rust-lang/rust/pull/44212)
* [proper expansion info for more builtin macros](https://github.com/rust-lang/rust/pull/44248)
* [macros 2.0 now have their `Span` include visibility modifiers](https://github.com/rust-lang/rust/pull/44375)
* [use `NodeId`/`HirId` instead of `DefId` for local vars](https://github.com/rust-lang/rust/pull/44316)
* [avoid hashing every `HirId` in existence](https://github.com/rust-lang/rust/pull/44335)
* [`SplitWhitespace` now implements `Debug`](https://github.com/rust-lang/rust/pull/44303)
* [`_.clamp(min, max)` for `Ord` types](https://github.com/rust-lang/rust/pull/44097)
* [panic on overflow in `Instance` ± `Duration`](https://github.com/rust-lang/rust/pull/44220)
* [the `LocalKey` facade of `thread_local!` is now inlineable cross-crate](https://github.com/rust-lang/rust/pull/43931)
* [avoid creating `static`s for each `panic`](https://github.com/rust-lang/rust/pull/44312)
* [MIR no longer emits `EndRegion`s by default](https://github.com/rust-lang/rust/pull/44249)
* [MIR: restrict `ProjectionElem::Index` and `Storage`{`Live`, `Dead`} to `Local`](https://github.com/rust-lang/rust/pull/44308)
* [MIR: no longer inlines trait methods](https://github.com/rust-lang/rust/pull/44383)
* [MIR: inliner bug fixed](https://github.com/rust-lang/rust/pull/44362)
* [macOS users can get backtraces again](https://github.com/rust-lang/rust/pull/44251)
* [fix macOs segfault](https://github.com/rust-lang/rust/pull/44384)
* [more metadata methods are queries](https://github.com/rust-lang/rust/pull/44142)
* [`rustc_metadata` no longer needs `DepGraph` handling, remove it](https://github.com/rust-lang/rust/pull/44418) (now querified)
* [rustc now deals correctly with really long linker commands](https://github.com/rust-lang/rust/pull/44094)
* [rustbuild can use hardlinks again, reduces copies](https://github.com/rust-lang/rust/pull/44260) (my small SSD rejoices)
* [cargo: hash dependencies of metadata into lib's metadata](https://github.com/rust-lang/cargo/pull/4469)
* [cargo: don't loop forever on cyclical features](https://github.com/rust-lang/cargo/pull/4473)
* [cargo: support vendoring git repositories](https://github.com/rust-lang/cargo/pull/3992)

## New Contributors

* Andrew Gauger
* Andy Gauge
* Jeremy Sorensen
* Lukas H
* Phlosioneer

## Approved RFCs

Changes to Rust follow the Rust [RFC (request for comments)
process](https://github.com/rust-lang/rfcs#rust-rfcs). These
are the RFCs that were approved for implementation this week:

* [Clamp functions](https://github.com/rust-lang/rfcs/pull/1961).
* [Generic associated types (associated type constructors)](https://github.com/rust-lang/rfcs/pull/1598).

## Final Comment Period

Every week [the team](https://www.rust-lang.org/team.html) announces the
'final comment period' for RFCs and key PRs which are reaching a
decision. Express your opinions now. [This week's FCPs][fcp] are:

[fcp]: https://github.com/rust-lang/rfcs/labels/final-comment-period

* [disposition: merge] [Clarify and streamline paths and visibility](https://github.com/rust-lang/rfcs/pull/2126).
* [disposition: merge] [Nested groups in imports](https://github.com/rust-lang/rfcs/pull/2128).
* [disposition: postpone] [Add the `()` → `Result<(), _>` coercion rule, for removing `Ok(())` everywhere](https://github.com/rust-lang/rfcs/pull/2120).
* [disposition: merge] [In-band lifetime bindings](https://github.com/rust-lang/rfcs/pull/2115).
* [disposition: merge] [Autoreferencing `Copy` types](https://github.com/rust-lang/rfcs/pull/2111).
* [disposition: postpone] [Ok wrapping: Improved support for writing code from an error handling mindset](https://github.com/rust-lang/rfcs/pull/2107).
* [disposition: merge] [Attributes for tools, 2.0](https://github.com/rust-lang/rfcs/pull/2103).
* [disposition: merge] [Infer `T: 'x` outlives requirements on structs](https://github.com/rust-lang/rfcs/pull/2093).
* [disposition: merge] [Implied bounds](https://github.com/rust-lang/rfcs/pull/2089).
* [disposition: merge] [Allow Irrefutable Patterns in if-let and while-let statements](https://github.com/rust-lang/rfcs/pull/2086).
* [disposition: merge] [Add impl Trait type alias and variable declarations](https://github.com/rust-lang/rfcs/pull/2071).
* [disposition: merge] [stable mechanism to specify the behavior of panic! in no-std applications](https://github.com/rust-lang/rfcs/pull/2070).
* [disposition: merge] [Evolving Rust through Epochs](https://github.com/rust-lang/rfcs/pull/2052).
* [disposition: merge] [Add `align_offset` intrinsic and `[T]::align_to` function](https://github.com/rust-lang/rfcs/pull/2043).
* [disposition: postpone] [Const/static type annotation elision](https://github.com/rust-lang/rfcs/pull/2010).
* [disposition: merge] [Const generics](https://github.com/rust-lang/rfcs/pull/2000).
* [disposition: merge] [Add external doc attribute to rustc](https://github.com/rust-lang/rfcs/pull/1990).
* [disposition: close] [Allow crates to specify the version of Rust in which they are written](https://github.com/rust-lang/rfcs/pull/1709).
* [disposition: merge] [Copy/Clone closures](https://github.com/rust-lang/rfcs/pull/2132). Implement `Clone` and `Copy` for closures where possible.
* [disposition: merge] [Compiler-generated Clone impls for arrays and tuples](https://github.com/rust-lang/rfcs/pull/2133).

## New RFCs

* [eRFC: Cargo build system integration](https://github.com/rust-lang/rfcs/pull/2136).
* [Support defining C-compatible variadic functions in Rust](https://github.com/rust-lang/rfcs/pull/2137).

## Style RFCs

[Style RFCs](https://github.com/rust-lang-nursery/fmt-rfcs) are part of the process for deciding on style guidelines for the Rust community and defaults for [Rustfmt](https://github.com/rust-lang-nursery/rustfmt). The process is similar to the RFC process, but we try to reach rough consensus on issues (including a final comment period) before progressing to PRs. Just like the RFC process, all users are welcome to comment and submit RFCs. If you want to help decide what Rust code should look like, come get involved!

The RFC style is now the default style in Rustfmt - try it out and let us know what you think!

We're currently writing up the discussions, we'd love some help. Check out [the tracking issue](https://github.com/rust-lang-nursery/fmt-rfcs/issues/89) for details.

PRs:

* [ranges and blocks](https://github.com/rust-lang-nursery/fmt-rfcs/pull/91)

# Upcoming Events

* [Sep  7. Rust release triage](https://internals.rust-lang.org/t/release-cycle-triage-proposal/3544).
* [Sep 11. Seattle Rust Monthly Meetup](https://www.meetup.com/Seattle-Rust-Meetup/events/242563613/).
* [Sep 12. Rust Berlin Meetup - September 2017](https://www.meetup.com/Rust-Berlin/events/242564404/).
* [Sep 13. Rust Community Team Meeting at #rust-community on irc.mozilla.org](https://chat.mibbit.com/?server=irc.mozilla.org&channel=%23rust-community).
* [Sep 13. Rust Documentation Team Meeting at #rust-docs on irc.mozilla.org](https://chat.mibbit.com/?server=irc.mozilla.org&channel=%23rust-docs).
* [Sep 14. Rust Washington, DC - Hacktember](https://www.meetup.com/RustDC/events/242847065/).
* [Sep 14. Columbus Rust Society - Monthly Meeting](https://www.meetup.com/columbus-rs/events/242459785/).
* [Sep 20. Rust Community Team Meeting at #rust-community on irc.mozilla.org](https://chat.mibbit.com/?server=irc.mozilla.org&channel=%23rust-community).
* [Sep 20. Rust Documentation Team Meeting at #rust-docs on irc.mozilla.org](https://chat.mibbit.com/?server=irc.mozilla.org&channel=%23rust-docs).
* [Sep 20. OpenTechSchool Berlin - Rust Hack and Learn](https://www.meetup.com/opentechschool-berlin/events/242793549/).
* [Sep 21. Rust release triage](https://internals.rust-lang.org/t/release-cycle-triage-proposal/3544).
* [Sep 30. - Oct 1. RustFest Zürich](http://zurich.rustfest.eu).
* [Oct 2.-3. Impl Days at RustFest Zürich](https://github.com/RustFestEU/blog.rustfest.eu/issues/29).

If you are running a Rust event please add it to the [calendar] to get
it mentioned here. Email the [Rust Community Team][community] for access.

[calendar]: https://www.google.com/calendar/embed?src=apd9vmbc22egenmtu5l6c5jbfc%40group.calendar.google.com
[community]: mailto:community-team@rust-lang.org

# Rust Jobs

* [Rust Systems Engineer at Immunant](http://immunant.com/page/002_rustacean/).
* [Sr. Software Development Engineer at Amazon](https://www.amazon.jobs/en/jobs/559813/sr-software-development-engineer).

*Tweet us at [@ThisWeekInRust](https://twitter.com/ThisWeekInRust) to get your job offers listed here!*

# Quote of the Week

> you can ask a Future “are we there yet”, to which it can answer “yes”, “no”, or "don’t make me come back there"
> an Iterator is something you can keep asking “more?” until it gets fed up and stops listening
> Display is just a way to say “show me your moves”, with the other formatting traits being other dance moves
> if something isn’t Send, then it’s a cursed item you can’t give away, it’s yours to deal with
> if something isn’t Sync, then it won’t even appear for other people, it’s possibly an apparition inside your head
> things that are Clone can reproduce asexually, but only on command. things that are Copy won’t bother waiting for you

— [@QuietMisdreavus on Twitter](https://twitter.com/QuietMisdreavus/status/903071042834489344).

Thanks to [Havvy](https://users.rust-lang.org/t/twir-quote-of-the-week/328/441) for the suggestion.

[Submit your quotes for next week][submit]!

[submit]: http://users.rust-lang.org/t/twir-quote-of-the-week/328

*This Week in Rust is edited by: [nasa42](https://github.com/nasa42), [llogiq](https://github.com/llogiq), and [brson](https://github.com/brson).*
