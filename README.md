# Ejercicio-4
Correlación-Horas viendo series vs. Horas viendo cine


String monate[]={"enero", "febrero","marzo", "abril", "mayo", "junio", "julio", "agosto", "septiembre","octubre", "noviembre", "diciembre"};
  int horas[]= {40, 30, 12, 35, 16, 24, 14, 3, 0, 0, 0, 0};
int cine[]= {6, 4, 0, 2, 6, 8, 4, 0, 0, 0, 0, 0};


PFont gluck; 

void setup(){
 size(1080,720);
 gluck= loadFont("Cambria-30.vlw");
 textFont(gluck,20);
}

  void draw(){
    background(0);
    text("Horas series vs. cine",50, 50);
    text("Love Processing",500, 610);
    for(int equis=0; equis<12; equis= equis + 1){
      for(int otra=0; otra<12; otra= otra+1){
      
     text(monate[equis],50, 100 + (equis*50));
     fill(58,191,240);
    rect(200, 85 + (equis*50), horas[equis], 10);
    fill(255);
    text(horas[equis], 210+horas[equis], 96 +(equis*50) );
   
     fill(255,0,150);
    rect(200, 95 + (otra*50), cine[otra], 10);
    fill(255);
    text(cine[otra], 210+cine[otra], 110 +(otra*50) );
    
    
      }
    
    }
  }
  
  
