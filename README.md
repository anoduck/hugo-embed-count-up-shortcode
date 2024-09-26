```text
  _  _             __ _                   __  __              _   
 | || |   _  _    / _` |   ___      o O O|  \/  |   ___    __| |  
 | __ |  | +| |   \__, |  / _ \    o     | |\/| |  / _ \  / _` |  
 |_||_|   \_,_|   |___/   \___/   TS__[O]|_|__|_|  \___/  \__,_|  
_|"""""|_|"""""|_|"""""|_|"""""| {======|_|"""""|_|"""""|_|"""""| 
"`-0-0-'"`-0-0-'"`-0-0-'"`-0-0-'./o--000'"`-0-0-'"`-0-0-'"`-0-0-' 
```

Hugo Embed Count Up Shortcode
=============================

A count up timer is the opposite of a countdown timer, instead of counting down towards an event, a count up timer counts up from an event. Often in the world of apps, these are referred to as "stopwatches", but labeling it as such is a misnomer. 

Usage
-----

This module should follow the same convention of installation as other Hugo modules, and is as follows:

1. Add the module to your go.mod

```bash
hugo mod fetch github.com/anoduck/hugo-embed-count-up-shortcode:latest
```

2. Then add the module to your config.toml or your config.yaml or your hugo.toml or your hugo.yaml etc, etc...

```toml
[[module.imports]]
	path = "github.com/anoduck/hugo-embed-count-up-shortcode"
```

3. Then use the shortcode like so `{{< countup date="$DATE_STRING" >}}`. 

```html
{{< countup date="2023-06-04" >}}
```

If you happen to leave off the `date=`, then the shortcode should accept the date as a positional argument, and that will work as well.

### Caveats

There is no guarantee that this shortcode will work for your particular Hugo configuration, this is because the shortcode is reliant on inline JavaScript to continually parse the difference of the two dates.


License
-------

Licensed under MIT License 2024 @ https://anoduck.mit-license.org
