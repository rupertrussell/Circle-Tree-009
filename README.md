# Circle-Tree-009
Added:
loadPixels();  //  Loads the pixel data of the current display window into the pixels[] array.
updatePixels(); // Updates the display window with the data in the pixels[] array. 

Removed Keypress and Mouseclick to save image and replaced with 
  if (Cells.size() > oldCellCount) {
    updatePixels();
    println("Cells.size() = " + Cells.size());
    oldCellCount = Cells.size();
    updatePixels(); // Updates the display window with the data in the pixels[] array. Otherwise the screen is blank when we save it
    save(filename + Cells.size() + ".png");
    println("*** saved " + filename + Cells.size());
  }
  
