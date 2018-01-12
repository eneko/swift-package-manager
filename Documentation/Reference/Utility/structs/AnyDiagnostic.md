**STRUCT**

# `AnyDiagnostic`

**Contents**

- [Properties](#properties)
  - `anyError`
- [Methods](#methods)
  - `init(_:)`

```swift
public struct AnyDiagnostic: DiagnosticData
```

> DiagnosticData wrapper for Swift errors.

## Properties
<details><summary markdown="span"><code>anyError</code></summary>

```swift
public let anyError: Swift.Error
```

</details>

## Methods
<details><summary markdown="span"><code>init(_:)</code></summary>

```swift
public init(_ error: Swift.Error)
```

</details>