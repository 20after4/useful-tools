This is just a collection of useful libraries, utilities and development tools that may be worth a look. Most of these are tools that I ( [@20after4](https://github.com/20after4/) ) use on a daily basis.

### Home Automation

- [ESPHome](https://esphome.io) - Makes it simple to connect just about any imaginable sensor or device to your home network. ESPHome is a firmware for microcontrollers which is easy to customize using a simple YAML configuration. Out of the box support for literally [100s of devices](https://esphome.io/components/) such as [atmospheric sensors](https://esphome.io/components/sensor/bme280), [biometrics](https://esphome.io/components/fingerprint_grow.html), [energy monitoring](https://esphome.io/#electricity), and many more. If you can imagine a way to connect or monitor something, ESPHome probably already has a driver for it, complete with ready to use example configurations.  Anything that isn't already supported is easy to add with just a bit of C++ code. This project is really cool! 
- [Home Assistant](https://www.home-assistant.io/) - a really high quality home automation controller and monitoring platform. With this running on a Raspberri Pi and a few ESPHome devices, you have a complete smart home system with 100% open source software. Easily integrates with just about every other home automation system out there. More importantly, it's a really well run project with great code quality, a great community, good security practices and good free software values.


### Misc.

- [tig](https://github.com/jonas/tig) - Text-mode Interface for Git. A secret weapon for Git productivity. Quickly browse repositories, view diffs, search commit logs and more. Highly recommended for anyone who prefers a command line but still misses some GUI code browser functionality.
- [rclone](https://rclone.org/) -  file management utility for cloud storage.
- https://github.com/pistazie/cdk-dia - generate graphical diagrams of CDK stacks
- [jc](https://github.com/kellyjonbrazil/jc) - parse the output from various command line utilities. Very useful for automating all of the things.
- https://github.com/simonw/datasette - “*An open source multi-tool for exploring and publishing data” - a high quality web (python) application framework built on SQLite with many plugins providing extensive functionality.*
- [https://lite.datasette.io/](https://lite.datasette.io/) - datasette lite is a version of datasette compiled to WebAssembly so that it can run entirely in the browser.
- [https://tmate.io/](https://tmate.io/) - Share a terminal session with a friend/ Great for remote pair programming or demonstration (much more efficient than streaming/screen sharing).
- [silverbullet.md](https://silverbullet.md/) - Markdown-based note taking app with collaboration using [CRDTs](https://en.wikipedia.org/wiki/Conflict-free_replicated_data_type)
- [red](https://github.com/antonmedv/red) - a terminal-based log analysis tool

### JSON

- https://github.com/antonmedv/fx - a TUI JSON tree viewer & query tool.
- https://github.com/jsonhero-io/jsonhero-web - a feature-rich GUI editor & browser for JSON data.
- https://github.com/blackflux/object-scan - an efficient and powerful library for traversing and extracting data from JavaScript object hierarchies.
    - Trivial Example
        
        ```jsx
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
