# &lt;aside-menu&gt;

> Create a aside menu with simple and complete skeleton

## Demo

[Check it live!](http://leonardosalles.com/aside-menu/)

## Usage

1. Import Web Components' polyfill:

    ```html
    <script src="lib/platform/platform.js"></script>
    ```

2. Import Custom Element CSS:

    ```html
    <link rel="stylesheet" type="text/css" href="src/aside-menu.css">
    ```

3. Import Custom Element:

    ```html
    <link rel="import" href="src/aside-menu.html">
    ```

4. Start using it!

    ```html
    <aside-menu bartitle="Home" fixed="true" basepath="views" indexview="home.html" id="aside-menu"></aside-menu>
    ```
    
    ```html
    <script type="text/javascript">
        //Select element and set menu items
        var asideMenu = document.querySelector('#aside-menu');
        asideMenu.items = [{href: 'home.html', description: 'Home', bartitle: 'Home'},
                           {href: 'services.html', description: 'Services', bartitle: 'Services'},
                           {href: 'forum.html', description: 'Forum', bartitle: 'Forum'},
                           {href: 'about.html', description: 'About', bartitle: 'About'},
                           {href: 'blog.html', description: 'Blog', bartitle: 'Blog'}];
    </script>
    ```
    



## Options

Attribute  | Options                   | Default             | Description
---        | ---                       | ---                 | ---
`bartitle` | *string*                  | null                | Title of you menu header
`fixedheader`| *boolean*                 | false               | Indicates if header is fixed
`basepath` | *string*                  | null                | The base path that contains the views
`indexview`| *string*                  | null                | First view should be rendered
`items`    | *array*                   | null                | Array of object with href, description and bartitle of views of menu

## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -m 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request :D

## History

For detailed changelog, check [Releases](https://github.com/leonardosalles/aside-menu/releases).

## License

[MIT License](http://opensource.org/licenses/MIT)

## Credits
This HTML and CSS code for skeleton is based on [Diego Eis article](http://tableless.com.br/fazendo-um-slide-menu-mobile-sem-plugin/)


