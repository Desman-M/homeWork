# homeWork
dz
#include <iostream>
//#unclude <string>

// 4 написать программу, которая заполняет диагональные элементы квадратной матрицы единицами 

 int main(){
 constexpr int SZ = 10;
 unsigned char arr[SZ][SZ] = {0};

 for (int y = 0; y < SZ; y++){
  arr[y][y] = 1;              //координаты arr[0][0] = 1
  arr[y][SZ - (y + 1)] = 1;   //координаты arr[0][10-(0+1)] = 1
}
 for (int y = 0; y < SZ; y++){
    for(int x = 0; x < SZ; x++){
        printf("2d", arr[y][x]);
    }
   printf("\n");
}



return 0;
}
