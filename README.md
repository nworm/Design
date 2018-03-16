# NWorm

NWorm stands for .Net Wasm Object Relational Mapping.

All credits to @praeclarum for the name.

The idea / thought is to provide a light weight ORM tool (or if it makes sense an EF adapter) to bridge localstorage or any other database that might can be connected through the WASM host.

A WASM host might be a Xamarin.Forms WebView that loads the Wasm site and allows the more permanent access to a Sqlite storage.

Also if working Ooui.Wasm Xamarin.Forms, you should be able to switch to Xamarin.Forms for Desktop / Mobile in a seemless way using the same ORM. 

## Join if you want.. 

This is just getting started, it might be just a simple tool, it might not endup anywhere or it might be just an inspirational discussion.
Send me a message in gitter @juanfranblanco.

## Local Storage access

This can be a low level interop bridge, accessing directly the localstorage or through an existing javascript library like https://github.com/knadh/localStorageDB.

In either scenario in Blazor you will to register each method of the Api. A simple port of the library above could be benefitial as it will avoid the coupling of the library.

## Other Non browser Host access
Here the processing will be done by the host, so here NWorm can provide the abstract layer for Wasm, Javascript bridge and generic backend to access ie Sqlite.

