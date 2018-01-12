**CLASS**

# `Git`

**Contents**

- [Methods](#methods)
  - `convertTagsToVersionMap(_:)`
  - `checkRefFormat(ref:)`

```swift
public class Git
```

## Methods
<details><summary markdown="span"><code>convertTagsToVersionMap(_:)</code></summary>

```swift
public static func convertTagsToVersionMap(_ tags: [String]) -> [Version: String]
```

> Compute the version -> tag mapping from a list of input `tags`.

</details>

<details><summary markdown="span"><code>checkRefFormat(ref:)</code></summary>

```swift
public static func checkRefFormat(ref: String) -> Bool
```

> Returns true if the git reference name is well formed.

</details>