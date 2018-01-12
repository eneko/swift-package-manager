**ENUM**

# `PkgConfigError`

**Contents**

- [Cases](#cases)
  - `couldNotFindConfigFile`
  - `parsingError`
  - `nonWhitelistedFlags`

```swift
public enum PkgConfigError: Swift.Error
```

## Cases
### `couldNotFindConfigFile`

```swift
case couldNotFindConfigFile
```

### `parsingError`

```swift
case parsingError(String)
```

### `nonWhitelistedFlags`

```swift
case nonWhitelistedFlags(String)
```
