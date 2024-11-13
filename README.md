# Password-Compliance
The purpose of this program is to verify that a password entered by the user complies with the established guidelines. After asking the user to enter a password, it determines if it satisfies the requirements. The criteria include certain character requirements and the password's length. The password follows this format: L$$555ee
#include <stdio.h>
int main() {
char username[] = "moeageli"; // Mohammed Munir Ali Ageli
char password[10];
printf("Enter your password: ");
scanf("%s"
, password);
int length = 0;
while (password[length] != '\0') {
length++;
}
int mohammedageli = (length == 8 &&
(password[0] >= 'a' && password[0] <= 'z' || password[0] >= 'A' &&
password[0] <= 'Z') &&
password[1] == '$' && password[2] == '$' &&
password[3] >= '0' && password[3] <= '9' &&
password[4] >= '0' && password[4] <= '9' &&
password[5] >= '0' && password[5] <= '9' &&
(password[6] >= 'a' && password[6] <= 'z' && password[7] >= 'a' &&
password[7] <= 'z'));
if (mohammedageli) {
printf("Password complies with the specified rules.\n");
} else {
printf("Password does not comply with the specified rules.\n");
}
return 0;
}
