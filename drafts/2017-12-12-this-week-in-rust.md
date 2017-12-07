Title: This Week in Rust 212
Number: 212
Date: 2017-12-12
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

* [Conference talk at Cycon 2017] [Forensic tool development with Rust](https://www.youtube.com/watch?v=wAHjiWt8XPY&list=PLV8RTnZwQxclg8-tvg-JG-_RwL2EBvOiP&index=25) Fast forward to minute 36:55.

# Crate of the Week

This week is a bit sad for lack of a crate. Look, if you want a weekly crate, [submit your suggestions and votes for next week][submit_crate]!

[submit_crate]: https://users.rust-lang.org/t/crate-of-the-week/2704

# Call for Participation

Always wanted to contribute to open-source projects but didn't know where to start?
Every week we highlight some tasks from the Rust community for you to pick and get started!

Some of these tasks may also have mentors available, visit the task page for more information.

* [Contribute to Rust's 2017 impl period](https://www.rustaceans.org/findwork/impl).

If you are a Rust project owner and are looking for contributors, please submit tasks [here][guidelines].

[guidelines]: https://users.rust-lang.org/t/twir-call-for-participation/4821

# Updates from Rust Core

146 pull requests were [merged in the last week][merged]

[merged]: https://github.com/search?q=is%3Apr+org%3Arust-lang+is%3Amerged+merged%3A2017-11-27..2017-12-04

* [allow nested groups in imports](https://github.com/rust-lang/rust/pull/45846)
* [add an i128_lowering flag in TargetOptions](https://github.com/rust-lang/rust/pull/46486)
* [implement the special repr(C)-non-clike-enum layout](https://github.com/rust-lang/rust/pull/46123)
* [rustc: filter out bogus extern crate warnings](https://github.com/rust-lang/rust/pull/46405)
* [rustc: prepare to enable ThinLTO by default](https://github.com/rust-lang/rust/pull/46382)
* [incr.comp.: make traits::VTable encodable and decodable](https://github.com/rust-lang/rust/pull/46400)
* [incr.comp.: remove ability to produce incr. comp. hashes during metadata export](https://github.com/rust-lang/rust/pull/46370)
* [incr.comp.: remove an unnecessary HIR access which enables hashing spans for type definitions](https://github.com/rust-lang/rust/pull/46368)
* [incr.comp.: load cached diagnostics lazily and allow more things in the cache](https://github.com/rust-lang/rust/pull/46338)
* [incr.comp.: some preparatory work for caching more query results](https://github.com/rust-lang/rust/pull/46299)
* [make coercions to `!` in unreachable code a hard error](https://github.com/rust-lang/rust/pull/45880)
* [stabilize const-calling existing const-fns in std](https://github.com/rust-lang/rust/pull/46287)
* [remove semicolon note](https://github.com/rust-lang/rust/pull/46258)
* [use suggestions instead of notes ref mismatches](https://github.com/rust-lang/rust/pull/46256) (for better tooling)
* [avoid type-live-for-region obligations on dummy nodes](https://github.com/rust-lang/rust/pull/46226)
* [suggest using slice when encountering `let _ = ""[..];`](https://github.com/rust-lang/rust/pull/46249)
* [add case insensitive comparison, besides Levenstein for DYM](https://github.com/rust-lang/rust/pull/46347)
* [MIR: split Operand::Consume into Copy and Move](https://github.com/rust-lang/rust/pull/46142)
* [MIR: Fix value moved diagnose messages](https://github.com/rust-lang/rust/pull/46231)
* [MIR: Fix CopyPropagation regression (2)](https://github.com/rust-lang/rust/pull/46462)
* [MIR borrowck: finalize `check_access_permissions()`](https://github.com/rust-lang/rust/pull/46041)
* [MIR-borrowck: immutable unique closure upvars can be mutated](https://github.com/rust-lang/rust/pull/46236)
* [disable jemalloc on executables for ios targets](https://github.com/rust-lang/rust/pull/46211)
* [stabilize `spin_loop_hint`](https://github.com/rust-lang/rust/pull/46174)
* [add a specialization of read_exact for Cursor](https://github.com/rust-lang/rust/pull/46485)
* [reject '2' as a binary digit in internals of b: number formatting](https://github.com/rust-lang/rust/pull/46356)
* [remove `T: Sized` on `ptr::is_null()`](https://github.com/rust-lang/rust/pull/46094)
* [stabilize some `ascii_ctype` methods](https://github.com/rust-lang/rust/pull/46077)
* [add std::sync::mpsc::Receiver::recv_deadline()](https://github.com/rust-lang/rust/pull/45969)
* [generic Associated Types Parsing & Name Resolution](https://github.com/rust-lang/rust/pull/45904)
* [`impl From<bool> for AtomicBool`](https://github.com/rust-lang/rust/pull/46293)
* [implement `From<RecvError>` for `TryRecvError` and `RecvTimeoutError`](https://github.com/rust-lang/rust/pull/45506)
* [deprecate the Formatter::flags method](https://github.com/rust-lang/rust/pull/46284)
* [introduce `LinkedList::drain_filter`](https://github.com/rust-lang/rust/pull/46262)
* [cargo: add a workspace.default-members config that overrides implied --all ](https://github.com/rust-lang/cargo/pull/4743)
* [rustdoc: fix search results overlap](https://github.com/rust-lang/rust/pull/46454)
* [rustdoc: fix deduplication of items](https://github.com/rust-lang/rust/pull/46433)
* [rustdoc: hide private trait type params and show hidden items with document-private](https://github.com/rust-lang/rust/pull/46412)
* [fix rustdoc item summaries that are headers](https://github.com/rust-lang/rust/pull/46387)
* [rustdoc: fix global search](https://github.com/rust-lang/rust/pull/46175)

## New Contributors

* Christian Duerr
* Irina-Gabriela Popa
* Julian Kulesh
* Kenjiro Nakayama
* Kyle Huey
* Nikolay Merinov

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

* [disposition: merge] [Fallible collection allocation 1.0](https://github.com/rust-lang/rfcs/pull/2116).
* [disposition: merge] [Implicit caller location (third try to the unwrap/expect line info problem)](https://github.com/rust-lang/rfcs/pull/2091).
* [disposition: merge] [Unsized rvalues](https://github.com/rust-lang/rfcs/pull/1909).
* [disposition: merge] [eRFC: Cargo build system integration](https://github.com/rust-lang/rfcs/pull/2136).
* [disposition: merge] [Type privacy and private-in-public lints](https://github.com/rust-lang/rfcs/pull/2145).

## New RFCs

* [Closures capture disjoint fields](https://github.com/rust-lang/rfcs/pull/2229).
* [Bury `Error::description()`](https://github.com/rust-lang/rfcs/pull/2230).
* [String reflection](https://github.com/rust-lang/rfcs/pull/2233).
* [Add a machine-readable JSON-output mode for Rust's libtest](https://github.com/rust-lang/rfcs/pull/2234).

# Upcoming Events

* [Dec 11. Seattle Rust Meetup](https://www.meetup.com/Seattle-Rust-Meetup/events/svbqbmywqbpb/).
* [Dec 13. Rust Amsterdam: Theme night on Procedural Macros & Custom Derive](https://www.meetup.com/Rust-Amsterdam/events/245075721/)
* [Dec 13. Rust Community Team Meeting at #rust-community on irc.mozilla.org](https://chat.mibbit.com/?server=irc.mozilla.org&channel=%23rust-community).
* [Dec 13. Rust Documentation Team Meeting at #rust-docs on irc.mozilla.org](https://chat.mibbit.com/?server=irc.mozilla.org&channel=%23rust-docs).
* [Dec 13. OpenTechSchool Berlin - Rust Hack and Learn](https://www.meetup.com/opentechschool-berlin/events/krnczlywqbrb/).
* [Dec 14. Rust release triage](https://internals.rust-lang.org/t/release-cycle-triage-proposal/3544).
* [Dec 14. Rust DC - Mid-month Rustful: Falcon](https://www.meetup.com/RustDC/events/243672324/).
* [Dec 14. Columbus Rust Society - Monthly Meeting](https://www.meetup.com/columbus-rs/events/czcwhlywqbsb/).
* [Dec 20. Rust Community Team Meeting at #rust-community on irc.mozilla.org](https://chat.mibbit.com/?server=irc.mozilla.org&channel=%23rust-community).
* [Dec 20. Rust Documentation Team Meeting at #rust-docs on irc.mozilla.org](https://chat.mibbit.com/?server=irc.mozilla.org&channel=%23rust-docs).
* [Dec 21. Cambridge Rust Meetup #6](https://www.meetup.com/Cambridge-Rust-Meetup/events/mgtcwnywqbcc/).

If you are running a Rust event please add it to the [calendar] to get
it mentioned here. Email the [Rust Community Team][community] for access.

[calendar]: https://www.google.com/calendar/embed?src=apd9vmbc22egenmtu5l6c5jbfc%40group.calendar.google.com
[community]: mailto:community-team@rust-lang.org

# Rust Jobs

*No jobs listed for this week.*

*Tweet us at [@ThisWeekInRust](https://twitter.com/ThisWeekInRust) to get your job offers listed here!*

# Quote of the Week

*No quote was selected for QotW.*

[Submit your quotes for next week][submit]!

[submit]: http://users.rust-lang.org/t/twir-quote-of-the-week/328

*This Week in Rust is edited by: [nasa42](https://github.com/nasa42) and [llogiq](https://github.com/llogiq).*
