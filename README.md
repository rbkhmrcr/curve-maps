# curve-maps

A variety of curve maps (hashing to elliptic curves) useful in different
circumstances.

The table below shows the curve maps used in this repo, along with links to
their reference papers, their computational cost, and conditions for their use.

## indifferentiable hashing to elliptic curves

| curve map | cost | conditions for use |
| --------- | ---- | ------------------ |
| Shallue, van der Woestijne [[0]](https://link.springer.com/chapter/10.1007/11792086_36) | sqrt + 2 ( . / q ) | no conditions! |
| Icart + SWU map [[1](https://eprint.iacr.org/2009/340), [2](https://eprint.iacr.org/2009/226)] | sixth root | q = 2 mod 3, ab != 0 |
| Koshelev [[3]](https://eprint.iacr.org/2021/301) | third root | a = 0, sqrt(b) \in Fq |
| Koshelev [[4]](https://eprint.iacr.org/2021/1604) | fourth root | b = 0 |
| SwiftEC [[5]](https://eprint.iacr.org/2022/759) | sqrt + 2 ( . / q ) | lots |

## non-indifferentiable hashing to elliptic curves

| curve map | cost | conditions for use |
| --------- | ---- | ------------------ |
| Icart [[2]](https://eprint.iacr.org/2009/226) | third root | q = 2 mod 3 |
| Brier et al + simplified SWU [[1]](https://eprint.iacr.org/2009/340) | sqrt | ab != 0 |
| Wahby Boneh [[6]](https://eprint.iacr.org/2019/403) | sqrt | ab = 0, E has a vertical Fq isogeny of small degree |
| Koshelev [[7]](https://eprint.iacr.org/2021/1034) | sqrt | ab = 0, trace of E has small divisor |
