%{
  #include <stdio.h>
  char* numbers[100];
  int num_count = 0;
  char* words[100]; 
  int word_count = 0;
%}

%%
[0-9]+ {numbers[num_count++] = yytext;
}
[a-zA-Z]+ {
  words[word_count++] = yytext;
}
printf("%s",yytext);
. {
  printf("Error: unexpected character '%c'\n", yytext[0]);
}
%%
int yywrap(){}

int main() {
  printf("enter the input");
  yylex();
  printf("Numbers:\n");
  for (int i = 0; i < num_count; i++) {
    printf("%s\n", numbers[i]);
  }
  printf("Words:\n");
  for (int i = 0; i < word_count; i++) {
    printf("%s\n", words[i]);
  }
  return 0;
}
