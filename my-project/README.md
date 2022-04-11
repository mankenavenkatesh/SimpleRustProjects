Learn how Rust Module system works

Rust contains packages which contains crates which contains modules

## Steps to create package
Create a package my-project
`cargo my-project`

This creates a package which contains a `src` folder and `Cargo.toml` file.

The Cargo.toml file contains the package information. You can create crates under this package by adding it to `Cargo.toml` file.

Default crates
- If there is main.rs is defined in src directory, then a binary crate with same name as package is automatically added with main.rs as the crate root.

- If there is lib.rs is defined in src directory, then a library crate with same name as package is automatically added with lib.rs as the crate root.


Module tree always starts from the root of the crate. Modules can be accessed using 
- Absolute path - From the create root
- Relative path - From the current path


Run this command to generate module tree (https://rustrepo.com/repo/regexident-cargo-modules)
- `cargo modules generate tree` 


## References
 - https://www.youtube.com/watch?v=5RPXgDQrjio
 - https://www.sheshbabu.com/posts/rust-module-system/
 
