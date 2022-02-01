#include <simplecpp>
main_program{
  initCanvas("Projectile motion", 500,500);
  Rectangle r(0,15,1000,80);
  r.setColor(COLOR("yellow"));
    r.setFill(true);
    Text t1(100,20,"Project By: Satyam Toraskar");
    Text t2(100,40,"Click anywhere on canvas");



  int start = getClick();

  Circle sp(start /65536, start % 65536, 5);
  sp.penDown();

  double vx=1,vy=-5;

  repeat(100){
    sp.move(vx,vy);
    vy += .1;
    wait(0);
  }

  Circle s1(start /65536, start % 65536, 5);
  s1.penDown();

    double qx=1,qy=-4;

  repeat(80){
    s1.move(qx,qy);
    qy += .1;
    wait(0);
  }

  Circle s2(start /65536, start % 65536, 5);
  s2.penDown();

    double wx=1,wy=-3;

  repeat(60){
    s2.move(wx,wy);
    wy += .1;
    wait(0);
  }

  Circle s3(start /65536, start % 65536, 5);
  s3.penDown();

    double ex=1,ey=-2;

  repeat(40){
    s3.move(ex,ey);
    ey += .1;
    wait(0);
  }

  Circle s4(start /65536, start % 65536, 5);
  s4.penDown();

    double rx=1,ry=-1;

  repeat(20){
    s4.move(rx,ry);
    ry += .1;
    wait(0);
  }

  Circle s5(start /65536, start % 65536, 5);
  s5.penDown();

    double tx=1,ty=0;

  repeat(100){
    s5.move(tx,ty);

    wait(0);
  }

  getClick();
}
