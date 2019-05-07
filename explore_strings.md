The links are given to the python tutor.  
Use them to solve and explore these three problems.

First, fix the code, to make them find the length of the string.

[One](http://www.pythontutor.com/c.html#code=int%20len_of_name%28char%20name%5B%5D%29%3B%0A%0Aint%20main%28%29%20%7B%0A%20%20char%20name%5B10%5D%20%3D%20%22Moon%22%3B%0A%20%20int%20name_len%20%3D%20len_of_name%28name%29%3B%0A%20%20printf%28%22The%20length%20of%20%25s%20is%20%25d.%5Cn%22,%20name,%20name_len%29%3B%0A%20%20return%200%3B%0A%7D%0A%0Aint%20len_of_name%28char%20name%5B%5D%29%20%7B%0A%20%20int%20len%20%3D%200%3B%0A%20%20for%28int%20i%20%3D%200%3B%20name%5Bi%5D%20!%3D%20'%20'%3B%20i%2B%2B%29%20%7B%0A%20%20%20%20printf%28%22%25c%22,%20name%5Bi%5D%29%3B%0A%20%20%20%20len%20%3D%20len%20%2B%201%3B%0A%20%20%7D%0A%20%20return%20len%3B%0A%7D&curInstr=36&mode=display&origin=opt-frontend.js&py=c&rawInputLstJSON=%5B%5D)


Sample code:

```
int len_of_name(char name[]);

int main() {
  char name[10] = "Moon";
  int name_len = len_of_name(name);
  printf("The length of %s is %d.\n", name, name_len);
  return 0;
}

int len_of_name(char name[]) {
  int len = 0;
  for(int i = 0; name[i] != ' '; i++) {
    printf("%c", name[i]);
    len = len + 1;
  }
  return len;
}
```

Second, fill the one line in the program to make it work.

[Two](http://www.pythontutor.com/c.html#code=void%20print_till_that_pos%28char%20*str,%20int%20pos%29%3B%0A%0Aint%20main%28%29%20%7B%0A%20%20char%20str%5B%5D%20%3D%20%22one%20two%20three%22%3B%0A%20%20print_till_that_pos%28str,%2011%29%3B%0A%20%20print_till_that_pos%28str,%207%29%3B%0A%20%20print_till_that_pos%28str,%203%29%3B%0A%20%20return%200%3B%0A%7D%0A%0A%0Avoid%20print_till_that_pos%28char%20*str,%20int%20pos%29%20%7B%0A%20%20%0A%20%20//%20write%20one%20statement%20bellow%20in%20Line-15%20to%20make%20this%20code%20work%0A%20%20%0A%20%20printf%28%22%25s%5Cn%22,%20str%29%3B%0A%7D&curInstr=0&mode=display&origin=opt-frontend.js&py=c&rawInputLstJSON=%5B%5D)


Sample code:

```
void print_till_that_pos(char *str, int pos);

int main() {
  char str[] = "one two three";
  print_till_that_pos(str, 11);
  print_till_that_pos(str, 7);
  print_till_that_pos(str, 3);
  return 0;
}


void print_till_that_pos(char *str, int pos) {
  
  // write one statement bellow in Line-15 to make this code work

  printf("%s\n", str);
}
```

Third, explore what is happening
After exploring try with different strings like
"0012", "abxzABXZ0198"

[Three](http://www.pythontutor.com/c.html#code=int%20convert_to_int%28char%20*str,%20int%20numbers%5B%5D%29%3B%0Avoid%20print_array%28int%20*a,%20int%20len%29%3B%0A%0Aint%20main%28%29%20%7B%0A%20%20int%20numbers%5B10%5D%3B%0A%20%20%0A%20%20int%20len%20%3D%200%3B%0A%20%20%0A%20%20char%20str1%5B%5D%20%3D%20%22abc%22%3B%0A%20%20len%20%3D%20convert_to_int%28str1,%20numbers%29%3B%0A%20%20printf%28%22%5C%22%25s%5C%22%20%3D%3E%20%22,%20str1%29%3B%0A%20%20print_array%28numbers,%20len%29%3B%0A%20%20%0A%20%20char%20str2%5B%5D%20%3D%20%22AXYZ%22%3B%0A%20%20len%20%3D%20convert_to_int%28str2,%20numbers%29%3B%0A%20%20printf%28%22%5C%22%25s%5C%22%20%3D%3E%20%22,%20str2%29%3B%0A%20%20print_array%28numbers,%20len%29%3B%0A%20%20%0A%20%20char%20str3%5B%5D%20%3D%20%22369%22%3B%0A%20%20len%20%3D%20convert_to_int%28str3,%20numbers%29%3B%0A%20%20printf%28%22%5C%22%25s%5C%22%20%3D%3E%20%22,%20str3%29%3B%0A%20%20print_array%28numbers,%20len%29%3B%0A%20%20%0A%20%20char%20str4%5B%5D%20%3D%20%22Aditya%20369%22%3B%0A%20%20len%20%3D%20convert_to_int%28str4,%20numbers%29%3B%0A%20%20printf%28%22%5C%22%25s%5C%22%20%3D%3E%20%22,%20str4%29%3B%0A%20%20print_array%28numbers,%20len%29%3B%0A%20%20%0A%20%20return%200%3B%0A%7D%0A%0A%0Aint%20convert_to_int%28char%20*str,%20int%20numbers%5B%5D%29%20%7B%0A%20%20int%20i%20%3D%200%3B%0A%20%20while%28*str%20!%3D%20'%5C0'%29%20%7B%0A%20%20%20%20*numbers%20%3D%20*str%3B%0A%20%20%20%20i%20%3D%20i%2B1%3B%0A%20%20%20%20numbers%20%3D%20numbers%20%2B%201%3B%0A%20%20%20%20str%20%3D%20str%20%2B%201%3B%0A%20%20%7D%0A%20%20return%20i%3B%0A%7D%0A%0Avoid%20print_array%28int%20*a,%20int%20len%29%20%7B%0A%20%20printf%28%22%5B%20%22%29%3B%0A%20%20for%28int%20i%20%3D%200%3B%20i%20%3C%20len-1%3B%20i%2B%2B%29%20%7B%0A%20%20%20%20printf%28%22%25d,%20%22,%20*a%29%3B%0A%20%20%20%20a%20%3D%20a%20%2B%201%3B%0A%20%20%7D%0A%20%20printf%28%22%25d%20%5D%5Cn%22,%20*a%29%3B%0A%7D&curInstr=0&mode=display&origin=opt-frontend.js&py=c&rawInputLstJSON=%5B%5D)

Sample code

```
int convert_to_int(char *str, int numbers[]);
void print_array(int *a, int len);

int main() {
  int numbers[10];
  
  int len = 0;
  
  char str1[] = "abc";
  len = convert_to_int(str1, numbers);
  printf("\"%s\" => ", str1);
  print_array(numbers, len);
  
  char str2[] = "AXYZ";
  len = convert_to_int(str2, numbers);
  printf("\"%s\" => ", str2);
  print_array(numbers, len);
  
  char str3[] = "369";
  len = convert_to_int(str3, numbers);
  printf("\"%s\" => ", str3);
  print_array(numbers, len);
  
  char str4[] = "aditya 369";
  len = convert_to_int(str4, numbers);
  printf("\"%s\" => ", str4);
  print_array(numbers, len);
  
  return 0;
}


int convert_to_int(char *str, int numbers[]) {
  int i = 0;
  while(*str != '\0') {
    *numbers = *str;
    i = i+1;
    numbers = numbers + 1;
    str = str + 1;
  }
  return i;
}

void print_array(int *a, int len) {
  printf("[ ");
  for(int i = 0; i < len-1; i++) {
    printf("%d, ", *a);
    a = a + 1;
  }
  printf("%d ]\n", *a);
}
```