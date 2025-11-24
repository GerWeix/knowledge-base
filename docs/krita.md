# Krita

## Shortcuts

|     |     |
| --- | --- |
| Space+STRG + Pen ↑/↓ | Zoom Canvas |
| Space+SHIFT | Rotate Canvas |
| Space + Pen ←/→ | Brush size |
| M   | Mirror, Flip Canvas |
| E   | Eraser mode |
| Insert | New paint layer |
| Delete | Clear |
| Backspace | Fill w/background color |
| R   | Pick layer |
| Page up | Activate next layer |
| page down | Activate previous layer |
| T   | Move tool |
| P   | Color pick |
| Ctrl+E | Merge down |
| Ctrl+R | Rect. selection |
| Ctrl+T | Transform tool |
| Ctrl+I | Invert |
| Ctrl+J | Duplicate layer |
| Ctrl+L | Levels |
| Ctrl+H | Display selection |
| W   | Wrap around mode |
| /   | Switch to previous preset |
| D   | Reset picker - BW |
| F   | Palette |
| J   | Elliptical selection |
| Shift+Ctrl+A | Deselect |
| Shift+Ctrl+C | Copy merged |
| Shift+I | Color selector |
| Shift+B | Show dockers |
| Shift+Z | Undo polygon selection points |
| Shift+Ctrl+E | Flatten image |
| Shift+Ctrl+F | Full screen mode |
| Shift+Ctrl+U | Desaturate |
| Shift+Ctrl+I | Invert selection |
| Shift+Ctrl+A | Deselect |
| Ctrl+\-/\- | Zoom out |
| Ctrl++/\= | Zoom in |
| 3   | Zoom to fit width |
| 2   | Zoom to fit |
| 1   | Zoom 1:1 |
| 0   | Zoom 1:1 |
| Tab | Canvas only mode |
| F11 | Toggle full screen |
| Shift+Backspace | Fill w/foreground color |
| K   | Darken color |
| B   | Brush tool |
| C   | Show common color |
| L   | Lighten color |
| X   | Swap fg/bg colors |
| H   | Show color history |
| A - Default _None_ | Preserve Alpha |

## Speedlines

* Create another layer > Select the **Ruler Assistant Editor** ; display your _tool option docker_ to select **Parrallel Ruler**.
* Click on the canvas to create a new widget.
* Then go back to the brush tool and in the tool option activate the **Assistant** checkbox. Now all your lines should be parrallel to your ruler.
* When it's over, delete the ruler widget with the **Ruler Assistant Editor** tool.
* You can now transform your line to bring an additional fluid movement to them.
* Note : You can also paint other type of Speedlines using other ruler.

## Cloud particles

* New layer > Layer Style > Outer Glow > Blend Mode > Addition Spread 50% > Size und Color setzen
* Mit Brush z.B. _Texture Splat_ Particle malen
* Verfeinern mit anderer Brush z.B. _Basic 5\_size_
* Schärfe ev. mit _Blender\_Smear_ abschwächen
* Da es Probleme beim Laden von fx-Layern gibt: Merge Down auf leeren Layer, Blending Mode: Addition

## Rain effect

* New layer > Black Color
* Filter > Other > Random Noise
* Farbe entfernen: Filter > Adjust > Desaturate
* Filter > Blur > Gaussian Blur
* Filter > Adjust > Level so einstellen, dass viele weiße Punkte entstehen
* Schwarz entfernen: Filter > Color to Alpha > Schwarz auswählen
* Filter > Blur > Motion Blur
* Mehr hervorheben mit Filter > Color Adjustment > Alpha > Kurve nach li reduzieren

2\. Variante

* Filter > Gimic > Degradations > Rain (geht nur auf Flattened Layer)
* Output Mode > New Layer
* Schwarz entfernen: Filter > Color to Alpha > Schwarz auswählen

## Colorize Mask

* Ink Layer auswählen > Add > Colorize Mask
* Colorize Mask Editing Tool auswählen > Farben markieren
* Transparente Farbe kann in den Tool Options definiert werden
* Ausführen durch _Refresh_ Button der Colorize Mask
* Mit _Pencil_ Button fertigstellen
* Mit _Pencil_ kann Maske verbessert werden
* Mit _Gaussian Blur_ kann Aliasing verbessert werden

## Blending Modes

* _Color Dodge_ für Lichter
* _Color:_ zum Erzeugen einer Basis zum Einfärben von S/W  
    2\. Anwendung zum Desaturieren von Farbe durch Auswahl eines Grautones
* _Overlay:_ Kontrast erhöhen oder Bild mit Textur überlagern
* _Lighten:_ Kontrast reduzieren, damit das Hauptobjekt mehr in den Vordergrund tritt.
* _Multiply:_ zum Hinzufügen von Patterns, Schatten, Tattoos, Make-Up

## Shading

* Layer/s markieren und mit CTRL+SHIFT+G eine Quick Clipping Group mit einem "Mask Layer" mit Alpha Vererbung erzeugen
* Mask Layer mit mittlerem Grau füllen: Aus _Default Palette_ den Farbton _Mid Grey 50%_ auswählen  
  Edit > Fill with Foreground Color Shift+Backspace
* Blending Mode _Lighten > Hard Light_. Der Mode kombiniert die Modes Screen und Multiply
* α-Kanal fixieren.
* Mit Airbrush und hellen/dunklen Farbtönen die Lichter/Schatten malen
* Finish mit _i) Wet\_Textured\_Soft und 80% Opacity_