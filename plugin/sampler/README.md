## sampler.js
> A [reveal.js][] plugin to include code samples in slides


### Dependencies
This plugin depends on jQuery, so make sure it is loaded before the plugin is
loaded.


### Usage
First, initialize the plugin in the `dependencies` part of the reveal.js config:

```js
{ src: 'plugin/sampler.js' }
```

This assumes that you copied the `sampler.js` file to `plugin/sampler.js` in
your reveal.js tree, but you can pick whatever you want. Then, inside source
files, use the following syntax to delimit code samples:

```
some code here

sample(sample-name)
...
end-sample

more code here
```

`sampler.js` will parse the source file, and anything between the `sample(...)`
and the `end-sample` tags will be taken to be a code sample named `sample-name`.
Including that code sample in a slide will cause all the code between the two
special tags to be included in that slide. However, anything on the same line
as one of the special tags will not be taken as part of the sample, which
allows commenting the tags:

```c++
// sample(sample-name)
...
// end-sample
```

Multiple samples can appear in the same source file, as long as they have
different names. Finally, to include a code sample in a slide, use `<code>`
tags as follows:

```html
<code class='sample' sample='path/to/source#sample-name'></code>
```

The plugin will take the sample named `sample-name` in the source file whose
path is given, and write it inside the `<code>` tag. It will also add the
`language-xxx` class to the `<code>` tag, where `xxx` is the extension of
the source file, so that code highlighting triggers properly if set up. This
usually works out of the box, because [highlight.js][] can recognize the
extensions associated to most languages.

You can find an example of using the `sampler.js` plugin in the `example/`
directory.


### License
`sampler.js` is placed in the public domain.


<!-- Links -->
[highlight.js]: https://highlightjs.org
[reveal.js]: https://github.com/hakimel/reveal.js/
