# Compiler Discussion

- Favorite part of compiler
  - Lower optimization (stuff done by LLM)
- Polonius
  - https://rust-lang.github.io/polonius/current_status.html
  - Too slow to put in rust compiler
  - Instead of lifetime be length of reference, the origin of some piece of data
  - If you drop a reference and then recreate to the same data, that works under Polonius but not current
  - Now based on non-lexical lifetimes
  - Question - about under the hood details, but no one in room knew details (location sensitive type checking?)
  - 2018/2019 core book had some details and some blog posts
  - Effectively required rewriting the entire borrow checker, so they are doing some bits piece by piece
-
