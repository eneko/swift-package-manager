**ENUM**

# `Platform`

**Contents**

- [Cases](#cases)
  - `darwin`
  - `linux`
- [Methods](#methods)
  - `darwinCacheDirectories()`

```swift
public enum Platform
```

## Cases
### `darwin`

```swift
case darwin
```

### `linux`

```swift
case linux(LinuxFlavor)
```

## Methods
<details><summary markdown="span"><code>darwinCacheDirectories()</code></summary>

```swift
public static func darwinCacheDirectories() -> [AbsolutePath]
```

> Returns the cache directories used in Darwin.

</details>