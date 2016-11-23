# -
Калькулятор для квадратных уравнений.
program kvadratnoe_uravnenie;
var a, b, c, D, x, x1, x2, z: real;
begin 
writeln('Ввели коэффициенты a, b и c для квадратного уравнения вида (ax^2+bx+c=0) :');
write('a= ');
read (a);
write('b= ');
read (b);
write('c= ');
read (c);
writeln('Решение:');
D:=b*b-4*a*c;
if D<0 then
  
  begin
  z:=-4*a*c;
     if z<0 then
     
     begin
     writeln( );
     writeln('Нет корней,т.к. дискриминант меньше 0');
     writeln( );
     writeln(a,'x^2+',b,'x+',c,'=0');
     writeln( );
     writeln('D=',b,'^2-4*',a,'*',c);
     writeln('D=',b*b,z);
     writeln('D=',D);
     writeln('D<0');
     end
     
     else
     
     begin
     writeln( );
     writeln('Нет корней,т.к. дискриминант меньше 0');
     writeln( );
     writeln(a,'x^2+',b,'x+',c,'=0');
     writeln( );
     writeln('D=',b,'^2-4*',a,'*',c);
     writeln('D=',b*b,'+',z);
     writeln('D=',D);
     writeln('D<0');
     end
     
  end
  
  else
   if D=0 then 
    
    begin
    x:=(-b)/2*a;
    z:=-4*a*c;
    if z<0 then
    
       begin
       writeln( );
       writeln('Есть лишь один корень');
       writeln( );
       writeln(a,'x^2+',b,'x+',c,'=0');
       writeln( );
       writeln('D=',b,'^2-4*',a,'*',c);
       writeln('D=',b*b,z);
       writeln('D=',D);
       writeln( );
       writeln('x=',-b,'/',2*a);
       end
       
       else
       
       begin
       writeln( );
       writeln('Есть лишь один корень');
       writeln( );
       writeln(a,'x^2+',b,'x+',c,'=0');
       writeln( );
       writeln('D=',b,'^2-4*',a,'*',c);
       writeln('D=',b*b,'+',z);
       writeln('D=',D);
       writeln( );
       writeln('x=',-b,'/',2*a);
       end
       
    end
    
   else
    
    begin
    x1:=(-b-sqrt(D))/2*a;
    x2:=(-b+sqrt(D))/2*a;
    z:=-4*a*c;
    if z<0 then
    
       begin
       writeln( );
       writeln('Есть два корня');
       writeln( );
       writeln(a,'x^2+',b,'x+',c,'=0');
       writeln( );
       writeln('D=',b,'^2-4*',a,'*',c);
       writeln('D=',b*b,z);
       writeln('D=',D);
       writeln( );
       writeln('x1=',-b,'-',sqrt(D),'/',2*a);
       writeln('x2=',-b,'+',sqrt(D),'/',2*a);
       writeln( );
       writeln('x1=',x1);
       writeln('x2=',x2);
       end
       
       else
       
       begin
       writeln( );
       writeln('Есть два корня');
       writeln( );
       writeln(a,'x^2+',b,'x+',c,'=0');
       writeln( );
       writeln('D=',b,'^2-4*',a,'*',c);
       writeln('D=',b*b,'+',z);
       writeln('D=',D);
       writeln( );
       writeln('x1=',-b,'-',sqrt(D),'/',2*a);
       writeln('x2=',-b,'+',sqrt(D),'/',2*a);
       writeln( );
       writeln('x1=',x1);
       writeln('x2=',x2);
       end
       
    end
    
end.
