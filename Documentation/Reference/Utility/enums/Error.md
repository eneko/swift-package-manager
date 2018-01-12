**ENUM**

# `Error`

**Contents**

- [Cases](#cases)
  - `invalidSchemaVersion`
  - `restoreFailure`

```swift
public enum Error: Swift.Error
```

> Describes a SimplePersistence errors.

## Cases
### `invalidSchemaVersion`

```swift
case invalidSchemaVersion(Int)
```

### `restoreFailure`

```swift
case restoreFailure(stateFile: AbsolutePath, error: Swift.Error)
```
