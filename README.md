# Kalkulator-sederhana

// Online C compiler to run C program online
#include <stdio.h>

int main() {
   float num1, num2, result;
    int choice;
    
    printf("Masukkan dua angka:\n");
    scanf("%f %f", &num1, &num2);
    
    
    printf("Kalkulator Sederhana\n");
    printf("Pilih operasi yang diinginkan:\n");
    printf("1 untuk Penjumlahan (+)\n");
    printf("2 untuk Pengurangan (-)\n");
    printf("3 untuk Perkalian (*)\n");
    printf("4 untuk Pembagian (/)\n");
    printf("Masukkan pilihan (1/2/3/4): ");
    scanf("%d", &choice);

    

    
    switch (choice) {
        case 1:
            result = num1 + num2;
            printf("Hasil Penjumlahan: %.2f\n", result);
            break;
        case 2:
            result = num1 - num2;
            printf("Hasil Pengurangan: %.2f\n", result);
            break;
        case 3:
            result = num1 * num2;
            printf("Hasil Perkalian: %.2f\n", result);
            break;
        case 4:
            
            if (num2 == 0) {
                printf("Error: Pembagian dengan nol tidak diperbolehkan.\n");
            } else {
                result = num1 / num2;
                printf("Hasil Pembagian: %.2f\n", result);
            }
            break;
        default:
            printf("Pilihan tidak valid. Silakan pilih antara 1, 2, 3, atau 4.\n");
            break;
    }

   

    return 0;
}
