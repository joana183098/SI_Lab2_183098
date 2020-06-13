# Втора лабораториска вежба по Софтверско инженерство

## Јоана Трајанова, 183098

### Група на код: 

Ја добив групата на код 5

###  Control Flow Graph

https://prnt.sc/sz2z3z


### Тест случаи според критериумот  MCC
 if (i - 1 >= 0 && list.get(i – 1).equals("#"))
A=(i - 1 >= 0) B=(list.get(i – 1).equals("#"))
Test Case1: A=TRUE  B=FALSE Decision Outcome: FALSE
Test Case2: A=FALSE B=TRUE  Decision Outcome: FALSE
Test Case3: A=TRUE  B=TRUE  Decision Outcome: TRUE 
Test Case3: A=FALSE B=FALSE Decision Outcome: FALSE 

if (i + 1 < list.size() && list.get(i + 1).equals("#"))
A=(i + 1 >= 0) B=(list.get(i + 1).equals("#"))
Test Case1: A=TRUE  B=FALSE Decision Outcome: FALSE
Test Case2: A=FALSE B=TRUE  Decision Outcome: FALSE
Test Case3: A=TRUE  B=TRUE  Decision Outcome: TRUE 
Test Case3: A=FALSE B=FALSE Decision Outcome: FALSE 

i + 1 < list.size()   list.get(i + 1).equals("#") Outcome (&&)
0                          0                         0
1                          0                         0
0                          1                         0
1                          1                         1



i - 1 < list.size()    list.get(i - 1).equals("#")   Outcome (&&)
0                            0                            0
1                            0                            0
0                            1                            0
1                            1                            1

....

### Тест случаи според критериумот Every statement
.... 
Test Case1:
public List<String> function(List<String> list) {
        if (list.size() <= 0) {
     throw new IllegalArgumentException("List length should be greater than 0");
        }
        List<String> numMines = new ArrayList<>();
        for (int i = 0; i < list.size(); i++) {
            if (!list.get(i).equals("#")) {
                int num = 0;
                if (i - 1 >= 0 && list.get(i - 1).equals("#")) {
                    num++;
                }
                if (i + 1 < list.size() && list.get(i + 1).equals("#")) {
                    num++;
                }
                numMines.add(String.valueOf(num));
            } 
             else {
                numMines.add(list.get(i));
            }
        }
        return numMines;
    } 22vk
Statement Coverage= 5/22 = 23%
Test Case2:
public List<String> function(List<String> list) {
        if (list.size() <= 0) {
            throw new IllegalArgumentException("List length should be greater than 0");
        }
        List<String> numMines = new ArrayList<>();
        for (int i = 0; i < list.size(); i++) {
            if (!list.get(i).equals("#")) {
                int num = 0;
                if (i - 1 >= 0 && list.get(i - 1).equals("#")) {
                    num++;
                }
                if (i + 1 < list.size() && list.get(i + 1).equals("#")) {
                    num++;
                }
                numMines.add(String.valueOf(num));
            } 
else {
                numMines.add(list.get(i));
            }
        }
        return numMines;
    }
Executed – 16/22
Statement Coverage = 16/22 = 73%
Test Case3:
public List<String> function(List<String> list) {
        if (list.size() <= 0) {
            throw new IllegalArgumentException("List length should be greater than 0");
        }
        List<String> numMines = new ArrayList<>();
        for (int i = 0; i < list.size(); i++) {
            if (!list.get(i).equals("#")) {
                int num = 0;
                if (i - 1 >= 0 && list.get(i - 1).equals("#")) {
                    num++;
                }
                if (i + 1 < list.size() && list.get(i + 1).equals("#")) {
                    num++;
                }
                numMines.add(String.valueOf(num));
            } 
else {
                numMines.add(list.get(i));
            }
        }
        return numMines;
    }
Executed - 13
Statement Coverage = 13/22 = 59%
Test Case4:
public List<String> function(List<String> list) {
        if (list.size() <= 0) {
            throw new IllegalArgumentException("List length should be greater than 0");
        }
        List<String> numMines = new ArrayList<>();
        for (int i = 0; i < list.size(); i++) {
            if (!list.get(i).equals("#")) {
                int num = 0;
                if (i - 1 >= 0 && list.get(i - 1).equals("#")) {
                    num++;
                }
                if (i + 1 < list.size() && list.get(i + 1).equals("#")) {
                    num++;
                }
                numMines.add(String.valueOf(num));
            } 
else {
                numMines.add(list.get(i));
            }
        }
        return numMines;
    }
Executed 12
Statement Coverage = 12/22 = 54%
Test Case5:
public List<String> function(List<String> list) {
        if (list.size() <= 0) {
            throw new IllegalArgumentException("List length should be greater than 0");
        }
        List<String> numMines = new ArrayList<>();
        for (int i = 0; i < list.size(); i++) {
            if (!list.get(i).equals("#")) {
                int num = 0;
                if (i - 1 >= 0 && list.get(i - 1).equals("#")) {
                    num++;
                }
                if (i + 1 < list.size() && list.get(i + 1).equals("#")) {
                    num++;
                }
                numMines.add(String.valueOf(num));
            } 
            else {
                numMines.add(list.get(i));
            }
        }
        return numMines;
    }
Executed 10
Statement Coverage = 10/22 = 45%
Test Case6:
public List<String> function(List<String> list) {
        if (list.size() <= 0) {
            throw new IllegalArgumentException("List length should be greater than 0");
        }
        List<String> numMines = new ArrayList<>();
        for (int i = 0; i < list.size(); i++) {
            if (!list.get(i).equals("#")) {
                int num = 0;
                if (i - 1 >= 0 && list.get(i - 1).equals("#")) {
                    num++;
                }
                if (i + 1 < list.size() && list.get(i + 1).equals("#")) {
                    num++;
                }
                numMines.add(String.valueOf(num));
            } 
            else {
                numMines.add(list.get(i));
            }
        }
        return numMines;
    }
Executed 8
Statement Coverage = 8/22 = 36%
### Објаснување на напишаните unit tests

...
...
