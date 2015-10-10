# &lt;instagram-user-card&gt;

Web component to show a card of your profile in Instagram using [Polymer](http://polymer-project.org). This project is designed to work with Polymer 1.0.

This is a fork of the project originally created by [Kessiler Rodrigues](https://github.com/kessiler).


## Demo

![Example](card-example.png)

> @NOTE : Data can not be displayed, because Instagram has a limit of 5000 requests per hour.

<!-- [Check it live!](http://kessiler.github.io/instagram-card) -->

## Install

Install the component using [Bower](http://bower.io/):

```sh
$ bower install instagram-user-card --save
```

Or [download as ZIP](https://github.com/willsteinmetz/instagram-user-card/archive/master.zip).

## Usage

1. Import Web Components' polyfill:

    ```html
    <script src="bower_components/webcomponentsjs/webcomponents-lit.min.js"></script>
    ```

2. Import Instagram custom element:

    ```html
    <link rel="import" href="bower_components/instagram-user-card/dist/instagram-user-card.html">
    ```

3. Start using it!

    ```html
    <instagram-user-card access-token="[access token]" client-id="[client id]"></instagram-user-card>
    ```


## Options

Attribute     | Options     | Description
---           | ---         | ---
`clientId`    | *string*    | your id from instagram.
`accessToken` | *string*    | key token of your user.

> @NOTE: If you do not know your clientId, you can search it [here](http://jelled.com/instagram/lookup-user-id).

> @NOTE: If you need an access token, you can generate one [here](http://instagram.pixelunion.net/).


## Development

In order to run it locally you'll need to fetch some dependencies and a basic server setup.

* Install [Bower](http://bower.io/) & [Grunt](http://gruntjs.com/):

    ```sh
    $ [sudo] npm install -g bower grunt-cli
    ```

* Install local dependencies:

    ```sh
    $ bower install && npm install
    ```

* To test your project, start the development server and open `http://localhost:8000`.

    ```sh
    $ grunt server
    ```

## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -m 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request

## License

[MIT License](http://opensource.org/licenses/MIT)
