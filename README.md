# Keyboards

![Four of my boards: an Osprangle, a Clog V2, an Osprette, and a Sephirette](images/collage.jpg)

I design open-source 34-key columnar keyboards with pinky clusters. There are two families, the [Osprettes][osprette]
(unibodies) and the [Clogs][clog] (splits).

## [The Osprette family][osprette] (unibodies)

The OG, based on the [balbuzard]. Great for never having to move your hands, only your fingers.

Best for travel.

![The Osprangle](images/osprangle.jpg)

| Board                                              | Switches      | Controller | Notes                        |
| -------------------------------------------------- | ------------- | ---------- | ---------------------------- |
| [Osprette](../../../osprette/tree/main/v1)         | Choc V1       | Pro Micro  | the original                 |
| [Osprette V2](../../../osprette/tree/main/v2)      | Choc V1       | Pro Micro  | nicer case, optional hotswap |
| [Osprette V3](../../../osprette/tree/main/v3)      | Choc V1       | Pro Micro  | direct solder                |
| [Osprette MX](../../../osprette/tree/main/mx)      | MX            | Pro Micro  | MX version                   |
| [Osprangle](../../../osprette/tree/main/osprangle) | Choc V2       | Pro Micro  | hotswap                      |
| [Roadkill](../../../osprette/tree/main/roadkill)   | Kailh PG1316S | Pro Micro  | butterfly switches           |

## [The Clog][clog] family (splits)

The same dang thing, cleft in twain. Slightly better for ergonomics if you have the desk space.

Best for home.

![The Steel Toe](images/steel-toe.jpg)

| Board                                            | Switches | Controller | Notes                          |
| ------------------------------------------------ | -------- | ---------- | ------------------------------ |
| [Clog](../../../clog/tree/main/v1)               | Choc V1  | Pro Micro  | the original split             |
| [Clog V2](../../../clog/tree/main/v2)            | Choc V1  | Xiao BLE   | wireless only, splay, roller   |
| [Clog V3](../../../clog/tree/main/v3)            | Choc V1  | Pro Micro  | solder or hotswap              |
| [Clog V4](../../../clog/tree/main/v4)            | Choc V1  | Xiao       | hotswap with a switch plate    |
| [Steel Toe](../../../clog/tree/main/steel-toe)   | Choc V1  | Pro Micro  | BoardSource's V3-derived board |
| [Sephirette](../../../clog/tree/main/sephirette) | MX       | Pro Micro  | MX split                       |

## Firmware

The Osprette boards all use the same `osprette` firmware in QMK and `osprette` shield in ZMK. The Clog boards share the
`clog` firmware in QMK and ZMK, though the Clog V2 has its own ZMK-only config, and Clog V4 runs the `geta` shield in my
[zmk-config].

My personal keymaps live in [qmk_userspace] and [zmk-config].

## Building

Most boards use my [smores.pretty][smores-pretty] KiCad library as a submodule, so clone with `--recurse-submodules`.
The original Osprette, Osprette MX, Clog, and Sephirette use Foostan's `kbd` and Daprice's `keyswitches.pretty` instead.
Each board's README has ordering details and pictures.

## Earlier designs

- [Fun Size][fun-size]: a 32-36 key hotswap low-profile board with encoder support.
- [Mankoffskey]: a 42-key split.
- [Papasweep]: a one-handed MX board for typing with [taipo].

[balbuzard]: https://github.com/brow/balbuzard
[clog]: ../../../clog
[fun-size]: ../../../fun-size
[mankoffskey]: ../../../mankoffskey
[osprette]: ../../../osprette
[papasweep]: ../../../papasweep
[qmk_userspace]: ../../../qmk_userspace
[smores-pretty]: ../../../smores.pretty
[taipo]: https://inkeys.wiki/en/keymaps/taipo
[zmk-config]: ../../../zmk-config
