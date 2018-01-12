**STRUCT**

# `ProcessExecutionError`

**Contents**

- [Properties](#properties)
  - `result`
- [Methods](#methods)
  - `init(_:)`

```swift
public struct ProcessExecutionError: DiagnosticData
```

> Diagnostic for the process execution failure.

## Properties
<details><summary markdown="span"><code>result</code></summary>

```swift
public let result: ProcessResult
```

> The process result.

</details>

## Methods
<details><summary markdown="span"><code>init(_:)</code></summary>

```swift
public init(_ result: ProcessResult)
```

</details>