**STRUCT**

# `Version`

**Contents**

- [Properties](#properties)
  - `major`
  - `minor`
  - `patch`
  - `prereleaseIdentifiers`
  - `buildMetadataIdentifiers`
- [Methods](#methods)
  - `init(_:_:_:prereleaseIdentifiers:buildMetadataIdentifiers:)`

```swift
public struct Version
```

> A struct representing a semver version.

## Properties
<details><summary markdown="span"><code>major</code></summary>

```swift
public let major: Int
```

> The major version.

</details>

<details><summary markdown="span"><code>minor</code></summary>

```swift
public let minor: Int
```

> The minor version.

</details>

<details><summary markdown="span"><code>patch</code></summary>

```swift
public let patch: Int
```

> The patch version.

</details>

<details><summary markdown="span"><code>prereleaseIdentifiers</code></summary>

```swift
public let prereleaseIdentifiers: [String]
```

> The pre-release identifier.

</details>

<details><summary markdown="span"><code>buildMetadataIdentifiers</code></summary>

```swift
public let buildMetadataIdentifiers: [String]
```

> The build metadata.

</details>

## Methods
<details><summary markdown="span"><code>init(_:_:_:prereleaseIdentifiers:buildMetadataIdentifiers:)</code></summary>

```swift
public init(
        _ major: Int,
        _ minor: Int,
        _ patch: Int,
        prereleaseIdentifiers: [String] = [],
        buildMetadataIdentifiers: [String] = []
    )
```

> Create a version object.

</details>