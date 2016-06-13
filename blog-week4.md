##How to save an input from a form in jQuery and display it on the screeeeen

First. Hop up into your html! Create your self a little form. How many inputs you want
2? 3? Lets say three. Maybe something like this?

`<form class="inputTitle">
  <input class="newLinkTitle" type="text" name="linkTitle" placeholder="Title"></input></form>
<form class="inputUrl">
  <input class="newLinkUrl" type="text" name="linkUrl" placeholder="URL"></input></form>
<form class="inputDecription">
    <input class="newLinkDescription" type="text" name="linkDescription" placeholder="Description"></input></form>
  <form class="userShare">`

  Yeah. Dat's nice. Ok now hop over to jQuery!
  Cool now we gotta capture the values of those there inputs. Maybe something like this?

     `var link = {
          "title": $('input[name="linkTitle"]').val(),
          "url": $('input[name="linkUrl"]').val(),
          "description": $('input[name="linkDescription"]').val()`

Oh dang! That looks fancy! Now lets show it on the screen! use something like this?


`
$(".whereIWantMyStuffToGo").append(<li> + link.title +
                                          link.url +
                                          link.description);`

Look at you aren't you fancy!
