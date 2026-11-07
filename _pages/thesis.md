---
layout: page
permalink: /thesis/
title: The Effect of Class Imbalance on Causal Effect Estimation
description: Senior honors thesis, Williams College, May 2026. Advised by Prof. Rohit Bhattacharya.
nav: false
---

<p><a href="/assets/pdf/Abel_Mesfin_Thesis.pdf" download>Download PDF</a></p>

<div id="thesis-viewer" style="width:100%">
  <p id="thesis-loading">Loading thesis…</p>
</div>

<script src="https://cdnjs.cloudflare.com/ajax/libs/pdf.js/3.11.174/pdf.min.js"></script>
<script>
  (function () {
    var viewer = document.getElementById("thesis-viewer");
    var loading = document.getElementById("thesis-loading");
    pdfjsLib.GlobalWorkerOptions.workerSrc =
      "https://cdnjs.cloudflare.com/ajax/libs/pdf.js/3.11.174/pdf.worker.min.js";
    pdfjsLib.getDocument("/assets/pdf/Abel_Mesfin_Thesis.pdf").promise.then(function (pdf) {
      loading.remove();
      var chain = Promise.resolve();
      for (var i = 1; i <= pdf.numPages; i++) {
        (function (n) {
          chain = chain.then(function () {
            return pdf.getPage(n).then(function (page) {
              var ratio = window.devicePixelRatio || 1;
              var scale = (viewer.clientWidth / page.getViewport({ scale: 1 }).width) * ratio;
              var vp = page.getViewport({ scale: scale });
              var canvas = document.createElement("canvas");
              canvas.width = vp.width;
              canvas.height = vp.height;
              canvas.style.width = "100%";
              canvas.style.display = "block";
              canvas.style.marginBottom = "16px";
              canvas.style.boxShadow = "0 1px 4px rgba(0,0,0,.2)";
              viewer.appendChild(canvas);
              return page.render({ canvasContext: canvas.getContext("2d"), viewport: vp }).promise;
            });
          });
        })(i);
      }
    }).catch(function () {
      loading.innerHTML = 'Could not load the viewer. <a href="/assets/pdf/Abel_Mesfin_Thesis.pdf">Open the PDF directly</a>.';
    });
  })();
</script>
