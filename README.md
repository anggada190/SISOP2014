# SISOP2014
sisop adalah perjuangan
/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */
package kudadansiput;

/**
 *
 * @author Kira S
 */
class HewanTest {

public static void main(String[] args) {

Hewan seekorKuda  = new Kuda(); Hewan seekorSiput = new Siput();

double waktuTempuh = 1.5;

System.out.println("Setelah berjalan selama "
+ waktuTempuh + " jam:");
System.out.printf("%s telah menempuh jarak sejauh %.2f km\n", seekorKuda.getClass().getSimpleName(), seekorKuda.berjalan(waktuTempuh));
System.out.printf("%s telah menempuh jarak sejauh %.2f km\n", seekorSiput.getClass().getSimpleName(), seekorSiput.berjalan(waktuTempuh));
    }
    
}
interface Hewan {


double berjalan(double jam);
}
class Kuda implements Hewan {

public double berjalan(double jam) {
// Kecepatan kuda berjalan adalah sekitar 88 km/jam
// (http://www.speedofanimals.com/animals/horse)
return 88 * jam;
}
}
class Siput implements Hewan {

public double berjalan(double jam) {
// Kecepatan siput berjalan adalah sekitar 0.1 km/jam
// (http://www.speedofanimals.com/animals/garden_snail)
return 0.1 * jam;
}
}
