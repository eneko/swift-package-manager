**STRUCT**

# `PathArgument`

**Contents**

- [Properties](#properties)
  - `path`
- [Methods](#methods)
  - `init(argument:)`

```swift
public struct PathArgument: ArgumentKind
```

> An argument representing a path (file / directory).
>
> The path is resolved in the current working directory.

## Properties
<details><summary markdown="span"><code>path</code></summary>

```swift
public let path: AbsolutePath
```

</details>

## Methods
<details><summary markdown="span"><code>init(argument:)</code></summary>

```swift
public init(argument: String) throws
```

</details>