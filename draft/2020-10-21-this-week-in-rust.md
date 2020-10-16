Title: This Week in Rust 361
Number: 361
Date: 2020-10-21
Category: This Week in Rust

Hello and welcome to another issue of *This Week in Rust*!
[Rust](http://rust-lang.org) is a systems language pursuing the trifecta: safety, concurrency, and speed.
This is a weekly summary of its progress and community.
Want something mentioned? Tweet us at [@ThisWeekInRust](https://twitter.com/ThisWeekInRust) or [send us a pull request](https://github.com/emberian/this-week-in-rust).
Want to get involved? [We love contributions](https://github.com/rust-lang/rust/blob/master/CONTRIBUTING.md).

*This Week in Rust* is openly developed [on GitHub](https://github.com/emberian/this-week-in-rust).
If you find any errors in this week's issue, [please submit a PR](https://github.com/emberian/this-week-in-rust/pulls).

# Updates from Rust Community

### Official

### Newsletters

### Tooling

### Observations/Thoughts

### Learn Simple Rust

### Learn More Rust

### Project Updates
* [Version 0.2 of async-hsm](https://crates.io/crates/async-hsm)

### Miscellaneous

# Call for Blog Posts

The Rust Core Team wants input from the community!
If you haven't already, [read the official blog](https://blog.rust-lang.org/2020/09/03/Planning-2021-Roadmap.html) and submit a blog post - it will show up here!
Here are the wonderful submissions since the call for blog posts:

# Crate of the Week

This week's crate is [paste](https://crates.io/crates/paste), a macro to concatenate identifiers (which would otherwise be nightly only).

Thanks to [mark-i-m](https://users.rust-lang.org/t/crate-of-the-week/2704/825) for the suggestion!

[Submit your suggestions and votes for next week][submit_crate]!

[submit_crate]: https://users.rust-lang.org/t/crate-of-the-week/2704

# Call for Participation

Always wanted to contribute to open-source projects but didn't know where to start?
Every week we highlight some tasks from the Rust community for you to pick and get started!

Some of these tasks may also have mentors available, visit the task page for more information.

If you are a Rust project owner and are looking for contributors, please submit tasks [here][guidelines].

[guidelines]: https://users.rust-lang.org/t/twir-call-for-participation/4821

# Updates from Rust Core

409 pull requests were [merged in the last week][merged]

[merged]: https://github.com/search?q=is%3Apr+org%3Arust-lang+is%3Amerged+merged%3A2020-10-05..2020-10-12

* [resolve: improve "try using the enum's variant"](https://github.com/rust-lang/rust/pull/77341)
* [Fix `LitKind`'s byte buffer to use refcounted slice](https://github.com/rust-lang/rust/pull/77560)
* [Replace `(Body, DefId)` with `Body` where possible](https://github.com/rust-lang/rust/pull/77552)
* [perf: `UninhabitedEnumBranching` avoid n²](https://github.com/rust-lang/rust/pull/77597)
* [Fix span for unicode escape suggestion](https://github.com/rust-lang/rust/pull/77587)
* [Implement `advance_by`, `advance_back_by` for `iter::Chain`](https://github.com/rust-lang/rust/pull/77594)
* [Add `PartialEq` impls for `Vec` ↔ `slice`](https://github.com/rust-lang/rust/pull/74194)
* [stdsimd: Use xor to implement `Neg::neg` for floats](https://github.com/rust-lang/stdsimd/pull/31)

## Rust Compiler Performance Triage

* [2020-10-13](https://github.com/rust-lang/rustc-perf/blob/master/triage/2020-10-13.md):
0 Regressions, 3 Improvements, 3 Mixed

Overall, fairly busy week, but without major regressions that need to be addressed.

See the [full report](https://github.com/rust-lang/rustc-perf/blob/master/triage/2020-10-13.md) for more.

## Approved RFCs

Changes to Rust follow the Rust [RFC (request for comments) process](https://github.com/rust-lang/rfcs#rust-rfcs). These
are the RFCs that were approved for implementation this week:

*No RFCs were approved this week.*

## Final Comment Period

Every week [the team](https://www.rust-lang.org/team.html) announces the
'final comment period' for RFCs and key PRs which are reaching a
decision. Express your opinions now.

### [RFCs](https://github.com/rust-lang/rfcs/labels/final-comment-period)
* [RFC: Promote aarch64-unknown-linux-gnu to a Tier-1 Rust target](https://github.com/rust-lang/rfcs/pull/2959)
* [Access to traits' associated functions and constants from trait objects](https://github.com/rust-lang/rfcs/pull/2886)

### [Tracking Issues & PRs](https://github.com/rust-lang/rust/labels/final-comment-period)

* [disposition: merge] [stabilize union with 'ManuallyDrop' fields and 'impl Drop for Union'](https://github.com/rust-lang/rust/pull/77547)
* [disposition: merge] [stop promoting union field accesses in 'const'](https://github.com/rust-lang/rust/pull/77526)
* [disposition: merge] [passes: `check_attr` on more targets](https://github.com/rust-lang/rust/pull/77015)
* [disposition: merge] [resolve: Do not put nonexistent crate `meta` into prelude](https://github.com/rust-lang/rust/pull/75802)
* [disposition: postpone][Tracking issue for experiments around coercions, generics, and Copy type ergonomics](https://github.com/rust-lang/rust/issues/44619)

## New RFCs


# Upcoming Events

### Online
* [Octover 15. Berlin, DE - Rust Hack and Learn - Berline.rs](https://www.meetup.com/opentechschool-berlin/events/txcprrybcnbtb/)
* [October 20. Denver, CO, US - Rust Denver - Data Science with Rust](https://www.meetup.com/Rust-Boulder-Denver/events/272996842/)
* [October 21. New York, NY, US - A Journey into the Nucleus at Dropbox with Parker Timmerman - Rust NYC](https://www.meetup.com/Rust-NYC/events/273887563)
* [October 21. Vancover, BC, CA - Rust Study/Hack/Hang-out night - Vancouver Rust](https://www.meetup.com/Vancouver-Rust/events/cxrtxrybcnbcc/)
* [October 22. Edinburgh, UK - Fluence: interface-types for server-side WebAssembly modules - Rust Edinburgh](https://www.meetup.com/rust-edi/events/273685985)
* [October 27. Dallas, TX, US - Last Tuesday - Dallas Rust](https://www.meetup.com/Dallas-Rust/events/jqxqwrybcnbkc/)

If you are running a Rust event please add it to the [calendar] to get
it mentioned here. Please remember to add a link to the event too.
Email the [Rust Community Team][community] for access.

[calendar]: https://www.google.com/calendar/embed?src=apd9vmbc22egenmtu5l6c5jbfc%40group.calendar.google.com
[community]: mailto:community-team@rust-lang.org

# Rust Jobs

*Tweet us at [@ThisWeekInRust](https://twitter.com/ThisWeekInRust) to get your job offers listed here!*

# Quote of the Week

> Just because Rust allows you to write super cool non-allocating zero-copy algorithms safely, doesn’t mean every algorithm you write should be super cool, zero-copy and non-allocating.

- [trentj on rust-users](https://users.rust-lang.org/t/feeling-rust-is-so-difficult/29962/15)

Thanks to [Nixon Enraght-Moony](https://users.rust-lang.org/t/twir-quote-of-the-week/328/948) for the suggestion!

[Please submit quotes and vote for next week!](https://users.rust-lang.org/t/twir-quote-of-the-week/328)

*This Week in Rust is edited by: [nellshamrell](https://github.com/nellshamrell), [llogiq](https://github.com/llogiq), and [cdmistman](https://github.com/cdmistman).*

<small>[Discuss on r/rust](https://www.reddit.com/r/rust/comments/iu3ge0/this_week_in_rust_356/)</small>
