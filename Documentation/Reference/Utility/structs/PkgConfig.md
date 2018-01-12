**STRUCT**

# `PkgConfig`

**Contents**

- [Properties](#properties)
  - `name`
  - `pcFile`
  - `cFlags`
  - `libs`
- [Methods](#methods)
  - `init(name:additionalSearchPaths:fileSystem:)`

```swift
public struct PkgConfig
```

> Information on an individual `pkg-config` supported package.

## Properties
<details><summary markdown="span"><code>name</code></summary>

```swift
public let name: String
```

> The name of the package.

</details>

<details><summary markdown="span"><code>pcFile</code></summary>

```swift
public let pcFile: AbsolutePath
```

> The path to the definition file.

</details>

<details><summary markdown="span"><code>cFlags</code></summary>

```swift
public let cFlags: [String]
```

> The list of C compiler flags in the definition.

</details>

<details><summary markdown="span"><code>libs</code></summary>

```swift
public let libs: [String]
```

> The list of libraries to link.

</details>

## Methods
<details><summary markdown="span"><code>init(name:additionalSearchPaths:fileSystem:)</code></summary>

```swift
public init(
        name: String,
        additionalSearchPaths: [AbsolutePath] = [],
        fileSystem: FileSystem = localFileSystem
    ) throws
```

> Load the information for the named package.
>
> It will search `fileSystem` for the pkg config file in the following order:
> * Paths defined in `PKG_CONFIG_PATH` environment variable
> * Paths defined in `additionalSearchPaths` argument
> * Built-in search paths (see `PkgConfig.searchPaths`)
>
> - parameter name: Name of the pkg config file (without file extension).
> - parameter additionalSearchPaths: Additional paths to search for pkg config file.
> - parameter fileSystem: The file system to use, defaults to local file system.
>
> - throws: PkgConfigError

#### Parameters

| Name | Description |
| ---- | ----------- |
| name | Name of the pkg config file (without file extension). |
| additionalSearchPaths | Additional paths to search for pkg config file. |
| fileSystem | The file system to use, defaults to local file system. |

</details>