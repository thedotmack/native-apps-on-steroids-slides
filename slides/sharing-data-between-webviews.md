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
The way shared data works, is that we're going to use the HTML5 postmessage API. We're going to send the message in one webview while listening for that message in our target webview.