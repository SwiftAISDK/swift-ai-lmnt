<!-- Generated distribution; edit the canonical repository. -->
# swift-ai-lmnt 1.1.0

Independent Swift-native port of Vercel AI SDK. Source and upstream dispositions are in PROVENANCE.json and Porting/.

## Distribution manifest

Add this package to your SwiftPM dependencies:

```swift
.package(url: "https://github.com/SwiftAISDK/swift-ai-lmnt.git", from: "1.1.0")
```

Products: `SwiftAILMNT`.
Contribute and report issues in the canonical SwiftAISDK repository.

## Authored usage guide

# LMNT for Swift

`SwiftAILMNT` adds LMNT to [SwiftAISDK](https://github.com/SwiftAISDK/SwiftAISDK), an independent Swift port of the Vercel AI SDK. It ports `@ai-sdk/lmnt` and supports speech.

Provider guide with models, options, streaming and errors:

- [LMNT](https://swiftaisdk.github.io/SwiftAISDK/providers/lmnt/)

## Usage

Add the `SwiftAI` product from `swift-ai-core` and the `SwiftAILMNT` product from this package to your target, then create the provider:

```swift
import SwiftAI
import SwiftAILMNT

let provider = try AIProviders.lmnt(configuration: LMNTProviderSettings())
```

By default the provider reads `LMNT_API_KEY` from the environment; values set in `LMNTProviderSettings` take precedence.

To use every provider through one dependency, add the complete [SwiftAISDK](https://github.com/SwiftAISDK/SwiftAISDK) package instead; see [Install](https://swiftaisdk.github.io/SwiftAISDK/getting-started/install/).

## Contributing

This package is exported from `Packages/swift-ai-lmnt` in the canonical [SwiftAISDK](https://github.com/SwiftAISDK/SwiftAISDK) repository. Open issues and pull requests there.
