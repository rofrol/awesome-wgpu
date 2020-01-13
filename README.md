# Awesome wgpu-rs

A curated list of wgpu-rs code and resources. 

PRs welcome.

## About wgpu-rs

- https://github.com/gfx-rs/wgpu-rs
- wgpu suports DX11, DX12 and Vulkan on Windows, Vulkan on Linux and Metal on macOS & iOS https://github.com/gfx-rs/wgpu
- [The rise of wgpu - Gfx-rs nuts and bolts](https://gfx-rs.github.io/2019/03/06/wgpu.html)
  - https://www.reddit.com/r/rust/comments/ay3olj/the_rise_of_wgpurs/
  - https://news.ycombinator.com/item?id=19327043
- current status of WebGPU in web browsers https://webgpu.io
  - https://www.reddit.com/r/rust_gamedev/comments/e9nh8w/current_status_of_webgpu_wasm_and_web_games_in/
- https://wiki.alopex.li/AGuideToRustGraphicsLibraries2019
- wgpu-rs and WebGL https://www.reddit.com/r/rust/comments/eh7wkx/the_state_of_ggez_2020/fcipapq/
- wgpu-rs and OpenGL https://www.reddit.com/r/rust/comments/eh7wkx/the_state_of_ggez_2020/fcj2hyq/
- Geometry shaders are effectively a dead https://www.reddit.com/r/rust/comments/dou249/will_wgpu_support_shader_types_that_are_not/f5r1a6k/
- https://www.reddit.com/r/rust_gamedev/comments/b01zy9/please_help_me_understand_the_gfxrs_architecture/

## Learn

- https://rust-tutorials.github.io/learn-wgpu
- https://github.com/sotrh/learn-wgpu
- old https://github.com/fredlangva/WGPU-Tut
- https://www.reddit.com/r/rust_gamedev/comments/bcjdl0/learning_wgpurs_coming_from_openwebgl/
- [3D Game in Rust #2 - Try to run a wgpu-rs tutorial - YouTube](https://www.youtube.com/watch?v=KZTmTbcA-VY)

## Gamedev

- An opinionated 2D game engine https://github.com/hecrj/coffee
- A tiny hardware-accelerated pixel frame buffer https://github.com/parasyte/pixels
  - Answer why RedrawRequested event is not implemented https://github.com/rukai/winit_input_helper/issues/3#issuecomment-545316276
  - https://github.com/JamesPatrickGill/mos-6502-rusted
- RTS game/engine https://github.com/Ruddle/oxidator
- https://github.com/maroider/overlay
- https://github.com/Noxime/vg-test
- https://github.com/robmikh/goldsrc-asset-viewer
- https://github.com/vulpesgames/mist-game-engine
- https://github.com/chutchinson/chip-8
- https://github.com/Napokue/chip-8
- https://github.com/deadcore/playstation-emulator
- https://github.com/catt-io/romy
- https://github.com/lavignes/dth
- 2D rendering library https://github.com/tonis2/felin
- 2D graphics library https://github.com/cloudhead/rgx used by https://github.com/cloudhead/rx

## Games

- https://github.com/rukai/canon_collision
- https://github.com/kvark/vange-rs
  - https://kvark.github.io/vange-rs/
- https://github.com/Technici4n/voxel-rs
- 2D, space invaders clone https://github.com/parasyte/pixels/tree/master/examples/invaders
- 2D, game of life https://github.com/parasyte/pixels/tree/master/examples/conway
- https://github.com/terrence2/openfa
- https://github.com/derekdreery/rogue
- https://github.com/Limvot/vulkemon
- https://github.com/glalonde/spout/tree/master/rust

## Applications

- pixel editor https://github.com/cloudhead/rx
- https://github.com/Yatekii/sailor
- https://github.com/manuranga/igni
- https://github.com/stevebob/rip
- https://github.com/chiptunecafe/rawrscope
- https://github.com/cbrewster/brewcode
- https://github.com/Elyhaka/Swaynimated
- https://github.com/CryZe/livesplit-one-desktop

## Examples

- https://github.com/gfx-rs/wgpu-rs/tree/master/examples
- https://github.com/LordBenjamin/sharp-and-rusty
- https://github.com/rohit507/rust-gfx-experiments
- https://github.com/stevebob/hello-wgpu
- https://github.com/vitvakatu/cubes
- https://github.com/laopo001/wgpu-learn
- https://github.com/xayon40-12/wgpu_ray
- https://github.com/maroider/wgpu_playground
- https://github.com/terrence2/stampede
- https://github.com/Lonsdaleiter/RustTest

### Older

- https://github.com/timokoesters/wgpu-project
- https://github.com/WaDelma/hiekkapeli
- https://github.com/krauslabs/wgpu-vg-toy
- https://github.com/fredlangva/wgpu_one
  - https://www.reddit.com/r/rust/comments/c9wsot/i_need_some_help_with_wgpu/
- https://github.com/WaDelma/hiekkapeli
- https://github.com/menuan/lack

## UI

- https://github.com/hecrj/iced
- https://github.com/dhardy/kas
  - https://www.reddit.com/r/rust/comments/ebvp4i/kas_gui/
- https://github.com/redox-os/orbtk

## Rendering

- some parts of rendy used by wgpu-rs https://github.com/rust-tutorials/learn-rendy
- svg https://github.com/nical/lyon
- https://github.com/mikialex/rendiation
- text https://github.com/hecrj/wgpu_glyph
- render bitmap fonts without jagged edges even at high magnifications https://github.com/grenlight/sdf-text-view
- terminal https://github.com/stevebob/prototty
- physically-based renderer https://github.com/mad-s/hijiki

## About Rendy

About Rendy and wgpu https://community.amethyst.rs/t/skepticism-about-rendy/1221/9

>wgpu uses gfx-hal and parts of rendy, totally fine on DX12 on Windows https://www.reddit.com/r/rust/comments/eh7wkx/the_state_of_ggez_2020/fcj1746/

>We hoped Amethyst team would help, but that didn't happen either. https://www.reddit.com/r/rust/comments/eh7wkx/the_state_of_ggez_2020/fcipapq/

>Switching to rendy nearly killed this project due to the time and effort required https://community.amethyst.rs/t/skepticism-about-rendy/1221/11

>This duality of APIs in gfx-hal worked to an extent. Providing safety was impossible without imposing some restrictions or overhead. In the command pool example, it’s only safe to re-use a command buffer if it’s done execution on the GPU, and the user doesn’t intent to use it. We can’t possibly know this in gfx-hal without introducing overhead… So, at the end of the day, we decided that the “typed” (user-facing) layer is still useful, it doesn’t have to be a part of gfx-hal. Thus, we removed it, recommending rendy-command as a replacement. This slimmed up gfx-hal API surface and allowed us to straighten up the terminology (no more “RawXXX” or “XxxTyped”). https://gfx-rs.github.io/2019/10/01/update.html

## Misc

- Processing-esque https://github.com/flmng0/peach
- Wave Function Collapse https://github.com/stevebob/wfc
- process images on the GPU https://github.com/danielbusaba/Rust-GPU
- LBM fluid simulation https://github.com/grenlight/fluid-webgpu
- Safe Wrapper Around the Chromium Embedded Framework https://github.com/anlumo/cef

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)
