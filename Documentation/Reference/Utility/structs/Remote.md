**STRUCT**

# `Remote`

**Contents**

- [Properties](#properties)
  - `url`
  - `reference`
  - `localizedDescription`
- [Methods](#methods)
  - `init(url:reference:)`

```swift
public struct Remote: DiagnosticLocation
```

> Represents location a remote package with no checkout on disk.

## Properties
<details><summary markdown="span"><code>url</code></summary>

```swift
public let url: String
```

> The URL of the package.

</details>

<details><summary markdown="span"><code>reference</code></summary>

```swift
public let reference: String
```

> The source control reference of the package. It could be version, branch, revision etc.

</details>

<details><summary markdown="span"><code>localizedDescription</code></summary>

```swift
public var localizedDescription: String
```

</details>

## Methods
<details><summary markdown="span"><code>init(url:reference:)</code></summary>

```swift
public init(url: String, reference: String)
```

</details>