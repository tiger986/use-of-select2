## How to Use Select2 Plug-in
#### code
```javascript
$("#uploader").select2({
    placeholder : '请选择发布者',
    ajax: {
        url: 'http://zj.primecloud.cn/teacherCourse/getBookCourse',
        type: 'get',
        dataType: 'json',
        processResults: function (data) {
            return {results: data.data};
        }
    }
});
