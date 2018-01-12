**CLASS**

# `ArgumentBinder`

**Contents**

- [Methods](#methods)
  - `init()`
  - `bind(option:to:)`
  - `bindArray(option:to:)`
  - `bind(positional:to:)`
  - `bindArray(positional:to:)`
  - `bindPositional(_:_:to:)`
  - `bindPositional(_:_:_:to:)`
  - `bind(_:_:to:)`
  - `bind(_:_:_:to:)`
  - `bindArray(_:_:to:)`
  - `bindArray(_:_:_:to:)`
  - `bind(parser:to:)`
  - `fill(_:into:)`

```swift
public final class ArgumentBinder<Options>
```

> A class to bind ArgumentParser's arguments to an option structure.

## Methods
<details><summary markdown="span"><code>init()</code></summary>

```swift
public init()
```

> Create a binder.

</details>

<details><summary markdown="span"><code>bind(option:to:)</code></summary>

```swift
public func bind<T>(
        option: OptionArgument<T>,
        to body: @escaping (inout Options, T) -> Void
    )
```

> Bind an option argument.

</details>

<details><summary markdown="span"><code>bindArray(option:to:)</code></summary>

```swift
public func bindArray<T>(
        option: OptionArgument<[T]>,
        to body: @escaping (inout Options, [T]) -> Void
    )
```

> Bind an array option argument.

</details>

<details><summary markdown="span"><code>bind(positional:to:)</code></summary>

```swift
public func bind<T>(
        positional: PositionalArgument<T>,
        to body: @escaping (inout Options, T) -> Void
    )
```

> Bind a positional argument.

</details>

<details><summary markdown="span"><code>bindArray(positional:to:)</code></summary>

```swift
public func bindArray<T>(
        positional: PositionalArgument<[T]>,
        to body: @escaping (inout Options, [T]) -> Void
    )
```

> Bind an array positional argument.

</details>

<details><summary markdown="span"><code>bindPositional(_:_:to:)</code></summary>

```swift
public func bindPositional<T, U>(
        _ first: PositionalArgument<T>,
        _ second: PositionalArgument<U>,
        to body: @escaping (inout Options, T, U) -> Void
    )
```

> Bind two positional arguments.

</details>

<details><summary markdown="span"><code>bindPositional(_:_:_:to:)</code></summary>

```swift
public func bindPositional<T, U, V>(
        _ first: PositionalArgument<T>,
        _ second: PositionalArgument<U>,
        _ third: PositionalArgument<V>,
        to body: @escaping (inout Options, T, U, V) -> Void
    )
```

> Bind three positional arguments.

</details>

<details><summary markdown="span"><code>bind(_:_:to:)</code></summary>

```swift
public func bind<T, U>(
        _ first: OptionArgument<T>,
        _ second: OptionArgument<U>,
        to body: @escaping (inout Options, T?, U?) -> Void
    )
```

> Bind two options.

</details>

<details><summary markdown="span"><code>bind(_:_:_:to:)</code></summary>

```swift
public func bind<T, U, V>(
        _ first: OptionArgument<T>,
        _ second: OptionArgument<U>,
        _ third: OptionArgument<V>,
        to body: @escaping (inout Options, T?, U?, V?) -> Void
    )
```

> Bind three options.

</details>

<details><summary markdown="span"><code>bindArray(_:_:to:)</code></summary>

```swift
public func bindArray<T, U>(
        _ first: OptionArgument<[T]>,
        _ second: OptionArgument<[U]>,
        to body: @escaping (inout Options, [T], [U]) -> Void
    )
```

> Bind two array options.

</details>

<details><summary markdown="span"><code>bindArray(_:_:_:to:)</code></summary>

```swift
public func bindArray<T, U, V>(
        _ first: OptionArgument<[T]>,
        _ second: OptionArgument<[U]>,
        _ third: OptionArgument<[V]>,
        to body: @escaping (inout Options, [T], [U], [V]) -> Void
     )
```

> Add three array option and call the final closure with their values.

</details>

<details><summary markdown="span"><code>bind(parser:to:)</code></summary>

```swift
public func bind(
        parser: ArgumentParser,
        to body: @escaping (inout Options, String) -> Void
    )
```

> Bind a subparser.

</details>

<details><summary markdown="span"><code>fill(_:into:)</code></summary>

```swift
public func fill(_ result: ArgumentParser.Result, into options: inout Options)
```

> Fill the result into the options structure.

</details>