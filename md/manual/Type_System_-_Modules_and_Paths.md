The distinction of a module and its containing type of the same name is blurry by design. In fact, addressing `haxe.ds.StringMap<Int>` can be considered shorthand for `haxe.ds.StringMap.StringMap<Int>`. The latter version consists of four parts:



1. the package `haxe.ds`
2. the module name `StringMap`
3. the type name `StringMap`
4. the type parameter `Int`


If the module and type name are equal, the duplicate can be removed, leading to the `haxe.ds.StringMap<Int>` short version. However, knowing about the extended version helps with understanding how [manual/Module_Sub-Types] are addressed.

Paths can be shortened further by using an [manual/Import], which typically allows omitting the package part of a path. This may lead to usage of unqualified identifiers, for which understanding the [manual/Resolution_Order] is required.