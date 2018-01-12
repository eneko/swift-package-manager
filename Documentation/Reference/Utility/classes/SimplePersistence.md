**CLASS**

# `SimplePersistence`

**Contents**

- [Methods](#methods)
  - `init(fileSystem:schemaVersion:supportedSchemaVersions:statePath:prettyPrint:)`
  - `restoreState(_:)`
  - `saveState(_:)`

```swift
public final class SimplePersistence
```

> A simple persistence helper.
>
> This class can be used to save and restore state of objects in simple JSON
> format. Note: This class is not thread safe.

## Methods
<details><summary markdown="span"><code>init(fileSystem:schemaVersion:supportedSchemaVersions:statePath:prettyPrint:)</code></summary>

```swift
public init(
        fileSystem: FileSystem,
        schemaVersion: Int,
        supportedSchemaVersions: Set<Int> = [],
        statePath: AbsolutePath,
        prettyPrint: Bool = false
    )
```

</details>

<details><summary markdown="span"><code>restoreState(_:)</code></summary>

```swift
public func restoreState(_ object: SimplePersistanceProtocol) throws -> Bool
```

</details>

<details><summary markdown="span"><code>saveState(_:)</code></summary>

```swift
public func saveState(_ object: SimplePersistanceProtocol) throws
```

</details>