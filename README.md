# kf
Kernel foundation library for Windows.

## Requirements
- Visual Studio 2019 or newer

## Roadmap 
- [ ] Document
- [ ] Add tests
- [ ] Add automated builds
- [ ] Rework `UString`, `USimpleString`, `ASimpleString` in favour of `std::string_view`, `std::wstring_view` as they have no 32k limit
- [ ] Think how to make `GenericTableAvl` safe for concurrent reading (maybe replace it?)
- [ ] Get rid of `FltResourceExclusiveLock`/`FltResourceSharedLock`/`EResourceExclusiveLock`/`EResourceSharedLock` and make `FltResource`/`EResource` lockable with `std::shared_lock`/`std::unique_lock`
