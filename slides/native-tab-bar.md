##  Native Tab Bar

Set in `config/application.coffee`

    steroids.config.tabBar.enabled = true
    steroids.config.tabBar.tabs = [
      {
        title: "Gallery"
        icon: "icons/photos@2x.png"
        location: "http://localhost/views/photo_gallery/index.html"
      },
      {
        title: "Feed"
        icon: "icons/feed@2x.png"
        location: "http://localhost/views/photo_gallery/feed.html"
      }
    ]

Note:
