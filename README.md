# Punto-5.104
Further Analysis
Load and run the script fi le, fn_z of Example 5.17.
XY=linspace(-3,3,19);

YX=linspace(-3,9,21);

[x,y]=meshgrid(XY,YX);

z=16*x.^4+15*x.^2-x+6-2*y.*x.^2+15*y.^2-y;

figure(1);

mesh(x,y,z);

box on; axis on;

xlabel(‘x-axis’);ylabel(‘y-axis’);zlabel(‘z-axis’)

title(‘Plot using mesh’)

figure(2)

meshc(x,y,z)

box on; axis on;

xlabel(‘x-axis’);ylabel(‘y-axis’);zlabel(‘z-axis’)

title(‘Plot using meshc’)

figure(3)

meshz(x,y,z)

box on; axis on;

xlabel(‘x-axis’);ylabel(‘y-axis’);zlabel(‘z-axis’)

title(‘Plot using meshz’)

figure(4);

surf(x,y,z);

box on; axis on;

xlabel(‘x-axis’);

ylabel(‘y-axis’);zlabel(‘z-axis’)

title(‘Plot using surf’)

figure(5)

surfc(x,y,z)

box on; axis on;

xlabel(‘x-axis’);ylabel(‘y-axis’);zlabel(‘z-axis’)

title(‘Plot using surfc ‘)

figure(6)

waterfall(x,y,z)

box on; axis on;

xlabel(‘x-axis’);ylabel(‘y-axis’);zlabel(‘z-axis’)

title(‘Plot using waterfall’)
