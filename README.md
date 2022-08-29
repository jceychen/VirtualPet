void setup() {
  size(510, 400);
  background(230, 230, 210);
  noStroke();
  fill(210, 220, 200);
  rect(0, 0, 30, 400);
  rect(60, 0, 30, 400);
  rect(120, 0, 30, 400);
  rect(180, 0, 30, 400);
  rect(240, 0, 30, 400);
  rect(300, 0, 30, 400);
  rect(360, 0, 30, 400);
  rect(420, 0, 30, 400); 
  rect(480, 0, 30, 400);
  stroke(150, 121, 105);
  strokeWeight(86);
  line(510, 400, 0, 400);
}

void draw() {
  var x = 255;
  var y = 255;
  var faceSize = 150;
  
  strokeWeight(3);
  stroke(113, 121, 126);
  
  fill(169, 169, 169);
  ellipse(x - 60, y - 40, faceSize/2, faceSize/2); //left ear
  ellipse(x + 60, y - 40, faceSize/2, faceSize/2); //right ear
  fill(113, 121, 126);
  ellipse(x - 60, y - 41, faceSize/4, faceSize/4); //inner left ear
  ellipse(x + 60, y - 41, faceSize/4, faceSize/4); //inner right ear
  
  fill(169, 169, 169);
  ellipse(x, y + 70, faceSize - 80, faceSize - 80); //body
  ellipse(x - 40, y + 80, faceSize - 100, faceSize - 30); //left paw
  ellipse(x + 40, y + 80, faceSize - 100, faceSize - 30); //right paw
  ellipse(x, y, faceSize, faceSize - 10); //face
  
  fill(113, 121, 126);
  ellipse(x, y + 30, faceSize/5, (faceSize/5) + 5); //nose
  ellipse(x - 30, y + 20, faceSize/8, faceSize/8); //left eye
  ellipse(x + 30, y + 20, faceSize/8, faceSize/8); //right eye
  noFill();
  arc(x, y + 21, 100, 100, QUARTER_PI, QUARTER_PI);
  
  fill(255, 255, 255);
  noStroke();
  ellipse(x - 31, y + 19, faceSize/16, faceSize/16); //inner left eye
  ellipse(x + 29, y + 19, faceSize/16, faceSize/16); //inner right eye
  ellipse(x - 170, y - 160, 120, 100); //middle cloud chunk 1
  ellipse(x - 230, y - 160, 90, 60); //left cloud chunk 2
  ellipse(x - 100, y - 160, 90, 60); //right cloud chunk 3
  ellipse(x + 190, y - 120, 120, 100); //middle cloud chunk 2
  ellipse(x + 240, y - 120, 90, 60); //left cloud chunk 2
  ellipse(x + 110, y - 120, 90, 60); //right cloud chunk 2
}
