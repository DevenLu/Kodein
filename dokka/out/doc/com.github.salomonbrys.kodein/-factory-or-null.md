[com.github.salomonbrys.kodein](index.md) / [FactoryOrNull](.)

# FactoryOrNull

`fun <A, T : Any> `[`LazyKodeinAwareBase`](-lazy-kodein-aware-base/index.md)`.FactoryOrNull(argType: `[`TypeToken`](-type-token/index.md)`<A>, type: `[`TypeToken`](-type-token/index.md)`<T>, tag: Any? = null): Lazy<(A) -> T>`

Gets a lazy factory for the given type, tag and argument type, or null if none is found.

A &amp; T generics will be kept.

### Parameters

`A` - The type of argument the factory held by this property takes.

`T` - The type of object to retrieve with the factory held by this property.

`tag` - The bound tag, if any.

### Exceptions

`Kodein.DependencyLoopException` - When calling the factory, if the value construction triggered a dependency loop.

**Receiver**
Either a [LazyKodein](-lazy-kodein/index.md) instance or a [LazyKodeinAware](-lazy-kodein-aware.md) class.

**Return**
A lazy property that yields a factory of `T`, or null if no factory was found.

