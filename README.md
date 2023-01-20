# screenshot-of-div-using-javascript

You can get screenshot of div using DOM Element using Javascript



domtoimage.toPng(imageCaptures)
    .then(function(dataUrl) {
    console.log(dataUrl);
      //window.open(dataUrl);
      var img = new Image();
      img.src = dataUrl;
      document.getElementById("capture-theimages").appendChild(img);
    })
    .catch(function(error) {
      console.error('oops, something went wrong!', error);
    });
