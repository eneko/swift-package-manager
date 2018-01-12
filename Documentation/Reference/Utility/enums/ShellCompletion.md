**ENUM**

# `ShellCompletion`

**Contents**

- [Cases](#cases)
  - `none`
  - `unspecified`
  - `filename`
  - `function`
  - `values`

```swift
public enum ShellCompletion
```

> Various shell completions modes supplied by ArgumentKind.
>
> - none:        Offers no completions at all; e.g. for string identifier
> - unspecified: No specific completions, will offer tool's completions
> - filename:    Offers filename completions
> - function:    Custom function for generating completions. Must be
>                provided in the script's scope.
> - values:      Offers completions from predefined list. A description
>                can be provided which is shown in some shells, like zsh.

## Cases
### `none`

```swift
case none
```

### `unspecified`

```swift
case unspecified
```

### `filename`

```swift
case filename
```

### `function`

```swift
case function(String)
```

### `values`

```swift
case values([(value: String, description: String)])
```
