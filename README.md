# Installation

It's recommended that this plugin is used inside of the require/AMD space and using the brightspot-js-grunt task, as demonstrated in the BSP-101 project
- Pull in via your bower.json. It will be automatically included into your project by brightspot-js-grunt task
- Add "bsp-lazyimage" into your compile.js to have it be included in your JS output
- Add in your markup 

Examples:

    1)  <span data-bsp-lazyimage data-src="asdf.jpg" alt="asdf" class="asdf"></span>
    
    2)  <img data-bsp-lazyimage data-src="asdf.jpg" alt="asdf" class="asdf"></img>

    3)  <div data-bsp-lazyimage>
            <span data-src="asdf.jpg" alt="asdf" class="asdf"></span>
            <span data-src="asdf.jpg" alt="asdf" class="asdf"></span>
        </div>

    4)  <picture class="asdf" data-bsp-lazyimage>
            <source data-srcset="/asdf.jpg" media="(max-width: 767px)">
            <img data-srcset="asdf.jpg" alt="Responsive Image">
        </picture>


If you would like to use the lazy-loader utility instead, you can require it, and then use any of the documented public APIs (addItems, createCheckListeners, checkItems, renderImage)