**STRUCT**

# `SwiftVersion`

**Contents**

- [Properties](#properties)
  - `version`
  - `isDevelopment`
  - `buildIdentifier`
  - `major`
  - `minor`
  - `patch`
  - `displayString`
  - `completeDisplayString`
  - `versionSpecificKeys`

```swift
public struct SwiftVersion
```

> A Swift version number.
>
> Note that these are *NOT* semantically versioned numbers.

## Properties
<details><summary markdown="span"><code>version</code></summary>

```swift
public var version: (major: Int, minor: Int, patch: Int)
```

> The version number.

</details>

<details><summary markdown="span"><code>isDevelopment</code></summary>

```swift
public var isDevelopment: Bool
```

> Whether or not this is a development version.

</details>

<details><summary markdown="span"><code>buildIdentifier</code></summary>

```swift
public var buildIdentifier: String?
```

> Build information, as an unstructured string.

</details>

<details><summary markdown="span"><code>major</code></summary>

```swift
public var major: Int
```

> The major component of the version number.

</details>

<details><summary markdown="span"><code>minor</code></summary>

```swift
public var minor: Int
```

> The minor component of the version number.

</details>

<details><summary markdown="span"><code>patch</code></summary>

```swift
public var patch: Int
```

> The patch component of the version number.

</details>

<details><summary markdown="span"><code>displayString</code></summary>

```swift
public var displayString: String
```

> The version as a readable string.

</details>

<details><summary markdown="span"><code>completeDisplayString</code></summary>

```swift
public var completeDisplayString: String
```

> The complete product version display string (including the name).

</details>

<details><summary markdown="span"><code>versionSpecificKeys</code></summary>

```swift
public var versionSpecificKeys: [String]
```

> The list of version specific identifiers to search when attempting to
> load version specific package or version information, in order of
> preference.

</details>
