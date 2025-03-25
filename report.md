
---

### **2️⃣ `REPORT.md` (For Theory & Analysis)**  
```markdown
# **Exponential, Jump, and Hashing-based Searching Algorithms**

## **Submitted by**  
**Name:** Samuel Diriba  
**Group:** 2  
**ID:** RNS-9464/23  

---

## **1. How the Algorithms Work**  

### **1️⃣ Exponential Search**  
- Used for **unbounded or large sorted arrays**.  
- First finds a range where the target **might** exist by doubling the index (2, 4, 8, 16, …).  
- Then applies **Binary Search** on the identified range.  

### **2️⃣ Jump Search**  
- Works on **sorted arrays** by jumping ahead by fixed steps (`√n`).  
- If the target is in the current jump range, it performs a **linear search** within that range.  
- Faster than **Linear Search** but slower than **Binary Search**.  

### **3️⃣ Hashing-based Search**  
- Uses a **hash table (unordered_map in C++)** for **O(1) average time complexity**.  
- Stores elements in **key-value pairs**, making lookups extremely fast.  
- Used in **databases and caching systems**.  

---

## **2. Complexity Analysis**  

| **Algorithm**          | **Best Case** | **Average Case** | **Worst Case** | **Space Complexity** |
|------------------------|--------------|----------------|--------------|----------------|
| **Exponential Search** | O(1)         | O(log n)       | O(log n)     | O(1) |
| **Jump Search**        | O(1)         | O(√n)         | O(√n)        | O(1) |
| **Hashing Search**     | O(1)         | O(1)          | O(n) (in case of collisions) | O(n) |

---

## **3. Summary of Findings**  
✔ **Exponential Search** is best for **large sorted arrays** when we don’t know the exact size.  
✔ **Jump Search** is a good balance between **Linear and Binary Search** but only works on sorted data.  
✔ **Hashing-based Search** is the **fastest** (O(1) average case), making it ideal for **lookup operations**.  

✅** If data is sorted, **Exponential Search** is great. If data is large and unordered, **Hashing-based Search** is the best choice! 🚀  
