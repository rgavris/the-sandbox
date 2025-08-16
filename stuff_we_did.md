# Learning Journey

A collection of programming concepts, tools, and technologies we've explored.

## 📅 August 16, 2025

### Full Stack Web Development Architecture

**Client Layer**: React (JavaScript, HTML, CSS)  
**API Layer**: Express, FastAPI, or Next.js  
**Database Layer**: Redis, MongoDB, or PostgreSQL

### Also Remember
Prequisites Included:
- CSS, HTML, JS, the browser DOM, React hooks, state, managed components, and more!
- Bash, virtual machines, package managers, dependency trees (that's when npm install keeps adding packages because our packages want packages)
- Git, merge conflicts, GitHub
- Filesystem and Path
- Networking (browser connecting to server via the TCP handshake/dance and then with HTTP requests)
- REST protocol for HTTP requests
- Computer science

#### 🎯 Planned Features
To improve, you simply plan and implement one feature after the other.

- **React UI Components**
- **Client-side CRUD Operations** - Streak component communicates with API
- **API Endpoints** - `/streak` endpoint implementation
- **Database CRUD Operations** - API handles streak data persistence
- **Data Storage** - Database stores streak tracking data
---

Rinse and repeat, one full-stack feature after the next.

#### Architecture

When we choose React + Express + Redis, we have chosen a __tech stack__, and committed to a nice simple app architecture.

**Architecture diagram:**
```
Browser/Client (React) 
    ↓ HTTP Requests
Express API Server
    ↓ Database Queries
Redis/PostgreSQL Database
```

Redis is really fast, Postgres (aka PostgreSQL) is also fast but not as fast. So we often like to store EVERYTHING in Postgres, and SOME THINGS in Redis.

**Hybrid Architecture diagram:**
```
Browser/Client (React)
    ↓ HTTP Requests
Express API Server
    ↓                    ↓
PostgreSQL          Redis Cache
(Persistent Data)   (Fast Access)
```

So we use both at the same time, instead of choosing one.

## 📅 August 2, 2025

### Development Environment & Tools

- ✅ **Learned Vim** - Text editor mastery
- 🛠️ **Struggled with nano** - Command-line text editing challenges
- 🖥️ **Installed WSL** - Windows Subsystem for Linux virtual machine
- ⚙️ **WezTerm Configuration** - Terminal emulator setup and config loading
- 🐚 **Bash Integration** - Using bash inside WezTerm for Unix/Linux commands
- 🔄 **Git Workflow** - Created pull requests and practiced version control

#### 🎮 Learning Resource
[Vim Adventures](https://vim-adventures.com/) - Interactive Vim learning game

---

## 📅 August 9, 2025

### Data Structures & Algorithms

#### 📊 Arrays
```javascript
// Arrays store the START address of contiguous memory cells
const myArray = [1, 2, 3, 4, 5];

// Time Complexity:
// - Access arbitrary element: O(1) - myArray[1000]
// - Push operation: O(1)
// - Pop operation: O(1)
```

#### ⚡ Big O Notation
**Concept**: How performance scales with input size

- **O(n) Example**: Searching 1 million vs 2 million names linearly
- **O(1) Example**: Direct array access `myArray[-1]` (last element)

#### 🗂️ Hash Tables
```javascript
// Object property access
myObject.myNameOfProperty;

// Array-like syntax with keys
myArray['mySuperKey'];

// Concept: Translate keys into array indices
// Benefits: Arbitrary location access with O(1) lookup
```

#### 🔢 Hashing Functions
```javascript
const myHashingFunction = (myKey) => {
  const start = 0;
  for(letter in myKey) {
    return (alphabetWorth(letter) + start) % lengthOfArray;
  }
};
```

**Requirements for good hash functions**:
- **Deterministic** - Same input always produces same output
- **Unique** - Different inputs should produce different outputs
- **Fast** - Quick computation time

---

## 🔢 Number Systems

### Decimal vs Hexadecimal
| Decimal | Hexadecimal | Notes |
|---------|-------------|-------|
| 10      | A           |       |
| 15      | F           |       |
| 16      | 10          |       |
| 26      | 1A          |       |
| 31      | 1F          |       |
| 32      | 20          |       |

**Hexadecimal digits**: `0, 1, 2, 3, 4, 5, 6, 7, 8, 9, A, B, C, D, E, F`

**Why use hex?** Shorter representation for large numbers
- Example: `fa35bc` is much shorter than equivalent decimal

### Hexadecimal Conversion Examples
```
10 hex = 16 decimal
20 hex = 32 decimal  
30 hex = 48 decimal
40 hex = 64 decimal
50 hex = 80 decimal
```

### Binary System
| Binary | Decimal |
|--------|---------|
| 01     | 1       |
| 10     | 2       |
| 11     | 3       |
| 100    | 4       |
| 101    | 5       |

---

*This document tracks our programming learning journey and serves as a reference for concepts we've explored together.*
