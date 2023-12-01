```dataviewjs
dv.paragraph("Semester Progress");

var a = moment("2023-11-20");
var b = moment("2024-01-01");

var n = moment();
var t = moment().startOf('day');

let q = b.diff(a, 'days');
let p = b.diff(t, 'days');
let r = t.diff(a, 'days');

let h = n.diff(a, 'hours');
let i = b.diff(a, 'hours');

let html = `<progress style="height:10px;width:80%" value="` + h + `" max="` + i + `"></progress>`;

if (r > 0 && r < q) {
    html += (h / i * 100).toFixed(2) + `%`;
}

dv.paragraph(html);
```
01. Chase Roll
02. 


