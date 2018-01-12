**EXTENSION**

# `DiagnosticsEngine`

## Methods
<details><summary markdown="span"><code>emit(data:)</code></summary>

```swift
public func emit(data: DiagnosticData)
```

> Emit a diagnostic with an unknown location.

</details>

<details><summary markdown="span"><code>emit(_:location:)</code></summary>

```swift
public func emit(
        _ error: Swift.Error,
        location: DiagnosticLocation = UnknownLocation.location
    )
```

> Emit a Swift error.
>
> Errors will be converted into diagnostic data if possible.
> Otherwise, they will be emitted as AnyDiagnostic.

</details>

<details><summary markdown="span"><code>emit(_:location:)</code></summary>

```swift
public func emit(
        _ convertible: DiagnosticDataConvertible,
        location: DiagnosticLocation = UnknownLocation.location
     )
```

> Emit a diagnostic data convertible instance.

</details>

<details><summary markdown="span"><code>wrap(with:_:)</code></summary>

```swift
public func wrap<T>(
        with constuctLocation: @autoclosure () -> (DiagnosticLocation) = UnknownLocation.location,
        _ closure: () throws -> T
    ) -> T?
```

> Wrap a throwing closure, returning an optional value and
> emitting any thrown errors.
>
> - Parameters:
>     - closure: Closure to wrap.
> - Returns: Returns the return value of the closure wrapped
>   into an optional. If the closure throws, nil is returned.

#### Parameters

| Name | Description |
| ---- | ----------- |
| closure | Closure to wrap. |

</details>

<details><summary markdown="span"><code>wrap(with:_:)</code></summary>

```swift
public func wrap(
        with constuctLocation: @autoclosure () -> (DiagnosticLocation) = UnknownLocation.location,
        _ closure: () throws -> Void
    ) -> Bool
```

> Wrap a throwing closure, returning a success boolean and
> emitting any thrown errors.
>
> - Parameters:
>     - closure: Closure to wrap.
> - Returns: Returns true if the wrapped closure did not throw
>   and false otherwise.

#### Parameters

| Name | Description |
| ---- | ----------- |
| closure | Closure to wrap. |

</details>