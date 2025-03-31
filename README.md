#define _CRT_SECURE_NO_WARNINGS
#include <stdio.h>
#include <string.h>
#include <time.h>

int main() {
    int score[10];
    int sum = 0;
    float average;
    int i;

    printf("10명의학생 성적평균 구하기\n");
    for (i = 0; i < 10; i++) {
        printf("학생 %d: ", i + 1);
        scanf("%d", &score[i]);
        sum += score[i];
    }
    average = sum / 10.0;
    printf("10명 학생의 평균 성적 : % 2f\n", average);
    return 0;
}
