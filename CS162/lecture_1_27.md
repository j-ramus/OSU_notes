# Structs

---

midterm feb 07 - no notes

practice midterm on canvas

Optional study session

---

Structs can have structs inside of them -> composition

Initialize `baseball* spaghetti = new baseball[6]`

---

# File i/o

include filestream

declaration: `std::ifstream data_file;`

initialization: `data_file.open("data.txt");`

open is a memeber if the ifstream object type

check if failed: `if (data_file.is_open()){}`

`is_open()` returns a boolean

`.close()` is called automatically when it falls out of scope

stream operators move through file using whitespace as delimiters

pass by reference almost always. Must be non-const because the "cursor" in the file needs to be able to move

---

### ofstreams

declaration: std::ofstream some_cool_file;

initialization: some_cool_file.open("cool_file.txr");

if not opened in append mode, the file is erased upon opening

append: `std::ofstream::app`
