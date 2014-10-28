####  Accessing hardware with Cordova APIs <!-- .element: class="bold" -->

    function getAcceleration() {
      navigator.accelerometer.getCurrentAcceleration(
      accelerometerOnSuccess, accelerometerOnError)
    }

    function accelerometerOnSuccess(acceleration) {
      acceleration_data.innerHTML =
        "x: " + acceleration.x + "<br>" +
        "y: " + acceleration.y + "<br>" +
        "z: " + acceleration.z + "<br>" +
        "timestamp: " + acceleration.timestamp
    }

    function accelerometerOnError(error) {
      alert("Accelerometer error: " + JSON.stringify(error));
    }

<small>http://docs.appgyver.com/en/stable/index.html</small>