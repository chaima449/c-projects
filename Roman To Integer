/*# c-projects
c projects
Roman to integer:
*/
#include<stdio.h>
#include<stdlib.h>
#include<string.h>

int romanToInt(char *s){
    int sum = 0;
    int i =0;
    int len;
    len = strlen(s);
    //printf("%d", len);
    while(i < len){//(s[i] != 0){
        if(s[i] == 'I'){
            if(s[i+1] == 'V'){
                sum += 4;
                i += 2;
            }
            else if(s[i+1] == 'X'){
                sum += 9;
                i += 2;
            }
            else{
                sum += 1;
                i++;
            }
        }
        else if(s[i] == 'V'){
            sum += 5;
            i++;
        }
        else if(s[i] == 'X'){
            if(s[i+1] == 'L'){
                sum += 40;
                i += 2;
            }
            else if(s[i+1] == 'C'){
                sum += 90;
                i += 2;
            }
            else{
                sum += 10;
                i++;
            }
        }
        else if(s[i] == 'L'){
            sum += 50;
            i++;
        }
        else if(s[i] == 'C'){
            if(s[i+1] == 'D'){
                sum += 400;
                i += 2;
            }
            else if(s[i+1] == 'M'){
                sum += 900;
                i += 2;
            }
            else{
                sum += 100;
                i++;
            }
        }
        else if(s[i] == 'D'){
            sum += 500;
            i++;
        }
        else if(s[i] == 'M'){
            sum += 1000;
            i++;
        }
    }
    return sum;
}

int main(){
    int result;
    result = romanToInt("MCMXCIV");
    //printf("hello");
    printf("%d", result);
}
