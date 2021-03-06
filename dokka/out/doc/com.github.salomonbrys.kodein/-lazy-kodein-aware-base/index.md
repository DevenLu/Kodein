[com.github.salomonbrys.kodein](../index.md) / [LazyKodeinAwareBase](.)

# LazyKodeinAwareBase

`interface LazyKodeinAwareBase`

Base [LazyKodeinAware](../-lazy-kodein-aware.md) interface.

It is separate from [LazyKodeinAware](../-lazy-kodein-aware.md) because [LazyKodein](../-lazy-kodein/index.md) implements itself LazyKodeinAwareBase but not [LazyKodeinAware](../-lazy-kodein-aware.md).
This is because there are some extension functions to [LazyKodeinAware](../-lazy-kodein-aware.md) that would not make sense applied to the [LazyKodein](../-lazy-kodein/index.md) object.
For example, [LazyKodeinAware.withClass](../with-class.md), if applied to [LazyKodein](../-lazy-kodein/index.md), would create a very un-expected result.

### Properties

| Name | Summary |
|---|---|
| [kodein](kodein.md) | `abstract val kodein: `[`LazyKodein`](../-lazy-kodein/index.md)<br>A Lazy Kodein Aware class must be within reach of a LazyKodein object. |

### Extension Functions

| Name | Summary |
|---|---|
| [Factory](../-factory.md) | `fun <A, T : Any> LazyKodeinAwareBase.Factory(argType: `[`TypeToken`](../-type-token/index.md)`<A>, type: `[`TypeToken`](../-type-token/index.md)`<T>, tag: Any? = null): Lazy<(A) -> T>`<br>Gets a lazy factory for the given type, tag and argument type. |
| [FactoryOrNull](../-factory-or-null.md) | `fun <A, T : Any> LazyKodeinAwareBase.FactoryOrNull(argType: `[`TypeToken`](../-type-token/index.md)`<A>, type: `[`TypeToken`](../-type-token/index.md)`<T>, tag: Any? = null): Lazy<(A) -> T>`<br>Gets a lazy factory for the given type, tag and argument type, or null if none is found. |
| [Instance](../-instance.md) | `fun <T : Any> LazyKodeinAwareBase.Instance(type: `[`TypeToken`](../-type-token/index.md)`<T>, tag: Any? = null): Lazy<T>`<br>Gets a lazy instance for the given type and tag. |
| [InstanceOrNull](../-instance-or-null.md) | `fun <T : Any> LazyKodeinAwareBase.InstanceOrNull(type: `[`TypeToken`](../-type-token/index.md)`<T>, tag: Any? = null): Lazy<T?>`<br>Gets a lazy instance for the given type and tag, or null is none is found. |
| [Provider](../-provider.md) | `fun <T : Any> LazyKodeinAwareBase.Provider(type: `[`TypeToken`](../-type-token/index.md)`<T>, tag: Any? = null): Lazy<() -> T>`<br>Gets a lazy provider for the given type and tag. |
| [ProviderOrNull](../-provider-or-null.md) | `fun <T : Any> LazyKodeinAwareBase.ProviderOrNull(type: `[`TypeToken`](../-type-token/index.md)`<T>, tag: Any? = null): Lazy<() -> T>`<br>Gets a lazy provider for the given type and tag, or null if none is found. |
| [With](../-with.md) | `fun <A> LazyKodeinAwareBase.With(argType: `[`TypeToken`](../-type-token/index.md)`<A>, arg: A): `[`CurriedLazyKodeinFactory`](../-curried-lazy-kodein-factory/index.md)`<A>`<br>Allows to get a lazy provider or instance from a curried factory with an `A` argument. |
| [WithF](../-with-f.md) | `fun <A> LazyKodeinAwareBase.WithF(argType: `[`TypeToken`](../-type-token/index.md)`<A>, arg: () -> A): `[`CurriedLazyKodeinFactory`](../-curried-lazy-kodein-factory/index.md)`<A>`<br>Allows to get a lazy provider or instance from a curried factory with an `A` argument. |
| [factory](../factory.md) | `fun <A, T : Any> LazyKodeinAwareBase.factory(tag: Any? = null): Lazy<(A) -> T>`<br>Gets a lazy factory for the given type, tag and argument type. |
| [factory](../../com.github.salomonbrys.kodein.erased/factory.md) | `fun <A, T : Any> LazyKodeinAwareBase.factory(tag: Any? = null): Lazy<(A) -> T>`<br>Gets a lazy factory for the given type, tag and argument type. |
| [factoryOrNull](../factory-or-null.md) | `fun <A, T : Any> LazyKodeinAwareBase.factoryOrNull(tag: Any? = null): Lazy<(A) -> T>`<br>Gets a lazy factory for the given type, tag and argument type, or null if none is found. |
| [factoryOrNull](../../com.github.salomonbrys.kodein.erased/factory-or-null.md) | `fun <A, T : Any> LazyKodeinAwareBase.factoryOrNull(tag: Any? = null): Lazy<(A) -> T>`<br>Gets a lazy factory for the given type, tag and argument type, or null if none is found. |
| [instance](../instance.md) | `fun <T : Any> LazyKodeinAwareBase.instance(tag: Any? = null): Lazy<T>`<br>Gets a lazy instance for the given type and tag. |
| [instance](../../com.github.salomonbrys.kodein.erased/instance.md) | `fun <T : Any> LazyKodeinAwareBase.instance(tag: Any? = null): Lazy<T>`<br>Gets a lazy instance for the given type and tag. |
| [instanceOrNull](../instance-or-null.md) | `fun <T : Any> LazyKodeinAwareBase.instanceOrNull(tag: Any? = null): Lazy<T?>`<br>Gets a lazy instance for the given type and tag, or null is none is found. |
| [instanceOrNull](../../com.github.salomonbrys.kodein.erased/instance-or-null.md) | `fun <T : Any> LazyKodeinAwareBase.instanceOrNull(tag: Any? = null): Lazy<T?>`<br>Gets a lazy instance for the given type and tag, or null is none is found. |
| [provider](../provider.md) | `fun <T : Any> LazyKodeinAwareBase.provider(tag: Any? = null): Lazy<() -> T>`<br>Gets a lazy provider for the given type and tag. |
| [provider](../../com.github.salomonbrys.kodein.erased/provider.md) | `fun <T : Any> LazyKodeinAwareBase.provider(tag: Any? = null): Lazy<() -> T>`<br>Gets a lazy provider for the given type and tag. |
| [providerOrNull](../provider-or-null.md) | `fun <T : Any> LazyKodeinAwareBase.providerOrNull(tag: Any? = null): Lazy<() -> T>`<br>Gets a lazy provider for the given type and tag, or null if none is found. |
| [providerOrNull](../../com.github.salomonbrys.kodein.erased/provider-or-null.md) | `fun <T : Any> LazyKodeinAwareBase.providerOrNull(tag: Any? = null): Lazy<() -> T>`<br>Gets a lazy provider for the given type and tag, or null if none is found. |
| [with](../with.md) | `fun <A> LazyKodeinAwareBase.with(arg: () -> A): `[`CurriedLazyKodeinFactory`](../-curried-lazy-kodein-factory/index.md)`<A>`<br>`fun <A> LazyKodeinAwareBase.with(arg: A): `[`CurriedLazyKodeinFactory`](../-curried-lazy-kodein-factory/index.md)`<A>`<br>Allows to get a lazy provider or instance from a curried factory with an `A` argument. |
| [with](../../com.github.salomonbrys.kodein.erased/with.md) | `fun <A> LazyKodeinAwareBase.with(arg: () -> A): `[`CurriedLazyKodeinFactory`](../-curried-lazy-kodein-factory/index.md)`<A>`<br>`fun <A> LazyKodeinAwareBase.with(arg: A): `[`CurriedLazyKodeinFactory`](../-curried-lazy-kodein-factory/index.md)`<A>`<br>Allows to get a lazy provider or instance from a curried factory with an `A` argument. |

### Inheritors

| Name | Summary |
|---|---|
| [LazyKodein](../-lazy-kodein/index.md) | `class LazyKodein : Lazy<`[`Kodein`](../-kodein/index.md)`>, LazyKodeinAwareBase`<br>An object that wraps a Kodein `Lazy` object and acts both as a `Lazy` property delegate &amp; a function. |
| [LazyKodeinAware](../-lazy-kodein-aware.md) | `interface LazyKodeinAware : LazyKodeinAwareBase`<br>Any class that extends this interface can use Kodein to "seamlessly" get lazy properties. |
