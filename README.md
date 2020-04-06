# You Dont Know JS EPUB/PDF

Generate `.epub` end `.pdf` files from [You Dont Know JS](https://github.com/getify/You-Dont-Know-JS) repository.

## Requirements - Generic

To generate the E-Books and PDFs, you must install `ruby` and a recent version of`pandoc`.


## Requirements - Ubuntu 18.04
I use this on Ubuntu 18.04 LTS, some extra info for that platform:

You need to install 'pandoc' from its DEBian package, do not use the Ubuntu supplied packages, they're too old.

You probably also need to install some latex related extras:
```console
$ apt-get install texlive-latex-extra texlive-xetex librsvg2-bin
```

## Instructions

Clone this repository and run the `convert.rb` script:

```console
$ git clone https://github.com/yoeriapts/ydkjs-epub
$ cd ydkjs-epub

$ ruby convert.rb
```

The script will create a `books` folder with sub-folders `1st-ed` and `2nd-ed`.

```console
$ tree books
books
├── 1st-ed
│   ├── You Dont Know JS: Async & Performance.epub
│   ├── You Dont Know JS: Async & Performance.pdf
│   ├── You Dont Know JS: ES6 & Beyond.epub
│   ├── You Dont Know JS: ES6 & Beyond.pdf
│   ├── You Dont Know JS: Scope & Closures.epub
│   ├── You Dont Know JS: Scope & Closures.pdf
│   ├── You Dont Know JS: This & Object Prototypes.epub
│   ├── You Dont Know JS: This & Object Prototypes.pdf
│   ├── You Dont Know JS: Types & Grammar.epub
│   ├── You Dont Know JS: Types & Grammar.pdf
│   ├── You Dont Know JS: Up & Going.epub
│   └── You Dont Know JS: Up & Going.pdf
└── 2nd-ed
    ├── You Dont Know JS: ES Next Beyond.epub
    ├── You Dont Know JS: ES Next Beyond.pdf
    ├── You Dont Know JS: Get Started.epub
    ├── You Dont Know JS: Get Started.pdf
    ├── You Dont Know JS: Objects Classes.epub
    ├── You Dont Know JS: Objects Classes.pdf
    ├── You Dont Know JS: Scope Closures.epub
    ├── You Dont Know JS: Scope Closures.pdf
    ├── You Dont Know JS: Sync Async.epub
    ├── You Dont Know JS: Sync Async.pdf
    ├── You Dont Know JS: Types Grammar.epub
    └── You Dont Know JS: Types Grammar.pdf
````

## License

The script is available as open source under the terms of the [MIT License](http://opensource.org/licenses/MIT).
