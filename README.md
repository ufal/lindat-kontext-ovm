# Lindat test corpora

A collection of precompiled corpora to be used for development and testing of [lindat-kontext](https://github.com/ufal/lindat-kontext)

## Usage

Checkout and point your context config to `corplist.xml`.

Work with default paths:
```
mkdir -p /opt/lindat
cd /opt/lindat
git clone https://github.com/ufal/lindat-test-corpora.git
```

*config.xml*://plugins/corparch
```
<corparch>
    ...
    <file>/opt/lindat/lindat-test-corpora/corplist.xml</file>
    <root_elm_path>/corplist_root</root_elm_path>
    ...
</corparch>
```

*config.xml*:/kontext/corpora/manatee_registry
```
<manatee_registry>/opt/lindat/lindat-test-corpora/registry</manatee_registry>
```
*TODO* can this be "autoincluded"?

## Adding new

Add [corpus configuration file](https://www.sketchengine.co.uk/documentation/the-corpus-configuration-file/) into `registry/` directory and the compiled corpus into `data/`. Update `corplist.xml` and this README accordingly. 

## Available corpora

List of available compiled corpora and their licenses below

----

### OVM – Otázky Václava Moravce prepared for kontext

Original dataset is available at http://hdl.handle.net/11858/00-097C-0000-000D-EC98-3. 

Converted to NoSketchEngine format, see http://nlp.fi.muni.cz/trac/noske. 
Used by https://github.com/ufal/lindat-kontext-vagrant.

#### License

[Attribution-NonCommercial 3.0 Unported (CC BY-NC 3.0)](http://creativecommons.org/licenses/by-nc/3.0/)

----
