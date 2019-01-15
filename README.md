### hopscotch
---
https://github.com/linkedin/hopscotch

```js
var tour = {
  id: "hello-hpscotch",
  steps: [
    {
      title: "My Header",
      content: "This is the header of my page.",
      target: "header",
      placement: "right"
    },
    {
      title: "My content",
      content: "Here is where I put my content.",
      target: document.querySelector("#content p"),
      placement: "bottom"
    }
  ]
};
hopscotch.startTour(tour);

var tour = {
  id: 'myTour',
  steps: [
    {
      target: 'firststep',
      placement: 'bottom',
      title: 'My First Step',
      onNext: function(){
        $('#firststep').hide();
      }
    }
  ],
  onStart: function(){
    $('#article').addClas('selected');
  }
};

hopscotch.registerHelper('selectArticle', function(){
  $('#article').addClass('selected');
});

hopscotch.registerHelper('fillText', function(textFieldId, textStr){
  document.getElementById(textFieldId).value = textStr;
});

var calloutMgs = hopscotch.getCalloutManager();
calloutMgr.createCallout({
  id: 'attach-icon',
  target: 'attach-btn',
  placement: 'bottom',
  title: 'Now you can share images &amp; files!',
  content: 'Share a project you\'re proud of, a photo from a recent event, or an interesting presentation.'
});
```

```
```

```
```

