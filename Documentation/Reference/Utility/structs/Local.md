**STRUCT**

# `Local`

**Contents**

- [Properties](#properties)
  - `name`
  - `packagePath`
  - `localizedDescription`
- [Methods](#methods)
  - `init(name:packagePath:)`

```swift
public struct Local: DiagnosticLocation
```

> Represents location of a locally available package. This could be root
> package, edited dependency or checked out dependency.

## Properties
<details><summary markdown="span"><code>name</code></summary>

```swift
public let name: String?
```

> The name of the package, if known.

</details>

<details><summary markdown="span"><code>packagePath</code></summary>

```swift
public let packagePath: AbsolutePath
```

> The path to the package.

</details>

<details><summary markdown="span"><code>localizedDescription</code></summary>

```swift
public var localizedDescription: String
```

</details>

## Methods
<details><summary markdown="span"><code>init(name:packagePath:)</code></summary>

```swift
public init(name: String? = nil, packagePath: AbsolutePath)
```

</details>