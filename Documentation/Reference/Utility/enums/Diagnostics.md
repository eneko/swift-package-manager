**ENUM**

# `Diagnostics`

**Contents**

- [Cases](#cases)
  - `fatalError`

```swift
public enum Diagnostics: Swift.Error
```

> An Swift error enum that can be used as a stub to early exit from a method.
>
> It is not expected for this enum to contain any payload or information about the
> error. The actual errors and warnings are supposed to be added using the Diagnostics
> engine.

## Cases
### `fatalError`

```swift
case fatalError
```
