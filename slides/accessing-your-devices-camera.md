###  Accessing Your Device's Camera <!-- .element: class="bold" -->

    function getPicture() {
        navigator.camera.getPicture(onSuccess, onFail, {
            quality         : 50,
            destinationType : Camera.DestinationType.DATA_URL
        });
    }

    function onSuccess(imageData) {
        var image = document.getElementById('myImage');
        image.src = "data:image/jpeg;base64," + imageData;
    }

    function onFail(message) {
        alert('Failed because: ' + message);
    }

<small>http://docs.appgyver.com/en/stable/cordova_camera_camera.md.html</small>