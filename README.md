![](raylib_logo.png)

# re-raylib-d [![DUB](https://img.shields.io/dub/v/re-raylib-d?style=for-the-badge)](https://code.dlang.org/packages/re-raylib-d)
(static) D bindings for [raylib](https://www.raylib.com/), a simple and easy-to-use library to learn videogames programming. this is based on a [fork](https://github.com/xdrie/raylib) of raylib, and a fork of the original [raylib-d](https://github.com/onroundit/raylib-d).

# Installation
`dub add re-raylib-d`

## First, get Raylib

these bindings are for this [branch](https://github.com/xdrie/raylib/tree/3.0.0_patch) (`3.0.0_patch`) of raylib.

## In order to link against raylib, add it to your dub.json.
```json
"libs": [ "raylib" ]
```

# Sample
```D
import raylib;

void main()
{
	InitWindow(800, 600, "Hello, World!");
	while (!WindowShouldClose())
	{
		BeginDrawing();
		ClearBackground(Colors.RAYWHITE);
		DrawText("Hello, World!", 400, 300, 28, Colors.BLACK);
		EndDrawing();
	}
	CloseWindow();
}
```

# docs
refer to the official [cheatsheet](https://www.raylib.com/cheatsheet/cheatsheet.html).

# License
re-raylib-d is licensed under an unmodified zlib/libpng license. View [LICENSE](LICENSE).
