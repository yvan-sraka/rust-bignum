Bignums for Rust backed by GMP
------------------------------

I'm hoping this will eventually be a drop-in replacement for the existing BigInt library, but I may change the API a bit in some places that I find awkward.

Currently only BigUint is supported, and all you can do is convert to and from, print, add, subtract, and multiply.

```rust
let x = 42.to_biguint().unwrap();
let two = 2.to_biguint().unwrap();

println!("{}", x + two); //-> 44
println!("{}", x - two); //-> 40
println!("{}", x * two); //-> 84
```

