# ESDoc (fork from https://github.com/esdoc/esdoc.git)


ESDoc is a documentation generator for JavaScript.<br/>
Please <a href="https://try.esdoc.org">try it out</a>!

<img class="screen-shot" src="https://raw.githubusercontent.com/esdoc/esdoc/master/manual/asset/image/top.png" width="500px" style="max-width: 500px; border: 1px solid rgba(0,0,0,0.1); box-shadow: 1px 1px 1px rgba(0,0,0,0.5);">

# Features
- Generates good documentation.
- Measures documentation coverage.
- Integrate test codes into documentation.
- Integrate manual into documentation.
- Parse ECMAScript proposals.
- [ESDoc Hosting Service](https://doc.esdoc.org)

And [more](https://github.com/search?o=desc&q=esdoc+filename%3Apackage.json+-user%3Ah13i32maru+-user%3Aesdoc+-user%3Aes-doc&ref=searchresults&s=indexed&type=Code&utf8=%E2%9C%93).

# Quick Start
```sh
# move to a your project directory
cd your-project/

# install ESDoc and standard plugin
npm install @zigen/esdoc esdoc-standard-plugin unscope-package

# unscoping @zigen/esdoc => esdoc, add this configuration to package.json

"scripts" : {
  "postinstall: "unscope-package"
},
"unscope": [
  "@zigen/esdoc"
]

# write a configuration file.
echo '{
  "source": "./src",
  "destination": "./docs",
  "plugins": [{"name": "esdoc-standard-plugin"}]
}' > .esdoc.json

# run ESDoc
./node_modules/.bin/esdoc

# see a documentation
open ./docs/index.html
```

# Document
please visit [esdoc.org](https://esdoc.org) to see more documentation.

# License
MIT

# Author
[Ryo Maruyama@h13i32maru](https://twitter.com/h13i32maru)
