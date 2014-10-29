###  Suggested File Structure

    your_project/
    └── app/
        ├── controllers/
        |   └── photo_gallery.js     
        ├── models/
        |   └── photo_gallery.js     
        └── views/
            ├── photo_gallery/
            |   ├── index.html
            |   ├── single.html
            |   └── feed.html
            └── layouts/
                └── photo_gallery.html

#### Steroids will take the `app` folder and compile it so you can keep DRY (Don't repeat yourself)

Note:
- Set up in a model / view / controller way
- Steroids builds these files for you