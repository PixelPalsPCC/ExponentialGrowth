float population = 1; // Initial population
float population2 = 1; // Initial population
float population3 = 1; // Initial population
float population4 = 1; // Initial population
float population5 = 1; // Initial population
float growthRate = 0.1; // Growth rate
float growthRate2 = 0.08; // Growth rate
float growthRate3 = 0.075; // Growth rate
float growthRate4 = 0.06; // Growth rate
float growthRate5 = 0.05; // Growth rate

void setup() {
  size(400, 400);
  background(255);
  textSize(16);
}

void draw() {
  background(255);
  fill(0);
  text("Population: " + int(population), 20, 20);

  text("Population2: " + int(population2), 20, 50);

  text("Population3: " + int(population3), 20, 80);

  text("Population4: " + int(population4), 20, 110);

  text("Population5: " + int(population5), 20, 140);

  // Exponential growth formula
  population *= 1 + growthRate;
  population2 *= 1 + growthRate2;
  population3 *= 1 + growthRate3;
  population4 *= 1 + growthRate4;
  population5 *= 1 + growthRate5;

  // Draw a rectangle representing the population size
  float rectHeight = map(population, 1, 10000, 10, height - 50);
  float rectHeight2 = map(population2, 1, 10000, 10, height - 50);
  float rectHeight3 = map(population3, 1, 10000, 10, height - 50);
  float rectHeight4 = map(population4, 1, 10000, 10, height - 50);
  float rectHeight5 = map(population5, 1, 10000, 10, height - 50);
  rect(width / 2, height - 20, 10, -rectHeight);
  rect(width / 2+20, height - 20, 10, -rectHeight2);
  rect(width / 2+40, height - 20, 10, -rectHeight3);
  rect(width / 2+60, height - 20, 10, -rectHeight4);
  rect(width / 2+80, height - 20, 10, -rectHeight5);
  
  // Add a condition to stop the growth for visualization purposes
  if (population > 10000) {
    noLoop(); // Stop the draw loop
  }
}
