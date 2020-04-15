# Awesome wgpu

A curated list of wgpu code and resources.

PRs welcome.

## About wgpu

- https://github.com/gfx-rs/wgpu-rs
- matrix chat https://matrix.to/#/#wgpu:matrix.org
- wgpu suports DX11, DX12 and Vulkan on Windows, Vulkan on Linux and Metal on macOS & iOS https://github.com/gfx-rs/wgpu
- [The rise of wgpu - Gfx-rs nuts and bolts](https://gfx-rs.github.io/2019/03/06/wgpu.html)
  - https://www.reddit.com/r/rust/comments/ay3olj/the_rise_of_wgpurs/
  - https://news.ycombinator.com/item?id=19327043
- current status of WebGPU in web browsers https://webgpu.io
  - https://www.reddit.com/r/rust_gamedev/comments/e9nh8w/current_status_of_webgpu_wasm_and_web_games_in/
- https://wiki.alopex.li/AGuideToRustGraphicsLibraries2019
- wgpu and WebGL https://www.reddit.com/r/rust/comments/eh7wkx/the_state_of_ggez_2020/fcipapq/
- wgpu and OpenGL https://www.reddit.com/r/rust/comments/eh7wkx/the_state_of_ggez_2020/fcj2hyq/
- Geometry shaders are effectively a dead end https://www.reddit.com/r/rust/comments/dou249/will_wgpu_support_shader_types_that_are_not/f5r1a6k/
- https://www.reddit.com/r/rust_gamedev/comments/b01zy9/please_help_me_understand_the_gfxrs_architecture/

## Ecosystem

1. individual API libraries like ash, d3d12-rs, metal-rs - for the lowest hard-core level available to Rust
2. gfx-hal for lowest portable level
3. Rendy for helping to solve the rough corners of gfx-hal
4. wgpu-rs for the lowest safe level
5. Engines like ggez or Amethyst for the highest level

https://www.reddit.com/r/rust_gamedev/comments/bv7w2f/wgpurs_now_uses_rendy_to_manage_memory_and/

## Learn

- https://rust-tutorials.github.io/learn-wgpu
  - https://github.com/rust-tutorials/learn-wgpu
- https://sotrh.github.io/learn-wgpu/
  - https://github.com/sotrh/learn-wgpu
  - this guide https://vulkano.rs/guide/introduction explains more i.e. swapchain https://vulkano.rs/guide/swapchain-creation
    - https://github.com/vulkano-rs/vulkano-www
  - https://crates.io/crates/winit
  - https://crates.io/crates/wgpu
- old https://github.com/fredlangva/WGPU-Tut
- https://www.reddit.com/r/rust_gamedev/comments/bcjdl0/learning_wgpurs_coming_from_openwebgl/
- [3D Game in Rust #2 - Try to run a wgpu-rs tutorial - YouTube](https://www.youtube.com/watch?v=KZTmTbcA-VY)
- [Get started with GPU Compute on the Web](https://developers.google.com/web/updates/2019/08/get-started-with-gpu-compute-on-the-web)

## Gamedev

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
- https://github.com/StarlitGhost/GBOxide
- A brawl file parser for Super Smash Bros. Brawl https://github.com/rukai/brawllib_rs
- An opinionated 2D game engine https://github.com/hecrj/coffee
  - based on old wgpu 0.2

## Rust gamedev

- https://github.com/rust-unofficial/awesome-rust/blob/master/README.md#game-development
- https://www.reddit.com/r/rust_gamedev
- Lack of allocator support in std is a big issue for gamedev. https://www.reddit.com/r/rust/comments/cr5rht/whats_the_state_of_game_development_in_rust/ex3g6e9/
- Game Input Library for Rust https://github.com/Arvamer/gilrs
  - Used by https://github.com/parasyte/pixels
- [How to make roguelike games in Rust](http://bfnightly.bracketproductions.com/rustbook/)
  - https://news.ycombinator.com/item?id=22020229
- Ultraviolet (linear algebra library specifically for games & graphics which is faster than the alternatives for both runtime and compile times) https://crates.io/crates/ultraviolet
  - via https://news.ycombinator.com/item?id=22024916
- experimental const generics based linear algebra library that works without any allocations in no_std and utilizes simd. So now you can do fancy maths on embedded. https://djugei.github.io/optimath-0-3-0/
  - https://www.reddit.com/r/rust/comments/eo4ury/show_rrust_optimath_linear_algebra_with_const/
- High performance Rust ECS library https://crates.io/crates/legion
  - via https://news.ycombinator.com/item?id=22024916
  - The flexibility in Legion is filled with tradeoffs, generally showing benefits in performance and runtime flexibility, while generally trading off some of the ergonomics of the SPECS interface. https://github.com/amethyst/rfcs/issues/22
- https://iolivia.me/posts/entity-component-system-explained/
- https://github.com/rukai/winit_input_helper
  - used by pixels and others https://crates.io/crates/winit_input_helper/reverse_dependencies
- experimental Rust library for continuous 2D collision detection in games https://github.com/SergiusIW/collider-rs
  - https://github.com/SergiusIW/chirperjax
- development library tailored to 2D pixel-art games. Supports SDL2 or WebAssembly https://github.com/SergiusIW/gate
  - https://github.com/SergiusIW/chirperjax

## General gamedev

- https://gafferongames.com/post/fix_your_timestep/
  - via https://github.com/17cupsofcoffee/tetra
- https://gafferongames.com/post/integration_basics/
- https://www.reddit.com/r/gamedev/comments/df7dth/i_compiled_a_massive_list_of_yt_channels_about/
- https://gamedev.stackexchange.com/questions?tab=Votes

## Physics/Collision

- http://arewegameyet.com/categories/physics/
- https://github.com/kvark/vange-rs/blob/master/bin/road/physics/mod.rs
- https://github.com/kvark/vange-rs/blob/master/src/render/collision.rs
- https://github.com/rukai/canon_collision/blob/master/canon_collision/src/collision.rs

## Games

- https://github.com/rukai/canon_collision
- https://github.com/kvark/vange-rs
  - https://kvark.github.io/vange-rs/
  - In a nutshell, it's Metal with Vulkan's binding model https://www.reddit.com/r/rust_gamedev/comments/bcjdl0/learning_wgpurs_coming_from_openwebgl/ektqwx3/
- https://github.com/Technici4n/voxel-rs
- 2D, space invaders clone https://github.com/parasyte/pixels/tree/master/examples/invaders
- 2D, game of life https://github.com/parasyte/pixels/tree/master/examples/conway
- https://github.com/terrence2/openfa
- https://github.com/derekdreery/rogue
- https://github.com/Limvot/vulkemon
- https://github.com/glalonde/spout/tree/master/rust
- https://github.com/Limvot/vulkemon

## Applications

- pixel editor https://github.com/cloudhead/rx
- https://github.com/Yatekii/sailor
- Realtime 3D N-Body-Simulation: https://git.koesters.xyz/timo/nbodysim
- https://github.com/manuranga/igni
- https://github.com/stevebob/rip
- https://github.com/chiptunecafe/rawrscope
- https://github.com/cbrewster/brewcode
- https://github.com/Elyhaka/Swaynimated
- https://github.com/CryZe/livesplit-one-desktop
- HDR image viewer https://github.com/mandeep/viewimg
  - Radiance HDR images (and later OpenEXR)

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
- iOS and Metal https://github.com/grenlight/idroid_demo

### Older

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
- bindings for Nuklear (using old `wgpu = "~0.3"`) https://github.com/snuk182/nuklear-backend-wgpurs

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

## WebGPU and portability

>One of the goals of WebGPU that differentiates it from the other libraries and APIs is "strong" portability, in a sense that it not only runs on all targeted platforms, but also the performance expectations match. Therefore, if don't see a way to consistently implement a feature on at least 2 or the 3 target platforms, in such a way that it works and using it shows a difference, we don't include it in the core API. Take sub-passes, for example, that, while you can technically implement them on Metal and DX12 by doing separate passes, they only make a difference on Vulkan mobile GPUs today, so there can't be expectation that using sub-passes makes you magically faster. Take buffer capabilities as another example: if we expose all the queries about what is supported and what not, it's easy to write an application that would work on the developer platform but then break on others, because they possibly forgot to query, or simply don't have another code path in place. Finally, things like "multiple queues" are desired for the most part, but we haven't yet figured a plan on how to expose them portably, as in - without race conditions affecting the portability of user programs. https://github.com/nannou-org/nannou/issues/374#issuecomment-533841665

## Misc

- Processing-esque https://github.com/flmng0/peach
- Wave Function Collapse https://github.com/stevebob/wfc
- process images on the GPU https://github.com/danielbusaba/Rust-GPU
- LBM fluid simulation https://github.com/grenlight/fluid-webgpu
- Safe Wrapper Around the Chromium Embedded Framework https://github.com/anlumo/cef

## Shading Language

- https://www.reddit.com/r/shaders/
- https://github.com/topics/shading-language
- https://github.com/KhronosGroup/Vulkan-Ecosystem
- books, editors, viewers recommendations https://www.reddit.com/r/gamedev/comments/cis14v/good_starting_points_for_learning_to_write_shaders/

### GLSL

>Found the problem - I need to become a GLSL shader expert https://www.reddit.com/r/rust_gamedev/comments/be08e2/wgpu_pipeline_question/el40lsl/

- https://github.com/radixzz/awesome-glsl
- https://thebookofshaders.com/
- https://vulkan-tutorial.com/Drawing_a_triangle/Graphics_pipeline_basics/Shader_modules
- https://www.lunarg.com/faqs/how-vulkan-shaders-written/
- https://www.khronos.org/opengl/wiki/Core_Language_(GLSL)
  - https://www.khronos.org/registry/OpenGL/specs/gl/GLSLangSpec.4.50.pdf
- https://www.khronos.org/opengl/wiki/OpenGL_Shading_Language
- https://www.reddit.com/r/rust_gamedev/comments/bcjdl0/learning_wgpurs_coming_from_openwebgl/eku9bsr/
- mandelbrot https://vulkano.rs/guide/mandelbrot
- https://stackoverflow.com/questions/16631981/what-is-the-difference-between-opengl-and-glsl
- https://gamedev.stackexchange.com/questions/4234/what-are-the-pros-and-cons-of-hlsl-vs-glsl-vs-cg
- https://community.khronos.org/t/glsl-and-hlsl-differences/53888/4
- https://stackoverflow.com/questions/2508818/how-to-debug-a-glsl-shader
- https://stackoverflow.com/questions/tagged/glsl?tab=Votes
- https://riptutorial.com/glsl
- http://nehe.gamedev.net/article/glsl_an_introduction/25007/index.html
- https://docs.unity3d.com/2020.1/Documentation/Manual/SL-GLSLShaderPrograms.html
- https://github.com/libretro/glsl-shaders

### HLSL

>Google and Samsung are developing HLSL compiler for Vulkan, because a large majority of game studios don't want to bother with Vulkan on Android if they cannot port their shaders. https://news.ycombinator.com/item?id=18439910

- https://github.com/KhronosGroup/glslang/wiki/HLSL-FAQ
  - [Complete HLSL -> SPIR-V translator · Issue #362 · KhronosGroup/glslang](https://github.com/KhronosGroup/glslang/issues/362)
- Make HLSL a first-class citizen for Vulkan https://www.khronos.org/assets/uploads/developers/library/2019-siggraph/Vulkan-06-DXC-Update_SIGGRAPH_Jul19.pdf
- https://github.com/microsoft/DirectXShaderCompiler#spir-v-codegen
- https://github.com/google/shaderc-rs
- https://www.reddit.com/r/gamedev/comments/cpdtn6/looking_for_ressources_to_learn_hlsl/

### GLSL vs HLSL

- use of raw GLSL is only recommended for testing, or when you know you are only targeting Mac OS X, OpenGL ES mobile devices, or Linux. In all normal cases, Unity will cross-compile Cg/HLSL into optimized GLSL when needed. https://docs.unity3d.com/2020.1/Documentation/Manual/SL-GLSLShaderPrograms.html

>My biggest concerns about using HLSL as the source are:
> - poor specification, or the lack of it
> - alien binding model: GLSL can easily specify descriptor sets and bindings, while HLSL was to resort to a parser-specific attribute magic to specify them.
>https://www.reddit.com/r/rust_gamedev/comments/cgaeuu/graphics_programming_hlsl_vs_glsl/eukphqa/


### WSL (formerly WHLSL)

>There are many Web developers using GLSL today in WebGL, so a potential browser accepting a different high level language, like HLSL, wouldn’t suit their needs well. In addition, a high-level language such as HLSL can’t be executed faithfully on every platform and graphics API that WebGPU is designed to execute on. https://webkit.org/blog/9528/webgpu-and-wsl-in-safari/
>
>So, we decided to make the language more simple, low-level, and fast to compile, and renamed the language to Web Shading Language to match this pursuit.

- [WHLSL: Web High Level Shading Language | Hacker News](https://news.ycombinator.com/item?id=18436961)
- https://github.com/gpuweb/WSL

### CG

>CG has been discontinued, and is no longer supported or actively worked on by Nvidia. Nvidia recommends that all users switch to a combination of GLSL and HLSL, or a newer library such as nvFX (on github). This is because it was too difficult to maintain feature-compatibility between GLSL and HLSL. https://gamedev.stackexchange.com/questions/4234/what-are-the-pros-and-cons-of-hlsl-vs-glsl-vs-cg/4333#4333

## OpenGL

- OpenGL is never going to magically become an API that works everywhere portably https://www.reddit.com/r/rust/comments/eh7wkx/the_state_of_ggez_2020/fcj2hyq/

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)
