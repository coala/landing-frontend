# landing-frontend
This is the coala frontend Landing Page which uses - https://gitlab.com/coala/landing as its backend.

## Usage

To run locally, first clone the repository:
```sh
    $ git clone https://github.com/coala/landing-frontend.git
    $ cd landing-frontend
```
Then to run the server:
```sh
    $ python2 -m SimpleHTTPServer 8080 #For python 2.x
```
or
```sh
    $ python3 -m http.server 8080 #For python 3.x
```

Open http://localhost:8080 in your browser.


## Adding new code snippets

- Open /data/snippets and add .md file with code snippet in it.
- Enclose that code snippet with ```.
- Open /resources/js/snippets.js and add the name of newly added
 language and the name of its corresponding .md file.
