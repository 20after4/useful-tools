This is just a collection of useful libraries, utilities and development tools that may be worth a look. Most of these are tools that I ( @20after4 ) use on a daily basis.

### Misc.

- https://github.com/jonas/tig - Text-mode Interface for Git. A secret weapon for Git productivity. Quickly browse repositories, view diffs, search commit logs and more. Highly recommended for anyone who prefers a command line but still misses some GUI code browser functionality.
- [https://rclone.org/](https://rclone.org/) -  file management utility for cloud storage.
- https://github.com/pistazie/cdk-dia - generate graphical diagrams of CDK stacks
- [jc](https://github.com/kellyjonbrazil/jc) - parse the output from various command line utilities. Very useful for automating all of the things.
- https://github.com/simonw/datasette - “*An open source multi-tool for exploring and publishing data” - a high quality web (python) application framework built on SQLite with many plugins providing extensive functionality.*
- [https://lite.datasette.io/](https://lite.datasette.io/) - datasette lite is a version of datasette compiled to WebAssembly so that it can run entirely in the browser.
- [https://tmate.io/](https://tmate.io/) - Share a terminal session with a friend/ Great for remote pair programming or demonstration (much more efficient than streaming/screen sharing).

### JSON

- https://github.com/jsonhero-io/jsonhero-web - a feature-rich GUI editor & browser for JSON data.
- https://github.com/antonmedv/fx - a TUI JSON tree viewer & query tool.
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
