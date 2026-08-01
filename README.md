# moglang/math

Portable numeric constants and helpers for Mog. The canonical import is
`github.com/moglang/math`, and the package supports Mog runtime `^0.1.4`.

```bash
mog add github.com/moglang/math@v0.2.0
```

```mog
const math = @import("github.com/moglang/math")

print(math.PI)
print(math.clampI64(12, 0, 10))
print(math.squareRoot(81.0))
print(math.roundValue(-2.6))
```

The package provides `i64` and `f64` absolute-value, minimum, maximum, and
clamping helpers, plus wrappers for square root, powers, floor, ceiling, and
rounding. Clamping rejects an inverted range. `roundValue` rounds halfway
values away from zero.

The original `VALUE`, `LABEL`, `Add`, `Multiply`, and `Name` exports remain for
source compatibility with the package's initial import-test release. New code
should prefer the descriptive lower-camel-case helpers. The complete public
contract is declared in `package.api.mog`. The package is licensed under MIT;
see `LICENSE`.
