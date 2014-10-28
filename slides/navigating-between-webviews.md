##  Navigating in between WebViews

In `app/controllers/photo_gallery.js`

    $('#thumbnails img').on('click',function(){

        var webView = new steroids.views.WebView(
                          '/views/photo_gallery/single.html'
                      );
        
        steroids.layers.push(webView);

    });

