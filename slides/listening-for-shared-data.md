###  Listening for Shared Data in Your Target WebView <!-- .element: class="bold" -->

In `app/views/photo_gallery/single.html`

    function messageReceived(event) {
        // check that the message is intended for us
        if (event.data.recipient == "singleView") {
            $('#single .card').html(
                '<img src="' + event.data.src + 
                '"><h3>' + event.data.title + '</h3>'
            );
        }
    }
    window.addEventListener("message", messageReceived);
