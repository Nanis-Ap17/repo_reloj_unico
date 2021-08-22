# repo_reloj_unico
void setup() {
size(400, 400);
stroke(255);
}
void draw() {
background(0);
fill(#000000);
stroke(#F6FF05);
ellipse(200, 200, 300, 300);
float o = map(second(), 0, 60, 0, TWO_PI) - HALF_PI;
stroke(#FF1CE9);
strokeWeight(4);
line(200, 200, cos(o) * 140 + 200, sin(o) * 140 + 200);
saveFrame("frames/####.tif");
}
