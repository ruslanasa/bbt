[![Build Status](https://travis-ci.org/DataWraith/bbt.svg?branch=master)](https://travis-ci.org/DataWraith/bbt)

**Status**: In maintenance mode. I will address Issues and Pull requests, but have no plans to add new features.

# BBT

BBT is an implementation of a skill-rating system similar to Elo, Glicko or
TrueSkill. It follows `Algorithm 1` from the paper
[A Bayesian Approximation Method for Online Ranking][ABAMOR].

[ABAMOR]: http://jmlr.csail.mit.edu/papers/volume12/weng11a/weng11a.pdf

## Instructions

Add BBT to your Cargo.toml:

```toml
[dependencies]
bbt = "0.2.0"
```

If you want to serialize Ratings with [Serde](https://serde.rs/), you will need
to add the following to your Cargo.toml instead:

```toml
[dependencies.bbt]
version = "0.2.0"
features = ["serde"]
```

See the [Documentation](https://docs.rs/bbt/) for information on how to use the
crate.

## Contributors

Thank you for your contributions!

* [@rakenodiax](https://github.com/rakenodiax) contributed the optional Serde
  serialization support
