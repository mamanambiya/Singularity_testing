# Singularity_testing
[![https://www.singularity-hub.org/static/img/hosted-singularity--hub-%23e32929.svg](https://www.singularity-hub.org/static/img/hosted-singularity--hub-%23e32929.svg)](https://singularity-hub.org/collections/1631)


```
var app = require('json-to-markdown');

var columns = [
    {key: a, label: 'custom title'},
    'b',
    'c'
];


var object = [
    {
        a: 'asdfa',
        b: [['239487','asdff'],['239487','asdff']],
        c: {c: 'asdf',g: ['239487','asdff']},
    },{
        d: 'efg',
        e: [],
        f: 'klm'
    },
    {
        a: 'sdf',
        b: 'gsdf',
        c: null
    }
];

var tableMdString = app(object, columns);

```
