Title: This Week in Rust 370
Number: 370
Date: 2020-12-23
Category: This Week in Rust

Hello and welcome to another issue of *This Week in Rust*!
[Rust](http://rust-lang.org) is a systems language pursuing the trifecta: safety, concurrency, and speed.
This is a weekly summary of its progress and community.
Want something mentioned? Tweet us at [@ThisWeekInRust](https://twitter.com/ThisWeekInRust) or [send us a pull request](https://github.com/rust-lang/this-week-in-rust).
Want to get involved? [We love contributions](https://github.com/rust-lang/rust/blob/master/CONTRIBUTING.md).

*This Week in Rust* is openly developed [on GitHub](https://github.com/rust-lang/this-week-in-rust).
If you find any errors in this week's issue, [please submit a PR](https://github.com/rust-lang/this-week-in-rust/pulls).

# Updates from Rust Community

No official blog posts or newsletters this week.

### Project/Tooling Updates
* [Rust Analyzer Changelog #56](https://rust-analyzer.github.io/thisweek/2020/12/21/changelog-56.html)
* [Knurling-rs Changelog #11](https://ferrous-systems.com/blog/knurling-changelog-11/)
* [Bevy 0.4](https://bevyengine.org/news/bevy-0-4/)
* [Announcing Tokio 1.0](https://tokio.rs/blog/2020-12-tokio-1-0)
* [hyper 0.14](https://seanmonstar.com/post/638320652536922112/hyper-v014)
* [RustFFT 5.0.0.experimental-1: Now faster than FFTW!](https://users.rust-lang.org/t/rustfft-5-0-0-experimental-1-now-faster-than-fftw/53049)
* [Allsorts Font Shaping Engine Year in Review](https://yeslogic.com/blog/allsorts-rust-font-shaping-engine-2020-review/)

### Observations/Thoughts
* [Looking back on 2020](http://smallcultfollowing.com/babysteps/blog/2020/12/18/looking-back-on-2020/)
* [I rewrote a Clojure tool in Rust](https://timofreiberg.github.io/clojure-vs-rust/)
* [🦀 Rust Reviewed: Is the hype justified? 🦀](https://dev.to/somedood/rust-reviewed-is-the-hype-justified-1pa1)
* [Three things I wish I'd known learning Rust](https://www.darkcoding.net/software/three-things-i-wish-id-known-learning-rust/)
* [Rust in a KDE Project](https://jbbgameich.github.io/misc/2020/12/21/rust-in-a-kde-project.html)
* [First 3 Months of Rust](https://www.reddit.com/r/rust/comments/khrt69/first_3_months_of_rust/)
* [How rust changed and saved my life](https://www.reddit.com/r/rust/comments/khlln4/how_rust_changed_and_saved_my_life/)
* [Problems with building backend app in Rust in 2020](https://blog.0xfa.be/building-a-backend-app-in-rust/)
* [Reaching the (current) limits of Rust's type system with asynchronous programming](https://gendignoux.com/blog/2020/12/17/rust-async-type-system-limits.html)
* [audio] [Rust GameDev Podcast - Interview with Fedor Logachev](https://rustgamedev.com/episodes/interview-with-fedor-logachev)

### Rust Walkthroughs
* [Build your own async primitive](https://tweedegolf.nl/blog/50/build-your-own-async-primitive)
* [Make A Language - Part Sixteen: Refactoring](https://arzg.github.io/lang/16/)
* [Make A Language - Part Seventeen: Crates](https://arzg.github.io/lang/17/)
* [Make A Language - Part Eighteen: Errors](https://arzg.github.io/lang/18/)
* [A Simple Neural Network (<200LoC, Rust)](https://explog.in/notes/funnn.html)
* [Rocket Tutorial 05: Enforcing uniqueness of emails](https://dev.to/davidedelpapa/rocket-tutorial-05-enforcing-uniqueness-of-emails-136j)
* [How to write a Terminal Multiplexer with Rust, Async, and Actors - Part 2](https://implaustin.hashnode.dev/how-to-write-a-terminal-multiplexer-with-rust-async-and-actors-part-2)
* [Learning Rust: static trait bounds](https://codeandbitters.com/static-trait-bound/)
* [Async: What is blocking?](https://ryhl.io/blog/async-what-is-blocking/)
* [Schedule the program in Rust](https://blog.knoldus.com/schedule-the-program-in-rust/)
* [video] [Generic Associated Types - Learn Rust](https://www.youtube.com/watch?v=JwG-Wa7dOBU&feature=youtu.be)
* [video] [series] [Rust Tutorial](https://youtube.com/playlist?list=PLLqEtX6ql2EyPAZ1M2_C0GgVd4A-_L4_5)

### Miscellaneous
* [A Potential Rust Learning Project Group](https://internals.rust-lang.org/t/a-potential-rust-learning-project-group/13620)
* [Watch all of RustFest Global](https://blog.rustfest.eu/watch-all-of-rustfest)
* [When to use Rust?](https://www.reddit.com/r/rust/comments/kgw8bz/when_to_use_rust/)
* [Hyper support is merged to curl master](https://www.reddit.com/r/rust/comments/kgcye2/hyper_support_is_merged_to_curl_master/)
* [Just wanted to say thanks to the Rust community!](https://www.reddit.com/r/rust/comments/kfiaqn/just_wanted_to_say_thanks_to_the_rust_community/)

# Crate of the Week

This week's crate is [RustFFT](https://github.com/ejmahler/RustFFT), a *Fast* Fourier transformation library that lives up to the name.

Thanks to [Willi Kappler](https://users.rust-lang.org/t/crate-of-the-week/2704/863) for the suggestion!

[Submit your suggestions and votes for next week][submit_crate]!

[submit_crate]: https://users.rust-lang.org/t/crate-of-the-week/2704

# Call for Participation

Always wanted to contribute to open-source projects but didn't know where to start?
Every week we highlight some tasks from the Rust community for you to pick and get started!

Some of these tasks may also have mentors available, visit the task page for more information.

* [The CCC Rustaceans are looking for artwork for badges](https://users.rust-lang.org/t/rc3-assembly-ccc-congress/50283/3)

If you are a Rust project owner and are looking for contributors, please submit tasks [here][guidelines].

[guidelines]: https://users.rust-lang.org/t/twir-call-for-participation/4821

# Updates from Rust Core

292 pull requests were [merged in the last week][merged]

[merged]: https://github.com/search?q=is%3Apr+org%3Arust-lang+is%3Amerged+merged%3A2020-12-14..2020-12-21

* [skip `dsymutil` by default for compiler bootstrap](https://github.com/rust-lang/rust/pull/80213)
* [implement if-let match guards](https://github.com/rust-lang/rust/pull/79051)
* [or\_patterns: implement `:pat` edition-specific behavior](https://github.com/rust-lang/rust/pull/80100)
* [improve and fix diagnostics of exhaustiveness checking](https://github.com/rust-lang/rust/pull/80104)
* [gracefully handle mistyping `->` as `=>` in function return type](https://github.com/rust-lang/rust/pull/77035)
* [handle desugaring in impl trait bound suggestion](https://github.com/rust-lang/rust/pull/80211)
* [enhance error message when misspelled label to value in break expression](https://github.com/rust-lang/rust/pull/80023)
* [always run intrinsics lowering pass](https://github.com/rust-lang/rust/pull/80040)
* [mir-opt: allow debuginfo to be generated for a constant or a Place](https://github.com/rust-lang/rust/pull/73210)
* [turn quadratic time on number of impl blocks into linear time](https://github.com/rust-lang/rust/pull/78317)
* [`MaybeUninit::copy`/`clone_from_slice`](https://github.com/rust-lang/rust/pull/79607)
* [stabilize `unsafe_cell_get_mut`](https://github.com/rust-lang/rust/pull/79485)
* [move {`f32`, `f64`}`::clamp` to `core`](https://github.com/rust-lang/rust/pull/79473)
* [stabilize all stable methods of `Ipv4Addr`, `Ipv6Addr` and `IpAddr` as const](https://github.com/rust-lang/rust/pull/79342)
* [stabilize `or_insert_with_key`](https://github.com/rust-lang/rust/pull/78083)
* [add fast futex-based thread parker for Windows](https://github.com/rust-lang/rust/pull/77618)
* [optimization for `bool`'s `PartialOrd` impl](https://github.com/rust-lang/rust/pull/80035)
* [fix overflow when converting ZST `Vec` to `VecDeque`](https://github.com/rust-lang/rust/pull/80003)
* [use pointer type in `AtomicPtr::swap` implementation](https://github.com/rust-lang/rust/pull/80236)
* [stdarch: move code out of constify macros](https://github.com/rust-lang/stdarch/pull/973)
* [stabilize cargo's new feature resolver](https://github.com/rust-lang/rfcs/pull/2957)

## Rust Compiler Performance Triage

* [2020-12-15](https://github.com/rust-lang/rustc-perf/blob/master/triage/2020-12-15.md):
6 Regressions, 1 Improvements, 2 Mixed

This week was fairly quite with lots of small regressions. Most of the regressions were either for fixes to changes that yielded large performance wins in previous weeks or small performance losses where there is already a plan for how to gain those losses back.

Triage done by @rylev.

See the [full report](https://github.com/rust-lang/rustc-perf/blob/master/triage/2020-12-15.md) for more.

## Approved RFCs

Changes to Rust follow the Rust [RFC (request for comments) process](https://github.com/rust-lang/rfcs#rust-rfcs). These
are the RFCs that were approved for implementation this week:

* [Stabilize Cargo's new feature resolver](https://github.com/rust-lang/rfcs/pull/2957)

## Final Comment Period

Every week [the team](https://www.rust-lang.org/team.html) announces the
'final comment period' for RFCs and key PRs which are reaching a
decision. Express your opinions now.

### [RFCs](https://github.com/rust-lang/rfcs/labels/final-comment-period)

* [disposition: merge] [Infallible promotion](https://github.com/rust-lang/rfcs/pull/3027)
* [disposition: postpone] [Opt-in Stable Trait VTables](https://github.com/rust-lang/rfcs/pull/2955)
* [disposition: merge] [RFC: Serve crates-io registry over HTTP as static files](https://github.com/rust-lang/rfcs/pull/2789)

### [Tracking Issues & PRs](https://github.com/rust-lang/rust/labels/final-comment-period)

* [disposition:merge] [Stabilize Arc::{increment,decrement}_strong_count](https://github.com/rust-lang/rust/pull/79285)
* [disposition:merge] [stabilize `#![feature(min_const_generics)]`](https://github.com/rust-lang/rust/pull/79135)
* [disposition:merge] [Add `impl Div<NonZeroU{0}> for u{0}` which cannot panic](https://github.com/rust-lang/rust/pull/79134)

## New RFCs

* [Primitive enum conversion reform](https://github.com/rust-lang/rfcs/pull/3040)
* [Rust 2021 Roadmap](https://github.com/rust-lang/rfcs/pull/3037)

# Upcoming Events

### Online
* [December 29, Dallas, TX, US - Last Tuesday - Dallas Rust](https://www.meetup.com/Dallas-Rust/events/jqxqwrybcqbmc/)
* [January 5, Buffalo, NY, US - Buffalo Rust User Group](https://www.meetup.com/Buffalo-Rust-Meetup/events/274936687/)

If you are running a Rust event please add it to the [calendar] to get
it mentioned here. Please remember to add a link to the event too.
Email the [Rust Community Team][community] for access.

[calendar]: https://www.google.com/calendar/embed?src=apd9vmbc22egenmtu5l6c5jbfc%40group.calendar.google.com
[community]: mailto:community-team@rust-lang.org

# Rust Jobs

*Tweet us at [@ThisWeekInRust](https://twitter.com/ThisWeekInRust) to get your job offers listed here!*

* [Distributed Systems (Rust) Developer at Signal (Remote)](https://jobs.lever.co/signal/7aa1ff1f-bd43-4359-82c7-8703d8b842d9)
* [Architect - Rust Library Design at Ockam (Remote)](https://www.ockam.io/team/Architect-Rust-Library-Design/53838c2d-1e48-5cec-8bb4-8fa8420e6171)
* [Senior Software Engineer (Rust & C++) at NZXT (Remote)](https://nzxt.bamboohr.com/jobs/view.php?id=259)
* [Lead Backend Engineer - Rust or C/C++ at Signavio (Berlin, DE)](https://boards.greenhouse.io/signavio/jobs/4167572003?gh_src=e31399983us)

# Quote of the Week

> It took me sometime to let go and embrace getting things working before optimizing. It was a major breakthrough on that journey when I realized that ALL my python variables are `Rc<RefCell<_>>` , so any chance I had to make a variable that was less complicated than that was already a big optimization. If 1/10 Rust variables had to be that complicated it would not feel good, but it would already be 90% better. So if 1/50 make the code ezere to read and maintain then do it!

– [Eh2406 on /r/rust](https://www.reddit.com/r/rust/comments/kdayix/i_need_some_advice_about_heap_usage_with_rust/gfvtcwx)

Thanks to [Stephan Sokolow](https://users.rust-lang.org/t/twir-quote-of-the-week/328/977) for the suggestion.

[Please submit quotes and vote for next week!](https://users.rust-lang.org/t/twir-quote-of-the-week/328)

*This Week in Rust is edited by: [nellshamrell](https://github.com/nellshamrell), [llogiq](https://github.com/llogiq), and [cdmistman](https://github.com/cdmistman).*

<small>[Discuss on r/rust](https://www.reddit.com/r/rust/comments/kj9mcb/this_week_in_rust_370/)</small>
