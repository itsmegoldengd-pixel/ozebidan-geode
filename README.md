
# Ozebidan Geode

Ozebidan Geode is a custom Geometry Dash mod loader project.

## Why Ozebidan Geode?

Unlike previous mod loaders, which merely inject the DLLs and let devs handle the rest, Ozebidan Geode aims to be a more comprehensive project that provides all the tools needed for creating mods in one package.

Ozebidan Geode's goal is to solve **mod incompatibility** - to ensure that mods work together without buttons getting misplaced or hooks mysteriously disappearing.

## "Hello World!" Example

Here's a **Hello World** mod in Ozebidan Geode:

```cpp
#include <Geode/Bindings.hpp>
#include <Geode/modify/MenuLayer.hpp>

using namespace geode::prelude;

class $modify(MenuLayer) {
	void onNews(CCObject*) {
		FLAlertLayer::create(
			"Ozebidan Geode",
			"Hello World from my Custom Mod!",
			"OK"
		)->show();
	}
};
```

This code modifies what happens when the "News" button is clicked on the home scene in Geometry Dash, showing a custom popup.

## Documentation

Detailed documentation, tutorials, and installation instructions on using Geode can be found [here](https://docs.geode-sdk.org).

New to modding OGDPS? Ozebidan Geode's documentation also comes with a handy [tutorial book](https://docs.geode-sdk.org/#/handbook/chap0) that explains all the basics of GD modding!

## Questions, help, etc.

If you have any further questions, need help, or just want to share your love for catgirls, be sure to join [our Discord server](https://discord.gg/NdbGEpEQw)!
