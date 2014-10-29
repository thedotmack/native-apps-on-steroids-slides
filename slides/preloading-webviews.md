##  Preloading WebViews

In `app/controllers/photo_gallery.js`

    var singleView = new steroids.views.WebView({
        location:   "/views/photo_gallery/single.html",
        id:         "singleView"
    });
    singleView.preload();

Note:
This is so the WebView exists for the data we're about to pass it.