---
tags: [ "eclipse" , "che" ]
title: Editing Files
excerpt: ""
layout: docs
permalink: /:categories/build-run/
---
{% include base.html %}

#### cURL : Create a new file

```shell  
curl -X POST -d 'var i = 1;' http://localhost:8080/api/ext/project/workspacesq6co30qcxi1kqsj/file/my-first-sample?name=newfile.js
```

#### cURL : Editing an existing file

```shell  
curl -X PUT -d $'var i = 1;\nvar test = "hello Eclipse Che";' http://localhost:8080/api/ext/project/workspacesq6co30qcxi1kqsj/file/my-first-sample/newfile.js
```

#### cURL : Deleting an existing file

```shell  
curl -X DELETE http://localhost:8080/api/ext/project/workspacex4zl7nvex1yldosj/my-first-sample/newfile.js
```
