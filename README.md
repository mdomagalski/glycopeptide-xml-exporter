# glycopeptide-xml-exporter

> Element converts json structure with results (see glycopeptide-multi-result) to xml compatible with MS Excel.
> Results for each mass are saved on separate tabs in tables.

## Usage

1. Import polyfill:

    ```html
    <script src="bower_components/webcomponentsjs/webcomponents-lite.min.js"></script>
    ```

2. Import custom element:

    ```html
    <link rel="import" href="bower_components/glycopeptide-xml-exporter/glycopeptide-xml-exporter.html">
    ```

3. Start using it!

    ```html
    <glycopeptide-xml-exporter></glycopeptide-xml-exporter>
    ```

## Options

Attribute     | Options     | Default      | Description
---           | ---         | ---          | ---
`filename`    | *string*    | ``           | output filename
`json`        | *array*     | ``           | search query results
`xml`         | *number*    | 10           | content of the output xml file

## Methods

Method          | Parameters   | Returns     | Description
---             | ---          | ---         | ---
`download()`    | None.        | Nothing.    | Creates the File object and binds it to the download button
                |              |             | and executes the query for each mass individually.
`jsonToSsXml()` | None.        | Nothing.    | Converts json to the XML content
`newWorksheet()`| None.        | Nothing.    | Converts json to the XML content

## Development

In order to run it locally you'll need to fetch some dependencies and a basic server setup.

1. Install [bower](http://bower.io/) & [polyserve](https://npmjs.com/polyserve):

    ```sh
    $ npm install -g bower polyserve
    ```

2. Install local dependencies:

    ```sh
    $ bower install
    ```

3. Start development server and open `http://localhost:8080/components/glycopeptide-xml-exporter/`.

    ```sh
    $ polyserve
    ```

## History

For detailed changelog, check [Releases](https://bitbucket.org/sib-pig/glycopeptide-xml-exporter/releases).

## License

[MIT License](http://opensource.org/licenses/MIT)
