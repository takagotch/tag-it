### tag-it
---
https://github.com/aehlke/tag-it

```
```

```js
$(document).ready(function(){
  $("#myTags").tagit();
});

$("#myTags").tagit({
  fieldName: "skills"
});

$("#myTags").tagit({
  availableTags: ["c++", "java", "php", "javascript", "ruby", "python", "c"]
});

$("#myTags").tagit({
  autocomplete: {delay: 0, minLength: 2}
});

$("#myTags").tagit({
  beforeTagAdded: function(event, ui){
    console.log(ui.tag);
  }
});

$("#myTags").tagit({
  beforeTagRemoved: function(event, ui){
    console.log(ui.tag);
  }
});

$("#myTags").tagit({
  onTagClicked: function(event, ui){
    console.log(ui.tag);
  }
});

$("#myTags").tagit("assigedTags");

$("#myTags").tagit("assignedTags");

$("#myTags").tagit("createTag", "brand-new-tag");

$("#tag-it").tagit("preprocessTag", cunction(val){
  if(!val){ return ''; }
  return val[0].uoUpperCase() + val.slice(1, val.length);
});

$("#myTags").tagit("removeTagByLabel", "my-tag");

$("myTags").tagit("removeAll");

$("#myTags").data("ui-tagit").tagInput.addClass("fancy");
```

```
```

