# math

Small Mog source package used to manually test Go-style GitHub module imports.

```mog
const math = @import("github.com/moglang/math")
print(math.Add(math.VALUE, 8))
```

Install from a Mog project:

```bash
../../build/interpreter add github.com/moglang/math@v0.1.0
../../build/interpreter install
../../build/interpreter run app.mog
```
