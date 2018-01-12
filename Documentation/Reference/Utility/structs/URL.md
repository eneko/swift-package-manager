**STRUCT**

# `URL`

**Contents**

- [Methods](#methods)
  - `scheme(_:)`

```swift
public struct URL
```

## Methods
<details><summary markdown="span"><code>scheme(_:)</code></summary>

```swift
public static func scheme(_ url: String) -> String?
```

> Parses the URL type of a git repository
> e.g. https://github.com/apple/swift returns "https"
> e.g. git@github.com:apple/swift returns "git"
>
> This is *not* a generic URI scheme parser!

</details>