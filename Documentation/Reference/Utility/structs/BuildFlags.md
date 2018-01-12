**STRUCT**

# `BuildFlags`

**Contents**

- [Properties](#properties)
  - `cCompilerFlags`
  - `cxxCompilerFlags`
  - `linkerFlags`
  - `swiftCompilerFlags`
- [Methods](#methods)
  - `init(xcc:xcxx:xswiftc:xlinker:)`

```swift
public struct BuildFlags
```

> Build-tool independent flags.

## Properties
<details><summary markdown="span"><code>cCompilerFlags</code></summary>

```swift
public var cCompilerFlags: [String]
```

> Flags to pass to the C compiler.

</details>

<details><summary markdown="span"><code>cxxCompilerFlags</code></summary>

```swift
public var cxxCompilerFlags: [String]
```

> Flags to pass to the C++ compiler.

</details>

<details><summary markdown="span"><code>linkerFlags</code></summary>

```swift
public var linkerFlags: [String]
```

> Flags to pass to the linker.

</details>

<details><summary markdown="span"><code>swiftCompilerFlags</code></summary>

```swift
public var swiftCompilerFlags: [String]
```

> Flags to pass to the Swift compiler.

</details>

## Methods
<details><summary markdown="span"><code>init(xcc:xcxx:xswiftc:xlinker:)</code></summary>

```swift
public init(
        xcc: [String]? = nil,
        xcxx: [String]? = nil,
        xswiftc: [String]? = nil,
        xlinker: [String]? = nil
    )
```

</details>