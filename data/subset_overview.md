# Data Subsets Overview

This folder contains representative subsets of the full production datasets. Each CSV file holds sample records with the same schema and value ranges as the originals.

---

## 1. `FaceInPage.csv`  - Defines user profiles.

- **ID** (int): Unique page owner ID, 1–200,000  
- **Name** (string): 10–20 characters (no commas)  
- **Nationality** (string): 10–20 characters (no commas)  
- **CountryCode** (int): 1–50  
- **Hobby** (string): 10–20 characters  

---

## 2. `Associates.csv`  - Models one-directional friendships.

- **FriendRel** (int): Unique relationship ID, 1–20,000,000  
- **PersonA_ID** (int): Owner ID (1–200,000)  
- **PersonB_ID** (int): Friend’s owner ID (1–200,000; ≠ PersonA_ID)  
- **DateofFriendship** (int): “Date” marker, 1–1,000,000  
- **Desc** (string): 20–50 characters describing relationship type (e.g., college-friend, family)  

> **Note:** Relationships are stored once; if A → B exists, B → A will not.

---

## 3. `AccessLogs.csv`  - Tracks page visits.

- **AccessId** (int): Unique log ID, 1–10,000,000  
- **ByWho** (int): Visitor’s owner ID  
- **WhatPage** (int): Page owner ID being accessed  
- **TypeOfAccess** (string): 20–50 characters describing action (view, note, add friend, etc.)  
- **AccessTime** (int): Timestamp (1–1,000,000 or epoch)  

---
