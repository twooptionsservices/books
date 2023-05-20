
<html>
<head><meta charset="utf 1">
<title>2OPTIONS SERVICES</title>
<style>
body {
background-color: black;
margin: 10%;
font-family: san-serif;}
h1 {
text-align: center;
font-family: serif;
font-weight: normal;
font-transform: uppercase;
color: white;}
h2 {color: white;}
p { color: white;}
</style>
<script src="https://mozilla.github.io/pdf.js/build/pdf.js"></script>
<div id="pdfContainer"></div>
<script> 
  const url = 'path/to/your/file.pdf';
  pdfjsLib.getDocument(url).promise.then(pdf => {
    pdf.getPage(1).then(page => { 
      const canvas = document.createElement('canvas');
      const context = canvas.getContext('2d');
      canvas.width = 600;
      canvas.height = 800;
      const viewport = page.getViewport({ scale: 1 });
      const renderContext = {
        canvasContext: context,
        viewport: viewport
      };
      page.render(renderContext).promise.then(() => {
       
        const container = document.getElementById('pdfContainer');
        container.appendChild(canvas);
      });
    });
  });
</script>
</head>
<body>
<h1>2OPTIONS SERVICES</h1>
<h2>FOREX TRADING COMPLETE COURSE</h2>
<iframe src="FOREX_TRADING_COMPLETE_COURSE_STUDY-_FOR.pdf" width="100%" height="600px"></iframe>
<p>If you are a beginner in retail trading and you want a quick start, this ebook can help you.</p>


</body>
</html>
