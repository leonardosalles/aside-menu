# &lt;aside-menu&gt;

> Create a aside menu with simple and complete skeleton

## Demo

[Check it live!](http://leonardosalles.com/aside-menu/)

## Usage

1. Import Web Components' polyfill:

    ```html
    <script src="lib/platform/platform.js"></script>
    ```

2. Import Custom Element:

    ```html
    <link rel="import" href="src/aside-menu.html">
    ```

3. Start using it!

    ```html
    <aside-menu bartitle="Home" 
		items="[
                	{href: 'home.html', description: 'Home', bartitle: 'Home'},
			{href: 'services.html', description: 'Services', bartitle: 'Services'},
                	{href: 'forum.html', description: 'Forum', bartitle: 'Forum'},
		        {href: 'about.html', description: 'About', bartitle: 'About'},
                	{href: 'blog.html', description: 'Blog', bartitle: 'Blog'}
                       ]" 
		fixed="true" 
		basepath="views" 
		indexview="home.html"></aside-menu>
    ```



## Options

Attribute  | Options                   | Default             | Description
---        | ---                       | ---                 | ---
`bartitle` | *string*                  | null                | Title of you menu header
`fixed`    | *boolean*                 | false               | Indicates if header is fixed
`basepath` | *string*                  | null                | The base path that contains the views
`indexview`| *string*                  | null                | First view should be rendered
`items`    | *array*                   | null                | Array of object with href, description and bartitle of views of menu

## Setup

In order to run it locally you'll need a basic server setup.

1. Install [NodeJS](http://nodejs.org/download/).
2. Install [GruntJS](http://gruntjs.com/):

    ```sh
    $ [sudo] npm install -g grunt-cli
    ```

3. Install local dependencies:

    ```sh
    $ npm install
    ```

4. Run a local server and open `http://localhost:8000`.

    ```sh
    $ grunt connect
    ```

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
