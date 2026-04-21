# PES VCS Lab - Content Addressable Version Control System

## 👨‍💻 Student Details
- Name: P.JAYA SURYA
- SRN: PES1UG24AM210
- Section: D

---

## 📌 Project Description

This project implements a simplified Git-like Version Control System called PES VCS.  
It supports object storage, trees, indexing, commits, and history traversal.

---

## ⚙️ Features Implemented

### Phase 1 - Object Store
- Content-addressable storage using SHA-256
- Blob objects stored in `.pes/objects/`
- Functions:
  - object_write()
  - object_read()

---

### Phase 2 - Tree Objects
- Directory snapshot representation
- Tree serialization and parsing
- Functions:
  - tree_serialize()
  - tree_parse()
  - tree_from_index()

---

### Phase 3 - Index (Staging Area)
- Tracks files to be committed
- Text-based `.pes/index`
- Functions:
  - index_load()
  - index_save()
  - index_add()

---

### Phase 4 - Commit System
- Stores project snapshots
- Maintains commit history
- Functions:
  - commit_create()
  - commit_parse()
  - commit_serialize()
  - commit_walk()

---

## 🚀 How to Run

make  
./pes init  
echo Hello > file.txt  
./pes add file.txt  
./pes commit -m "Initial commit"  
./pes log  

---

## 📸 Screenshots Included

- Phase 1: Object tests

  1-A
  <img width="697" height="164" alt="image" src="https://github.com/user-attachments/assets/401b6640-9524-4087-b063-5c660270a49d" />

  1-B
  <img width="618" height="67" alt="image" src="https://github.com/user-attachments/assets/cd9a77f5-23a6-4c82-b7fc-702bf5dc8167" />
  
- Phase 2: Tree serialization
  
  2-A
  <img width="617" height="137" alt="image" src="https://github.com/user-attachments/assets/e62ffbda-60bf-4cfb-b60c-d91effd3cbb0" />

  2-B
  <img width="946" height="108" alt="image" src="https://github.com/user-attachments/assets/2907f874-c34c-4788-82a3-7502e8bf79cb" />

- Phase 3: Index and status
  
  3-A
  <img width="516" height="395" alt="image" src="https://github.com/user-attachments/assets/c71ccd44-9c98-487a-bb4c-a9af1af6695f" />

  3-B
  <img width="681" height="39" alt="image" src="https://github.com/user-attachments/assets/f19509ea-d972-469f-8558-a63f259533ac" />

- Phase 4: Commit log  

  4-A
  <img width="618" height="370" alt="image" src="https://github.com/user-attachments/assets/d06a7871-92a8-4a96-bf7f-45e38f5ecea8" />

  4-B
  <img width="647" height="391" alt="image" src="https://github.com/user-attachments/assets/f87f4466-90b3-4bae-ab07-fb1bc858de57" />

  4-C
  <img width="581" height="60" alt="image" src="https://github.com/user-attachments/assets/68a0bee8-ee83-49b3-9598-8b3054d86404" />

  FINAL INTEGRATION TEST

  <img width="623" height="932" alt="image" src="https://github.com/user-attachments/assets/f4f9f932-cadf-4c77-b7cd-d765cd21404e" />  

---

## 🧠 Concepts Learned

- Hashing (SHA-256)  
- File system storage  
- Version control internals  
- Trees and commits  
- Atomic file operations  

---

## 📂 Repository Structure

.
├── object.c  
├── tree.c  
├── index.c  
├── commit.c  
├── pes.c  
├── Makefile  
├── README.md  
└── screenshots/  

---

## 🎯 Conclusion

This project helped in understanding how Git internally manages data using content-addressable storage, trees, and commits.
