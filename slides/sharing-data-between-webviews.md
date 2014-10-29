###  Sharing Data between WebViews <!-- .element: class="bold" -->

In `app/controllers/photo_gallery.js`

    $('#thumbnails img').on('click',function(){
        message = {
            recipient:  'singleView',
            src:        $(this).attr('src'),
            title:      $(this).attr('alt')
        }
        window.postMessage(message);
        steroids.layers.push(singleView);
    });

Note:
- Uses the HTML5 postmessage API. 
- send the message in one webview
- listening for that message in our target webview