# Rust

> Cheatsheet for the Rust programming language

- Create a new vector:

`let vec = vec![1,2,3,4,5];`

- Copy a vector:

`let new_vec = vec.to_vec();`

- Implement a trait for any type that implements another trait:

`impl<T: Display> ToString for T { --snip-- }`

- Implement Pair::cmd_display only if type T implements Display and PartialOrd:

`impl<T: Display + PartialOrd> Pair<T> { fn cmp_display(&self) { --snip-- } }`

- You are using a Greek (non-ASCII) character that's identical to the corresponding English letter:

`error[E0658]: non-ascii idents are not fully supported`

- Get the value out of a std::sync::Mutex:

`let protected_var = mutex_var.lock().unwrap();`

- Spawn a new thread - run in a function:

`joinhandles.push(thread::spawn(move || { ... })`

- Show println statements in rust tests:

`cargo test -- --nocapture`
