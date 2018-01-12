**ENUM**

# `ArgumentConversionError`

**Contents**

- [Cases](#cases)
  - `unknown`
  - `typeMismatch`
  - `custom`

```swift
public enum ArgumentConversionError: Swift.Error
```

> Conversion errors that can be returned from `ArgumentKind`'s failable
> initializer.

## Cases
### `unknown`

```swift
case unknown(value: String)
```

> The value is unkown.

### `typeMismatch`

```swift
case typeMismatch(value: String, expectedType: Any.Type)
```

> The value could not be converted to the target type.

### `custom`

```swift
case custom(String)
```

> Custom reason for conversion failure.
