<!DOCTYPE html>
<html lang="en">
<head>
  <title>Lightning Selector Tool</title>
  <style>
    body {
      margin: 0;
      display: flex;
      flex-direction: column;
      align-items: center;
    }
    #lightningImage {
      max-width: 100%;
      height: auto;
      border: 1px solid #ccc;
      margin-top: 20px;
    }
    #selectionCanvas {
      position: absolute;
      top: 0;
      left: 0;
      pointer-events: none;
    }
    #finishSelection {
      margin-top: 10px;
      padding: 10px 20px;
      background-color: #4caf50;
      color: white;
      border: none;
      cursor: pointer;
      font-size: 16px;
    }
    #finishSelection:hover {
      background-color: #45a049;
    }
  </style>
</head>
<body>
  <!-- Lightning Image -->
  <div style="position: relative; display: inline-block;">
    <img id="lightningImage" src="https://media.discordapp.net/attachments/1263161954810335372/1277290134617980929/2.webp?ex=675da5a2&is=675c5422&hm=f8b9c5b5d47a6c133fe92e88353a089b5304e5e55f1428fd45b768f56135f400&=&format=webp" alt="Lightning">
    <canvas id="selectionCanvas"></canvas>
  </div>

  <!-- Finish Button -->
  <button id="finishSelection">Finish Selection</button>

  <script>
    const lightningImage = document.getElementById("lightningImage");
    const selectionCanvas = document.getElementById("selectionCanvas");
    const finishButton = document.getElementById("finishSelection");

    // Adjust canvas size to match the image
    lightningImage.onload = () => {
      selectionCanvas.width = lightningImage.width;
      selectionCanvas.height = lightningImage.height;
    };

    // Capture user clicks for selection
    const points = [];
    lightningImage.addEventListener("click", (event) => {
      const rect = lightningImage.getBoundingClientRect();
      const x = event.clientX - rect.left;
      const y = event.clientY - rect.top;
      points.push([x, y]);
      drawPoints(points);
    });

    // Draw points or a path on the canvas
    function drawPoints(points) {
      const ctx = selectionCanvas.getContext("2d");
      ctx.clearRect(0, 0, selectionCanvas.width, selectionCanvas.height);
      ctx.beginPath();
      points.forEach(([x, y], index) => {
        if (index === 0) {
          ctx.moveTo(x, y);
        } else {
          ctx.lineTo(x, y);
        }
      });
      ctx.strokeStyle = "yellow";
      ctx.lineWidth = 2;
      ctx.stroke();
    }

    // Send the selection points to Photopea
    finishButton.addEventListener("click", () => {
      window.parent.postMessage(
        `app.activeDocument.selection.select(${JSON.stringify(points)});`,
        "*"
      );
    });
  </script>
</body>
</html>
