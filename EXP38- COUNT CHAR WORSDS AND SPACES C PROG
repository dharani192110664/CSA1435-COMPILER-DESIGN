#include <stdio.h>

int main() {
  char text[1000];
  int words = 0, characters = 0, lines = 0;

  printf("Enter the text: ");
  scanf("%[^\n]", text);


  for (int i = 0; text[i] != '\0'; i++) {
    if (text[i] == ' ' || text[i] == '\t' || text[i] == '\n') {
      words++;
    }
  }

 
  for (int i = 0; text[i] != '\0'; i++) {
    characters++;
  }

  
  for (int i = 0; text[i] != '\0'; i++) {
    if (text[i] == '\n') {
      lines++;
    }
  }

  printf("Number of words: %d\n", words);
  printf("Number of characters: %d\n", characters);
  printf("Number of lines: %d\n", lines);

  return 0;
}
