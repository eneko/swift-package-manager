**CLASS**

# `InterruptHandler`

**Contents**

- [Methods](#methods)
  - `init(_:)`

```swift
public final class InterruptHandler
```

> This class can be used by command line tools to install a handler which
> should be called when a interrupt signal is delivered to the process.

## Methods
<details><summary markdown="span"><code>init(_:)</code></summary>

```swift
public init(_ handler: @escaping () -> Void) throws
```

> Start watching for interrupt signal and call the handler whenever the signal is received.

</details>