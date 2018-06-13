Title: This Week in Rust 238
Number: 238
Date: 2018-06-12
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

* [Migrating to Actix from Rocket](https://noyez.gitlab.io/post/2018-06-11-rocket-to-actix/).

# Crate of the Week

This week's crate is [clap-verbosity-flag](https://crates.io/crates/clap-verbosity-flag), a small crate to easily add a verbosity setting to Rust command line applications. Thanks to [Yoshuawuyts](https://users.rust-lang.org/u/yoshuawuyts) for the suggestion!

[Submit your suggestions and votes for next week][submit_crate]!

[submit_crate]: https://users.rust-lang.org/t/crate-of-the-week/2704

# Call for Participation

Always wanted to contribute to open-source projects but didn't know where to start?
Every week we highlight some tasks from the Rust community for you to pick and get started!

Some of these tasks may also have mentors available, visit the task page for more information.

* [wasm-pack has several open good first issues available to new contributors](https://github.com/ashleygwilliams/wasm-pack/issues?q=is%3Aissue+is%3Aopen+label%3A%22help+wanted%22).
* [Get started with these beginner-friendly issues](https://www.rustaceans.org/findwork/starters).

If you are a Rust project owner and are looking for contributors, please submit tasks [here][guidelines].

[guidelines]: https://users.rust-lang.org/t/twir-call-for-participation/4821

# Updates from Rust Core

110 pull requests were [merged in the last week][merged]

[merged]: https://github.com/search?q=is%3Apr+org%3Arust-lang+is%3Amerged+merged%3A2018-06-04..2018-06-11

* [Keyword unreservations (pure, sizeof, alignof, offsetof)](https://github.com/rust-lang/rust/pull/51196) (RFC [#2421](https://rust-lang.github.io/rfcs/2421-unreservations-2018.html))
* [parser: split `+=` into `+` and `=` where `+` is explicitly requested (such as generics)](https://github.com/rust-lang/rust/pull/51068)
* [enable fall through past $:lifetime matcher](https://github.com/rust-lang/rust/pull/51480)
* [deny `#[cfg]` and `#[cfg_attr]` on generic parameters](https://github.com/rust-lang/rust/pull/51283)
* [include parens to type parameter](https://github.com/rust-lang/rust/pull/50205)
* [use scope tree depths to speed up `nearest_common_ancestor`](https://github.com/rust-lang/rust/pull/51394)
* [avoid useless Vec clones in `pending_obligations`](https://github.com/rust-lang/rust/pull/51412)
* [NLL performance boost](https://github.com/rust-lang/rust/pull/51399)
* [NLL: report type moved from behind borrow of array/slice](https://github.com/rust-lang/rust/pull/51247)
* [deduplicate auto traits in trait objects](https://github.com/rust-lang/rust/pull/51276)
* [remove dependency on fmt_macros from typeck](https://github.com/rust-lang/rust/pull/51380)
* [re-enable trivial bounds](https://github.com/rust-lang/rust/pull/51042)
* [use spans pointing at the inside of a rustdoc attribute](https://github.com/rust-lang/rust/pull/51391)
* [suggest parentheses when a struct literal needs them](https://github.com/rust-lang/rust/pull/51360)
* [suggest not mutably borrowing a mutable reference](https://github.com/rust-lang/rust/pull/51242)
* [add deprecation lint for duplicated `macro_export`s](https://github.com/rust-lang/rust/pull/50143)
* [accept `..` in incorrect position to avoid further errors](https://github.com/rust-lang/rust/pull/51201)
* [fix the use of closures within `#[panic_implementation]`](https://github.com/rust-lang/rust/pull/51368)
* [refactor the const eval diagnostic API](https://github.com/rust-lang/rust/pull/51316)
* [check array indices in constant propagation](https://github.com/rust-lang/rust/pull/51308)
* [`ScalarPairs` are offset==0 field + other non-zst field](https://github.com/rust-lang/rust/pull/51307/files)
* [blocking Rayon queries](https://github.com/rust-lang/rust/pull/50699/files)
* [reexport `fmt::Alignment` into `std`](https://github.com/rust-lang/rust/pull/51333)
* [add `Future` and task system to the standard library](https://github.com/rust-lang/rust/pull/51263)
* [futures: add a few blanket impls to `std`](https://github.com/rust-lang/rust/pull/51442)
* [fix confusing error message for sub_instant](https://github.com/rust-lang/rust/pull/51255)
* [stabilize `Iterator::step_by`](https://github.com/rust-lang/rust/pull/51320)
* [stabilize `iterator_repeat_with`](https://github.com/rust-lang/rust/pull/51200)
* [stabilize `entry-or-default`](https://github.com/rust-lang/rust/pull/51079)
* [stabilize unit tests with non-`()` return type](https://github.com/rust-lang/rust/pull/51298)
* [cargo: allow rustc bootstrap to use unstable features even though it's using a beta-cargo](https://github.com/rust-lang/cargo/pull/5613)
* [fix crate-name option in rustdoc](https://github.com/rust-lang/rust/pull/51256)
* [rustbuild: allow enabling incremental via config.toml](https://github.com/rust-lang/rust/pull/51317)
* [rustbuild: do not require stage 2 compiler for rustdoc](https://github.com/rust-lang/rust/pull/51436)

## Approved RFCs

Changes to Rust follow the Rust [RFC (request for comments)
process](https://github.com/rust-lang/rfcs#rust-rfcs). These
are the RFCs that were approved for implementation this week:

* [Amend 1105: Unstable features accidentally usable on the Stable release chanel are still unstable](https://github.com/rust-lang/rfcs/pull/2405).

## Final Comment Period

Every week [the team](https://www.rust-lang.org/team.html) announces the
'final comment period' for RFCs and key PRs which are reaching a
decision. Express your opinions now.

### [RFCs](https://github.com/rust-lang/rfcs/labels/final-comment-period)

*No RFCs are currently in final comment period.*

### [Tracking Issues & PRs](https://github.com/rust-lang/rust/labels/final-comment-period)

* [disposition: merge] [Tracking issue for the GlobalAlloc trait and related APIs](https://github.com/rust-lang/rust/issues/49668).
* [disposition: merge] [Stabilize GlobalAlloc and `#[global_allocator]`](https://github.com/rust-lang/rust/pull/51241).
* [disposition: merge] [Tracking issue for `ToOwned::clone_into` (`toowned_clone_into`)](https://github.com/rust-lang/rust/issues/41263).
* [disposition: merge] [Tracking issue for "macro naming and modularisation" (RFC #1561)](https://github.com/rust-lang/rust/issues/35896).
* [disposition: merge] [Tracking issue for promoting `!` to a type (RFC 1216)](https://github.com/rust-lang/rust/issues/35121).
* [disposition: merge] [Exhaustive integer matching](https://github.com/rust-lang/rust/pull/50912).
* [disposition: merge] [Stabilize `std::path::Path::ancestors`](https://github.com/rust-lang/rust/pull/50894).
* [disposition: merge] [Add ability to apply custom derive to union types](https://github.com/rust-lang/rust/pull/50383).

## New RFCs

* [Re-Rebalancing Coherence](https://github.com/rust-lang/rfcs/pull/2451).
* [Allow non-ASCII identifiers](https://github.com/rust-lang/rfcs/pull/2457).
* [Unused const fn results](https://github.com/rust-lang/rfcs/pull/2450).

# Upcoming Events

* [Jun 10. Mountain View, US - Open Table / Icebreaker: what projects are you working on](https://www.meetup.com/Rust-Dev-in-Mountain-View/events/glnfcpyxjbnb/).
* [Jun 11. Zürich, CH - Actix.rs - July Meetup](https://www.meetup.com/de-DE/Rust-Zurich/events/250386292/).
* [Jun 11. Seattle, US - Monthly meetup](https://www.meetup.com/Seattle-Rust-Meetup/events/hztzcpyxjbpb/).
* [Jun 12. Rome, IT - Rust learning and hacking evening #9](https://www.meetup.com/Rust-Roma/events/251298815/).
* [Jun 13. Berlin, DE - OpenTechSchool - Rust Hack and Learn](https://www.meetup.com/opentechschool-berlin/events/250904450/).
* [Jun 13. Rust Community Team Meeting at #rust-community on irc.mozilla.org](irc://irc.mozilla.org/rust-community).
* [Jun 13. Vancouver, CA - Rust Study/Hack/Hang-out night](https://www.meetup.com/Vancouver-Rust/events/dqldspyxjbrb/).
* [Jun 14. Columbus, US - Columbus Rust Society - Monthly Meeting](https://www.meetup.com/columbus-rs/events/dbcfrpyxjbsb/).
* [Jun 14. San Diego, US - San Diego Rust June Meetup](https://www.meetup.com/San-Diego-Rust/events/251001684/).
* [Jun 14. Utah Valley, US - Utah Rust meetup](https://docs.google.com/document/d/1O8S7IEfDw-3jTN74CWCuKYl_UWxTLd6-epz7NOMDYRg).
* [Jun 17. Mountain View, US - Open Table / Icebreaker: what projects are you working on](https://www.meetup.com/Rust-Dev-in-Mountain-View/events/glnfcpyxjbwb/).
* [Jun 19. Denver, US - Rust Boulder/Denver - June Meetup in Boulder](https://www.meetup.com/Rust-Boulder-Denver/events/250076478/).
* [Jun 19. Rust Community Content Subteam Meeting at #rust-content on irc.mozilla.org](irc://irc.mozilla.org/rust-content).
* [Jun 20. Rust Events Team Meeting](https://t.me/joinchat/EkKINhHCgZ9llzvPidOssA).
* [Jun 20. Rust Community Team Meeting at #rust-community on irc.mozilla.org](irc://irc.mozilla.org/rust-community).
* [Jun 21. Cambridge, GB - Cambridge Rust Meetup](https://www.meetup.com/Cambridge-Rust-Meetup/events/pzwshpyxjbcc/).
* **[Aug 17. Portland, US - RustConf 2018](http://rustconf.com/).** Registration is now open.

If you are running a Rust event please add it to the [calendar] to get
it mentioned here. Email the [Rust Community Team][community] for access.

[calendar]: https://www.google.com/calendar/embed?src=apd9vmbc22egenmtu5l6c5jbfc%40group.calendar.google.com
[community]: mailto:community-team@rust-lang.org

# Rust Jobs

* [Senior Backend Engineer at ClanHQ, San Francisco (remote available)](https://twitter.com/JonathanBelolo/status/1000128978936623104).
* [Rust Developer at 1am, Berlin](https://twitter.com/__1aim/status/1002493500099833856).

*Tweet us at [@ThisWeekInRust](https://twitter.com/ThisWeekInRust) to get your job offers listed here!*

# Quote of the Week

> explicit lifetimes no longer scare me the way they used to.

– Nicholas Nethercote on [his blog](https://blog.mozilla.org/nnethercote/2018/06/05/how-to-speed-up-the-rust-compiler-some-more-in-2018)

(selected by llogiq per one unanimous vote)

[Please submit your quotes for next week][submit]!

[submit]: http://users.rust-lang.org/t/twir-quote-of-the-week/328

*This Week in Rust is edited by: [nasa42](https://github.com/nasa42) and [llogiq](https://github.com/llogiq).*
