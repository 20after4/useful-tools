---
aliases:
    - tools
    - cool tools
---
This is just a collection of useful libraries, utilities and development tools that may be worth a look. Most of these are tools that I ( [@20after4](https://github.com/20after4/) ) use on a regular basis.

## Terminal, CLI and TUI Tools
- [kitty](https://sw.kovidgoyal.net/kitty/) - an extremely powerful, customizable and high performance terminal emulator for multiple platforms. Kitty offers several modern extensions to terminal functionality such as inline graphics and advanced text formatting, decorations and more.
- [iterm2](https://iterm2.com/) - honorable mention. iTerm has functionality similar to kitty, and a few features found nowhere else. I used this and loved it in the past when I used a Mac regularly.
- [wezterm](https://wezfurlong.org/wezterm/) - another cross-platform terminal with advanced features. Similar in functionality to Kitty and in some ways even more powerful, however, in my experience it uses more memory and performance seems a bit worse than Kitty. If kitty didn't exist then this would probably be my daily driver.
- [fx](https://github.com/antonmedv/fx) - a TUI JSON tree viewer & query tool. Kind of like jq with a syntax that makes sense and an interactive tree viewer. This is my go-to tool for viewing, searching or mangling JSON at the terminal.
- [jc](https://github.com/kellyjonbrazil/jc) - parse the output from various command line utilities. Very useful for automating all of the things.
- [nnn](https://github.com/jarun/nnn) a flexible and powerful TUI file manager.
- [rclone](https://rclone.org/) - file management utility for cloud storage.
- [red](https://github.com/antonmedv/red) - a terminal-based log analysis tool
- [tig](https://github.com/jonas/tig) - **Text-mode Interface for Git**. A secret weapon for Git productivity. Quickly browse repositories, view diffs, search commit logs and more. Highly recommended for anyone who prefers a command line but still misses some GUI code browser functionality.
- [tmate](https://tmate.io/) - Share a terminal session with a friend/ Great for remote pair programming or demonstration (much more efficient than streaming/screen sharing).
- [up](https://github.com/akavel/up) - interactively build shell pipelines.
- [gomplate](https://github.com/hairyhenderson/gomplate) - Render GO-Templates from the CLI. Can inject values from various data sources and file formats including local or remote files (JSON, YAML), Environment variables, AWS Secrets/Parameter Store, Consul, and a bunch more.
- [xc](https://github.com/joerdav/xc) - a CLI task runner. Execute scripts embeded in markdown.
## Language Servers and Editor Extensions
- [markdown oxide](https://github.com/Feel-ix-343/markdown-oxide) - a language server for note taking with markdown. Supports vs.code and neovim, among others.
    > "*Markdown Oxide is attempting to be the best Personal Knowledge Management (PKM) system for software enthusiasts*"

  *This document was created using markdown oxide.*
- [Pretty-ts-errors](https://marketplace.visualstudio.com/items?itemName=yoavbls.pretty-ts-errors) a VS.code extension that significantly improves the readability and presentation of TypeScript errors in the editor.


## Misc. tools and utilities
- [Datasette](https://github.com/simonw/datasette) - a high quality web (python) application framework built on SQLite with many plugins providing extensive functionality.
  > “*An open source multi-tool for exploring and publishing data*”
- [datasette lite](https://lite.datasette.io/) - Datasette compiled to WebAssembly so that it can run entirely in the browser, no server necessary.
- [cdk-dia](https://github.com/pistazie/cdk-dia) - generate graphical diagrams of CDK stacks
- [silverbullet.md](https://silverbullet.md/) - Markdown-based note taking app with collaboration using [CRDTs](https://en.wikipedia.org/wiki/Conflict-free_replicated_data_type)


## Frameworks and Libraries
* [htl](https://github.com/observablehq/htl) - tagged template literal for HTML by Observablehq
* [lipgloss](https://github.com/charmbracelet/lipgloss) a nice terminal color and style library for go.
* [bubbletea](https://github.com/charmbracelet/bubbletea) TUI framework based for go.
  > "The fun, functional and stateful way to build terminal apps. A Go framework based on The Elm Architecture. Bubble Tea is well-suited for simple and complex terminal applications, either inline, full-window, or a mix of both."

## Servers and Infrastructure Components
* [caddy](https://caddyserver.com/) - a single-binary webserver with automatic ssl certificate management. Extremely easy to configure and deploy yet powerful and versitile. Caddy is a very capable reverse-proxy server and works especially well with node.js and php applications.

### JSON

- [jsonhero](https://github.com/jsonhero-io/jsonhero-web) - a feature-rich GUI editor & browser for JSON data.
- [object-scan](https://github.com/blackflux/object-scan) - an efficient and powerful library for traversing and extracting data from JavaScript object hierarchies.
    - Trivial Example
    ```js
        import objectScan from 'object-scan';

        const haystack = {
         a: {
             b: { c: 'd' },
             e: { f: 'g' }
         }
        };
        const pattern = ['a.*.f'];
        const scanner = objectScan(pattern, { joined: true })

        scanner(haystack);
        // => [ 'a.e.f' ]


    ```

  
## Home Automation

- [ESPHome](https://esphome.io) - Makes it simple to connect just about any imaginable sensor or device to your home network. ESPHome is a firmware for microcontrollers which is easy to customize using a simple YAML configuration. Out of the box support for literally [100s of devices](https://esphome.io/components/) such as [atmospheric sensors](https://esphome.io/components/sensor/bme280), [biometrics](https://esphome.io/components/fingerprint_grow.html), [energy monitoring](https://esphome.io/#electricity), and many more. If you can imagine a way to connect or monitor something, ESPHome probably already has a driver for it, complete with ready to use example configurations.  Anything that isn't already supported is easy to add with just a bit of C++ code. This project is really cool!
- [Home Assistant](https://www.home-assistant.io/) - a really high quality home automation controller and monitoring platform. With this running on a Raspberri Pi and a few ESPHome devices, you have a complete smart home system with 100% open source software. Easily integrates with just about every other home automation system out there. More importantly, it's a really well run project with great code quality, a great community, good security practices and good free software values.


